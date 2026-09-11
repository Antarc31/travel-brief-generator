# Analisi feedback e KPI — Travel AI

Documento vivo: lo aggiorno io (Claude) recuperando i dati reali dai due form Netlify via API, ogni volta che mi chiedi "aggiorna l'analisi feedback" (o simile). Non si aggiorna da solo — vedi nota in fondo.

Fonti dati:
- Form `richiesta-accesso` (chi vuole entrare in beta) — segmentazione + problema dichiarato
- Form `feedback-beta` (chi ha già usato la dashboard) — Fase 4 del piano, Sezione 32 del manuale operativo

**Ultimo aggiornamento:** 2026-09-10 — 0 risposte reali su entrambi i form (solo submission di test create e poi eliminate durante lo sviluppo).

---

## 1. KPI (Sezione 33 del manuale)

| KPI | Valore | Fonte |
|---|---|---|
| Richieste di accesso ricevute | 0 | form `richiesta-accesso` |
| Feedback post-uso ricevuti | 0 | form `feedback-beta` |
| Tasso di risposta al feedback (feedback / accessi) | N/D | richiede almeno 1 accesso |
| % che ha usato la dashboard per tutto il viaggio | N/D | campo `usoDashboard` |
| % disposta a pagare (qualsiasi cifra) | N/D | campo `pagherebbe` |
| % che consiglierebbe (sicuramente/probabilmente sì) | N/D | campo `consiglierebbe` |
| Visite alla landing page | N/D — non tracciato | serve analytics (non ancora installato) |
| Click sulla CTA | N/D — non tracciato | serve analytics |
| Tempo di completamento questionario | N/D — non tracciato | serve analytics sull'app |
| % che riaprono/esportano l'itinerario | N/D — non tracciato | fuori scope attuale (l'app è statica, nessun tracking) |

**Nota:** le righe "N/D — non tracciato" restano vuote finché non si decide di aggiungere un sistema di analytics (es. Plausible, Netlify Analytics a pagamento, o eventi custom). Non è stato richiesto in questa fase — lo segnalo solo perché il manuale le elenca tra le metriche minime.

---

## 2. Segmentazione — Fase 5 del piano

Incrocio tra `tipoViaggio` (form accesso) e le risposte di feedback (`pagherebbe`, `consiglierebbe`, `capitoSituazione`), quando la stessa email compare in entrambi i form.

| Tipo di viaggio | N. richieste accesso | N. feedback ricevuti | Pagherebbe (sì/tot) | Consiglierebbe (sì/tot) |
|---|---|---|---|---|
| Famiglia | 0 | 0 | — | — |
| Coppia | 0 | 0 | — | — |
| Da solo/a | 0 | 0 | — | — |
| Gruppo di amici | 0 | 0 | — | — |
| Viaggio con budget limitato | 0 | 0 | — | — |
| Altro | 0 | 0 | — | — |

**Criterio Fase 5 (dal piano):** serve segnale reale, non impressioni, prima di dichiarare una verticale vincente — tabella vuota finché non arrivano risposte.

---

## 3. Analisi del feedback (Sezione 32 del manuale)

Ogni riga è un feedback testuale (`tempoRisparmiato`, `genericoInutile`, `cosaManca`, `capitoSituazione`) classificato singolarmente.

| Feedback | Categoria | Gravità (1-5) | Frequenza | Impatto | Azione consigliata | Priorità |
|---|---|---|---|---|---|---|
| *(nessuno ancora)* | | | | | | |

Categorie possibili: problema tecnico, problema di chiarezza, problema di qualità, problema di utilità, richiesta di nuova funzione, obiezione, elogio, rischio di rimborso, opportunità di upsell, opportunità di referral.

**Promemoria dal manuale:** non trattare un singolo commento isolato come prova di una domanda di mercato, salvo che sia un errore grave, di sicurezza o di privacy. Servono almeno alcuni segnali coerenti prima di agire.

### Sintesi
- **Tre problemi più urgenti:** N/D — nessun feedback ancora
- **Tre richieste più frequenti:** N/D
- **Cosa correggere subito:** N/D
- **Cosa rimandare:** N/D
- **Cosa eliminare:** N/D
- **Quale domanda fare agli utenti per ottenere informazioni migliori:** N/D

---

## Come aggiornare questo documento

Chiedimi semplicemente "aggiorna l'analisi feedback" (o equivalente). In quel momento:
1. Recupero le submission reali di entrambi i form via API Netlify (`listFormSubmissions`)
2. Ricalcolo i KPI derivabili dai form
3. Classifico ogni nuovo feedback testuale secondo lo schema della Sezione 32
4. Aggiorno la tabella di segmentazione incrociando le email tra i due form
5. Riscrivo la sintesi finale

Non è schedulato: si aggiorna solo quando me lo chiedi (scelta fatta il 2026-09-10 per evitare di gestire un token Netlify separato per un job automatico, dato che al momento non c'erano ancora dati reali da analizzare). Se in futuro arrivano abbastanza risposte da volere un aggiornamento periodico senza doverlo chiedere ogni volta, si può configurare un agente schedulato con un Personal Access Token Netlify dedicato.
