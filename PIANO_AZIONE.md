# Piano d'azione — Lancio Travel AI Business

Documento operativo, separato dalla cartella di contesto (00-11): quei file raccontano cosa sappiamo, questo dice cosa fare, in che ordine, e quando si può passare al passo successivo. Si aggiorna spuntando le fasi, non riscrivendo la strategia ogni volta.

**Regola di manutenzione:** la cartella TRAVEL_AI_BUSINESS (00-11) si aggiorna solo quando una fase qui sotto produce un dato reale (un tester ottenuto, un prezzo confermato, una verticale che converte) — non per ogni ipotesi discussa in chat.

**Decisione presa:** outreach ampio, multi-verticale, senza filtrare per nicchia in questa fase. Il prodotto resta generico; il form raccoglie il tipo di viaggiatore per segmentare *dopo*, sui dati reali — non si sceglie una nicchia a tavolino.

---

## FASE 0 — Decisioni bloccanti
**Stato: completata**

| Decisione | Dettaglio | Stato |
|---|---|---|
| Hosting | Netlify (deploy via CLI) | Fatto — https://radiant-tarsier-d8da3a.netlify.app |
| Dominio | Sottodominio netlify.app provvisorio, dominio proprio da valutare più avanti | Fatto (provvisorio) |

**Criterio per passare alla Fase 1:** hai un URL pubblico funzionante su cui pubblicare qualcosa. ✅

---

## FASE 1 — Prodotto pronto
**Stato: quasi completo**

- [x] Questionario e generazione brief funzionanti (`generatore-viaggio.html`)
- [x] Regole di affidabilità dati rafforzate nelle istruzioni AI (fatto/inferenza/ipotesi, fonti ufficiali, coerenza itinerario)
- [x] Pubblicazione online del prodotto — live su /app/ (https://radiant-tarsier-d8da3a.netlify.app/app/)
- [ ] Test end-to-end personale: completare un itinerario vero prima di mandarlo a chiunque

**Criterio per passare alla Fase 2:** hai usato tu stesso il prodotto pubblicato online, dall'inizio alla fine, senza errori bloccanti.

---

## FASE 2 — Landing page e form
**Stato: completata** (landing, form e redirect pubblicati e testati; resta consigliato un check veloce personale da telefono reale, il test automatico ha coperto solo layout/refresh/invio dati, non la resa visiva su Safari reale)

**Landing generica (non tagliata su una nicchia):**
- Titolo: "Organizza il tuo viaggio in un unico posto, senza passare ore tra decine di app e tab."
- Sottotitolo, esempio visivo (screenshot reali, non stock), problema, come funziona (3 passi), cosa ricevi, "per chi è" con più profili elencati in parallelo (famiglie, coppie, budget...), "cosa non è", un solo CTA finale.

**Form (8-10 domande), le due chiave da non perdere:**
- "Qual è la parte più difficile nell'organizzare questo viaggio?" (linguaggio reale del cliente)
- "Tipo di viaggio" (famiglia, coppia, solo, budget, gruppo...) — è il campo che userai per segmentare in Fase 5

**Criterio per passare alla Fase 3:** landing e form pubblicati, testati su telefono e desktop, form che salva correttamente le risposte. ✅

---

## FASE 3 — Outreach ampio
**Stato: da fare — dipende da Fase 2**

- Obiettivo: 30 contatti, filtrando solo per "problema di viaggio concreto e attivo", non per tipo di viaggiatore
- Canali: gruppi Facebook viaggi, Reddit (r/travel, r/ItalyTravel), commenti sotto creator travel di qualsiasi tipo, forum, gruppi expat, WhatsApp/Telegram viaggiatori
- Ritmo: almeno 10 contatti al giorno
- Messaggio tipo: "Ciao, ho visto che stai organizzando un viaggio. Sto testando uno strumento che crea una dashboard personalizzata con itinerario, spostamenti e attività organizzate giorno per giorno. Sto cercando persone che stiano davvero pianificando un viaggio, disposte a usarlo e darmi feedback sincero."

**Criterio per passare alla Fase 4:** 10-20 persone hanno accettato di provare il prodotto.

---

## FASE 4 — Test prodotto e prezzo
**Stato: da fare — dipende da Fase 3**

- 5 tester gratuiti → feedback approfondito
- 5-10 tester beta a pagamento (€10-20) → verifica disponibilità reale a pagare
- Domande di feedback: cosa ha risparmiato tempo, cosa era generico/inutile, ha seguito l'itinerario, cosa avrebbe fatto con ChatGPT/Google, cosa manca, pagherebbe €29/€49/€79, lo consiglierebbe
- Domanda aggiuntiva per la segmentazione: il prodotto ha funzionato bene per il suo tipo di viaggio specifico, o sentiva che non capiva la sua situazione?

**Criterio go/no-go:** se nessuno paga nemmeno €10-20, il problema non è ancora dimostrato abbastanza urgente — si torna a rivedere promessa o pubblico, non si passa alla fase successiva.

**Criterio per passare alla Fase 5:** hai risposte da almeno 8-10 tester, con almeno alcuni pagamenti confermati.

---

## FASE 5 — Segmentazione sui dati reali
**Stato: da fare — dipende da Fase 4**

- Incrocia le risposte del form (tipo di viaggio) con: chi ha usato di più il prodotto, chi ha dato il feedback migliore, chi ha pagato più volentieri
- Identifica **una verticale vincente** (es. famiglie, coppie, budget) con più segnale delle altre
- Le verticali non vincenti non si scartano: restano candidate per un secondo giro, dopo aver validato la prima

**Criterio per passare alla Fase 6:** hai identificato quale tipo di viaggiatore converte meglio, con numeri reali a supporto (non impressioni).

---

## FASE 6 — Contatto creator (solo sulla verticale vincente)
**Stato: da fare — dipende da Fase 5**

- Usa i candidati già mappati per nicchia (vedi 03_Creator_DNA nella cartella di contesto): famiglie → @viaggiapiccoli e alternative; coppie → @martiquestonomegiaesisteva, @dueromaniazonzo; budget → @viaggiasenzanalira
- Prima di contattare: controllare ultimi 10-20 contenuti, domande nei commenti, cosa vende già, se è concorrenza diretta o segnale di validazione
- Messaggio con demo concreta (screenshot, feedback reali dei tester), non solo l'idea descritta

**Criterio per passare alla Fase 7:** almeno un creator ha risposto positivamente ed è disponibile a discutere un pilot.

---

## FASE 7 — Pilot con creator
**Stato: non ancora raggiungibile**

- Durata consigliata: 60-90 giorni
- Da definire prima dell'inizio: prodotto, destinazione, pubblico, prezzo, canale di vendita, calendario, responsabilità reciproche, revenue share (vedi 07_Offer_and_Pricing e 11_Legal_and_Ownership)
- Obiettivo: dati sufficienti per decidere se continuare, modificare o fermare

---

## Vista rapida — cosa fare adesso

1. **Ora:** Fase 0 — scegliere hosting (Netlify o Vercel) e dominio provvisorio
2. **Poi:** Fase 1 — pubblicare il prodotto online e testarlo tu stesso
3. **Poi:** Fase 2 — scrivere e pubblicare landing + form
4. Tutto il resto segue in ordine, senza saltare fasi

Ogni fase ha un criterio esplicito per passare alla successiva: se non è soddisfatto, non si avanza, si corregge.
