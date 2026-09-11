# Manuale Operativo — Travel AI Business

## Sezione 1. Obiettivo del progetto

Il progetto consiste nello sviluppo di un prodotto digitale capace di creare itinerari personalizzati per persone che vogliono viaggiare in Italia.

Il prodotto parte da informazioni fornite dall'utente, come:

- destinazione
- date
- durata del viaggio
- budget
- interessi
- ritmo desiderato
- composizione del gruppo
- preferenze alimentari
- necessità di trasporto
- eventuali limitazioni
- esperienze già prenotate

L'obiettivo non è creare una semplice lista di luoghi. L'obiettivo è ridurre il tempo necessario per organizzare il viaggio e trasformare informazioni sparse in un piano pratico, leggibile e personalizzato.

Il prodotto deve aiutare l'utente a passare da:

> "Non so cosa vedere, come organizzarmi e cosa prenotare"

a:

> "Ho un itinerario chiaro, coerente con le mie preferenze e pronto da verificare e utilizzare".

La prima applicazione è il mercato italiano, con possibilità di iniziare da una singola destinazione o da una nicchia specifica.

Esempi:

- weekend romantici a Roma
- viaggi gastronomici in Emilia-Romagna
- itinerari per famiglie in Toscana
- viaggi economici in Sicilia
- itinerari di lusso sul Lago di Como
- viaggi fotografici nelle Dolomiti
- percorsi per digital nomad
- viaggi senza automobile
- itinerari per coppie over 50
- esperienze locali lontane dalle attrazioni più turistiche

## Sezione 2. Distinzione tra funzione, prodotto e business

Una funzione è una capacità tecnica.

Esempio: "Genera un itinerario con l'intelligenza artificiale".

Un prodotto è una funzione inserita in un'esperienza completa, con un pubblico preciso, una promessa, un risultato e un modo semplice per acquistarlo e usarlo.

Esempio: "Ricevi in 10 minuti un itinerario di 5 giorni a Roma, costruito per coppie che vogliono vedere i luoghi principali senza correre e senza perdere tempo nella ricerca".

Un business richiede anche:

- distribuzione
- acquisizione clienti
- pricing
- supporto
- aggiornamento dei dati
- responsabilità
- proprietà degli asset
- sistema di feedback
- margini
- capacità di replicare il processo

Il generatore tecnico da solo non è ancora il business.

Il business nasce quando una persona specifica è disposta a pagare per ottenere una trasformazione concreta.

## Sezione 3. Valutazione del prototipo attuale

Il prototipo HTML rappresenta un buon punto di partenza per validare il concetto.

Le funzioni già presenti o ipotizzate includono:

- dashboard
- raccolta delle preferenze
- generazione dell'itinerario
- salvataggio tramite localStorage
- visualizzazione delle giornate
- export in formato .ics
- deploy tramite Netlify

Queste funzioni sono sufficienti per creare una demo e mostrare il prodotto a potenziali utenti o creator.

Non sono ancora sufficienti per sostenere una crescita significativa.

Prima di costruire nuove funzioni è necessario verificare:

- se gli utenti capiscono il prodotto
- se completano il questionario
- se l'itinerario sembra davvero personalizzato
- se utilizzano l'itinerario durante il viaggio
- se esportano il calendario
- se sarebbero disposti a pagare
- quali errori si ripetono
- quanto tempo richiede l'assistenza

La priorità non è rendere il prodotto più complesso. La priorità è dimostrare che risolve un problema reale.

## Sezione 4. Il posizionamento

Un generatore generalista deve competere con: ChatGPT, Google, blog di viaggio, TikTok, Instagram, TripAdvisor, Google Maps, app di viaggio, agenzie tradizionali.

Competere frontalmente contro tutti questi strumenti è una cattiva strategia.

Il prodotto deve invece diventare più specifico.

La domanda corretta non è: "Come creo il miglior itinerario per chiunque?"

La domanda corretta è: "Per quale tipo di viaggiatore posso creare un'esperienza molto più utile di una soluzione generica?"

Il posizionamento deve contenere almeno quattro elementi:

1. pubblico specifico
2. destinazione o tipo di viaggio
3. problema concreto
4. risultato desiderato

**Formula:** "Aiutiamo [pubblico] a vivere [tipo di viaggio] in [destinazione] senza [problema principale], attraverso [meccanismo distintivo]".

Esempio: "Aiutiamo coppie che visitano Roma per la prima volta a vedere le attrazioni principali senza passare il viaggio a organizzare orari, spostamenti e prenotazioni".

## Sezione 5. Core engine e layer di personalizzazione

Il modello più efficiente è costruire un core engine riutilizzabile e aggiungere layer specifici.

**Il core engine contiene:** raccolta input, logica di pianificazione, struttura giornaliera, gestione delle preferenze, calcolo dei tempi, gestione delle alternative, esportazione calendario, controllo di completezza, sistema di feedback.

**Il layer destinazione contiene:** luoghi, quartieri, attrazioni, ristoranti, trasporti, eventi, stagionalità, tempi medi, avvertenze, dati da verificare.

**Il layer nicchia contiene:** esigenze del pubblico, tono, priorità, esclusioni, livello di budget, ritmo di viaggio, problemi ricorrenti.

**Il layer creator contiene:** voce, valori, preferenze, stile, raccomandazioni, punti di vista, contenuti già pubblicati, rapporto con il pubblico.

**Il distribution layer contiene:** contenuti, landing page, email, call to action, partnership, offerte, campagne, referral.

Questa architettura permette di cambiare destinazione o creator senza ricostruire tutto il prodotto.

## Sezione 6. Perché partire da una nicchia

Una nicchia riduce la concorrenza percepita e rende la promessa più credibile.

Un itinerario generico può sembrare facilmente sostituibile. Un itinerario costruito per un bisogno specifico ha maggiore valore percepito.

Esempi di nicchie: famiglie con bambini piccoli, coppie in viaggio romantico, viaggiatori con budget limitato, persone che vogliono viaggiare senza auto, persone con pochi giorni a disposizione, viaggiatori interessati al cibo, persone che cercano esperienze locali, viaggiatori senior, persone con esigenze di accessibilità, viaggiatori che vogliono fotografare una destinazione, nomadi digitali, persone che viaggiano con animali.

La nicchia non deve essere scelta soltanto perché sembra interessante. Deve avere: un problema frequente, capacità di spesa, urgenza, accesso a canali di distribuzione, possibilità di raggiungere il pubblico, una promessa realizzabile.

## Sezione 7. La trasformazione promessa

Il prodotto non vende informazioni su una destinazione. Vende chiarezza, risparmio di tempo, riduzione dello stress e maggiore sicurezza nella pianificazione.

La trasformazione deve essere concreta. Esempi:

- da una lista disordinata a un itinerario giornaliero
- da troppe opzioni a una selezione ragionata
- da giornate sovraccariche a un ritmo sostenibile
- da ricerca infinita a un piano pronto da verificare
- da luoghi casuali a esperienze coerenti con gli interessi
- da paura di perdere tempo a maggiore controllo del viaggio

La promessa deve evitare espressioni assolute come: viaggio perfetto, miglior itinerario possibile, zero problemi, tutto garantito, nessun imprevisto.

Una promessa più credibile è: "Un itinerario personalizzato e pratico, costruito sulle tue preferenze, con indicazioni chiare su cosa verificare prima della partenza".

## Sezione 8. Modello creator plus operator

**Il creator possiede normalmente:** attenzione, fiducia del pubblico, distribuzione, stile comunicativo, conoscenza delle domande frequenti, contesto personale, credibilità nella nicchia.

**L'operatore possiede o coordina:** strategia, prodotto, automazioni, AI, landing page, funnel, analytics, supporto, miglioramento continuo, controllo qualità.

Il creator non deve necessariamente costruire il prodotto. L'operatore non deve necessariamente diventare il volto del prodotto.

Il modello funziona quando entrambi portano una risorsa complementare: il creator porta distribuzione e contesto, l'operatore porta esecuzione e infrastruttura.

Il prodotto viene venduto con il brand o la voce del creator, mentre il lavoro operativo viene standardizzato dietro le quinte.

## Sezione 9. Criteri per scegliere un creator

Un creator interessante non è necessariamente quello con più follower.

**Valutare:** qualità dei commenti, frequenza delle domande, rapporto tra visualizzazioni e interazioni, chiarezza della nicchia, fiducia del pubblico, coerenza delle destinazioni trattate, presenza di problemi ripetuti, disponibilità a vendere, storia di collaborazioni, qualità della comunicazione, capacità di produrre contenuti con una call to action, assenza di conflitti con prodotti già esistenti.

**Segnali positivi:** il pubblico chiede spesso consigli pratici; il creator risponde con esperienza personale; esistono domande su itinerari, costi e organizzazione; le persone chiedono link, mappe o guide; il creator ha già venduto qualcosa; il pubblico mostra intenzione di viaggio; i commenti sono specifici e non soltanto complimenti.

**Segnali negativi:** engagement artificiale; pubblico non coerente; contenuti troppo generici; creator non affidabile; nessuna disponibilità a promuovere; aspettative economiche non realistiche; assenza di chiarezza su proprietà e responsabilità.

## Sezione 10. Analisi AI del creator

Non è necessario guardare manualmente ogni reel. È possibile creare un campione rappresentativo e analizzarlo con l'AI.

**Raccogliere:** bio, ultimi 20-50 contenuti, caption, trascrizioni, titoli, commenti, domande ricevute, contenuti con maggiore engagement, call to action, eventuali prodotti già venduti.

**L'analisi deve cercare:** argomenti ricorrenti, problemi del pubblico, desideri, obiezioni, tono, parole ricorrenti, format più efficaci, destinazioni più richieste, domande con intento d'acquisto, elementi che il pubblico associa al creator.

**L'AI deve separare:**
- **Fatti**: informazioni direttamente presenti nei contenuti.
- **Inferenze**: conclusioni ragionevoli basate su più segnali.
- **Ipotesi**: idee ancora da validare con il creator o con il pubblico.

Non trattare un singolo commento come prova di una domanda di mercato. La frequenza e la qualità del segnale sono più importanti del volume grezzo.

## Sezione 11. Creator DNA

Il Creator DNA è il profilo operativo del creator.

Non serve a copiare il creator. Serve a capire come costruire un prodotto coerente con la sua esperienza, il suo modo di comunicare, il suo pubblico, i suoi valori, le sue destinazioni, i problemi che il pubblico gli affida.

**Deve contenere:** nome e handle, piattaforme principali, lingua, paese, nicchia, destinazioni trattate, tipo di pubblico, età e profilo del pubblico, interessi, paure, desideri, ostacoli, domande frequenti, obiezioni, stile comunicativo, parole ricorrenti, valori, contenuti migliori, prodotti già venduti, esperienze personali rilevanti, elementi da evitare, possibili prodotti, dati non ancora verificati.

Il documento deve distinguere chiaramente tra ciò che il creator ha detto, ciò che è stato osservato e ciò che è soltanto ipotizzato.

## Sezione 12. Analisi del pubblico

Il pubblico deve essere analizzato come un gruppo di persone con problemi simili, non come una massa indistinta.

**Analizzare:** chi guarda, perché guarda, cosa cerca, cosa ha già provato, cosa lo blocca, cosa desidera ottenere, quanto è vicino a un acquisto, quali parole usa per descrivere il problema, quali contenuti salva, quali commenti ricevono più risposte, quali domande si ripetono.

**Dividere i commenti in livelli:**

- **Livello 1 — interesse generale.** Es: "Che posto bellissimo".
- **Livello 2 — interesse pratico.** Es: "Quanti giorni servono per visitare questa zona?"
- **Livello 3 — intenzione concreta.** Es: "Parto a giugno con due bambini. Come organizzeresti quattro giorni?"
- **Livello 4 — intenzione d'acquisto.** Es: "Avete una guida o un itinerario già pronto da comprare?"

I commenti di livello 3 e 4 sono quelli più utili per validare un prodotto.

## Sezione 13. Ricerca delle opportunità

Dopo avere analizzato creator e pubblico, creare almeno cinque ipotesi di prodotto.

**Ogni ipotesi deve includere:** nome provvisorio, pubblico, destinazione, problema, trasformazione, formato, contenuto, prezzo ipotetico, motivo per cui il creator è credibile, prova disponibile, rischio principale, metodo di validazione.

**Esempio:**
- Nome: Roma senza stress.
- Pubblico: Coppie alla prima visita a Roma.
- Problema: Troppe attrazioni, spostamenti confusi e giornate sovraccariche.
- Trasformazione: Itinerario di quattro giorni con ritmo sostenibile, zone raggruppate e alternative in caso di pioggia.
- Formato: Questionario più itinerario personalizzato più calendario.
- Validazione: Landing page, lista d'attesa e pilot con un piccolo gruppo di clienti.

Non scegliere l'idea più creativa. Scegliere quella con la combinazione migliore tra: problema, domanda, accesso al pubblico, credibilità, velocità di realizzazione, possibilità di miglioramento.

## Sezione 14. Scelta dell'offerta

L'offerta deve essere semplice da capire.

**Struttura minima:** risultato, per chi è, cosa include, come funziona, quanto tempo richiede, cosa non include, prezzo, assistenza, condizioni di rimborso, call to action.

Esempio: "Compila il questionario sul tuo viaggio e ricevi un itinerario personalizzato di cinque giorni in Toscana, organizzato in base al tuo budget, al tuo ritmo e ai tuoi interessi".

**Possibili livelli di offerta:**
1. itinerario base
2. itinerario personalizzato
3. itinerario personalizzato più calendario
4. itinerario più supporto umano
5. pacchetto premium per gruppi o famiglie

Non creare cinque livelli prima di avere validato il primo. Il primo prodotto deve essere abbastanza completo da produrre un risultato, ma abbastanza semplice da poter essere corretto rapidamente.

## Sezione 15. MVP concierge

Il primo MVP non deve essere completamente automatizzato.

**Il modello concierge consiste nel:**
1. vendere il prodotto
2. raccogliere le informazioni tramite questionario
3. usare l'AI per creare una prima versione
4. controllare manualmente l'output
5. correggere dati, tempi e coerenza
6. consegnare l'itinerario
7. chiedere feedback
8. documentare ogni problema

**Questo approccio permette di capire:** quali input servono davvero, quali domande sono inutili, quali errori commette l'AI, quali parti richiedono controllo umano, quali richieste si ripetono, quale formato è più utile, quanto tempo richiede ogni consegna.

Automatizzare troppo presto nasconde gli errori dietro una bella interfaccia. Prima bisogna capire il processo manuale. Poi si automatizzano le parti ripetitive.

## Sezione 16. Validazione

La validazione deve avvenire prima di costruire funzioni avanzate.

**Procedura:**
1. scegliere una nicchia
2. definire una promessa
3. creare una landing page semplice
4. mostrare un esempio di risultato
5. chiedere una pre-iscrizione o una vendita
6. consegnare manualmente a un piccolo gruppo
7. misurare utilizzo e soddisfazione
8. correggere il prodotto
9. ripetere

La validazione non consiste nel chiedere soltanto: "Compreresti questo prodotto?" — le persone spesso rispondono in modo positivo senza acquistare.

**Segnali più forti:** lasciano l'email, rispondono al questionario, prenotano una call, pagano, usano il prodotto, chiedono aggiornamenti, consigliano il prodotto, chiedono una versione per un'altra destinazione.

La vendita è un segnale più forte di un complimento.

## Sezione 17. Pilot con un creator

Il pilot deve avere durata, obiettivo e responsabilità chiare.

**Durata consigliata:** 60-90 giorni.

**Prima dell'inizio definire:** prodotto, destinazione, pubblico, prezzo, canale di vendita, numero minimo di contenuti, calendario di pubblicazione, responsabilità del creator, responsabilità dell'operatore, gestione del supporto, gestione dei rimborsi, accesso ai dati, proprietà degli asset, modalità di uscita, criteri di successo.

Il pilot non deve essere una collaborazione indefinita. Deve produrre dati sufficienti per decidere se: continuare, modificare l'offerta, cambiare il pubblico, cambiare la destinazione, cambiare il creator, interrompere il progetto.

## Sezione 18. Revenue share

La revenue share deve essere negoziata sulla base del contributo reale di ogni parte.

**Possibili fattori:** chi crea il prodotto, chi sostiene i costi tecnici, chi porta il traffico, chi gestisce il supporto, chi gestisce i rimborsi, chi possiede il brand, chi possiede il codice, chi crea i contenuti, chi assume il rischio operativo, chi mantiene il prodotto aggiornato.

**Non discutere soltanto la percentuale. Definire anche:** ricavi lordi o netti, costi deducibili, commissioni di pagamento, tasse, rimborsi, tempi di pagamento, accesso ai dati, durata della collaborazione, uso del contenuto, proprietà dei clienti, proprietà del codice, condizioni di uscita.

Una percentuale alta su un modello non validato vale meno di un accordo chiaro e sostenibile.

Formalizzare sempre l'accordo in modo adeguato alla situazione e ottenere consulenza professionale quando necessario.

## Sezione 19. Proprietà e responsabilità

**Prima di lanciare il prodotto, chiarire chi possiede:** codice, dominio, brand, logo, account email, account di pagamento, database, dati clienti, landing page, contenuti, prompt, automazioni, analytics, profili social, materiali del creator.

**Chiarire anche chi è responsabile di:** aggiornamento dei luoghi, controllo dei link, accuratezza dei dati, assistenza, richieste di rimborso, privacy, sicurezza, comunicazioni con il cliente, gestione degli incidenti.

Non dare per scontato che chi ha creato un asset ne sia automaticamente il proprietario. La proprietà deve essere definita per iscritto.

## Sezione 20. Struttura delle cartelle di contesto

Creare una cartella principale chiamata `TRAVEL_AI_BUSINESS`, con all'interno:

- `00_Project_Brief` — descrizione del progetto, obiettivo, fase attuale, pubblico, destinazioni, modello di business, vincoli, decisioni prese, decisioni ancora aperte.
- `01_Product_Core` — funzioni, flusso utente, questionario, struttura dell'itinerario, regole di generazione, formato di consegna, export calendario, limiti tecnici, problemi conosciuti.
- `02_Niche_Profile` — nicchia, problema, desideri, obiezioni, budget, linguaggio, destinazioni preferite, alternative già utilizzate.
- `03_Creator_DNA` — bio, tono, valori, contenuti, parole ricorrenti, posizionamento, pubblico, domande, prodotti già venduti.
- `04_Audience_Research` — commenti, sondaggi, interviste, domande frequenti, desideri, paure, obiezioni, segnali d'acquisto, temi ricorrenti.
- `05_Destination_Database` — luoghi, categorie, zone, coordinate, tempi, accessibilità, trasporti, fonti, data dell'ultima verifica, livello di affidabilità.
- `06_Rules_and_Exclusions` — luoghi da evitare, promesse vietate, dati non verificati, limiti dell'AI, criteri di sicurezza, condizioni per suggerire alternative, regole per famiglie, mobilità ridotta e budget.
- `07_Offer_and_Pricing` — offerte, prezzi, bonus, condizioni, rimborsi, upsell, revenue share, costi.
- `08_Brand_Voice` — tono, parole da usare, parole da evitare, esempi, stile del creator, regole di comunicazione.
- `09_Funnel_and_Content` — landing page, email, contenuti, hook, call to action, calendario editoriale, messaggi outreach, campagne.
- `10_Feedback_and_Analytics` — KPI, feedback, errori, rimborsi, richieste, test, decisioni, versioni del prodotto.
- `11_Legal_and_Ownership` — accordi, proprietà, responsabilità, privacy, termini, supporto, gestione dei dati, condizioni di uscita.

Ogni file deve avere: data di aggiornamento, autore, versione, fonti, elementi verificati, elementi da verificare.

Non inserire informazioni inventate soltanto per completare un file.

## Sezione 21. Questionario per l'utente

Il questionario deve raccogliere soltanto informazioni utili a creare un itinerario migliore.

**Dati essenziali:** destinazione, date del viaggio, numero di giorni, numero di viaggiatori, età dei partecipanti, budget indicativo, ritmo desiderato, interessi, luoghi già visitati, luoghi assolutamente da vedere, preferenze alimentari, necessità di trasporto, disponibilità di automobile, esigenze di accessibilità, presenza di bambini, orari di arrivo e partenza, prenotazioni già effettuate, preferenze per mattina/pomeriggio/sera, attività da evitare, livello di flessibilità.

Usare domande semplici e comprensibili. Evitare questionari troppo lunghi: ogni domanda deve avere una funzione. Se una domanda non modifica il risultato finale, eliminarla o renderla facoltativa.

Il questionario deve includere una schermata finale che riassume i dati inseriti prima della generazione. L'utente deve poter correggere le risposte.

**Se mancano informazioni importanti, il sistema deve:** fare una domanda aggiuntiva, utilizzare un'impostazione predefinita dichiarandola, oppure segnalare che il risultato sarà meno preciso.

Non trattare mai un dato mancante come se fosse una preferenza.

## Sezione 22. Struttura dell'itinerario

**Ogni giornata dovrebbe contenere:** data, zona principale, obiettivo della giornata, attività mattutina, pausa o pranzo, attività pomeridiana, cena o attività serale, tempi stimati, spostamenti, alternativa in caso di pioggia, cosa prenotare, cosa verificare, livello di energia richiesto, note personalizzate.

L'itinerario deve avere un ritmo realistico. Non inserire troppe attività nella stessa giornata solo per mostrare più valore. Raggruppare luoghi geograficamente vicini quando possibile.

**Considerare:** tempo per gli spostamenti, code, pause, pasti, ritardi, orientamento, stanchezza, orari di apertura, necessità di prenotazione.

Ogni giornata deve essere eseguibile, non soltanto interessante da leggere.

## Sezione 23. Personalizzazione

La personalizzazione deve modificare concretamente il risultato. Non è sufficiente cambiare il nome dell'utente o inserire i suoi interessi in una frase.

**La personalizzazione può modificare:** scelta delle attrazioni, ordine delle attività, durata delle visite, zone incluse, ritmo della giornata, modalità di trasporto, livello di spesa, numero di pause, alternative, ristoranti, esperienze, livello di dettaglio.

**Esempio — viaggiatore interessato alla gastronomia dovrebbe ricevere:** mercati, botteghe, ristoranti coerenti con il budget, esperienze culinarie, quartieri con identità gastronomica, indicazioni su prenotazioni e orari.

**Esempio — viaggiatore con bambini dovrebbe ricevere:** attività più brevi, pause frequenti, luoghi accessibili, bagni o servizi quando verificabili, alternative in caso di stanchezza, minore densità di spostamenti.

Se la personalizzazione non cambia il piano, il sistema non sta davvero personalizzando.

## Sezione 24. Regole di generazione

**Regole principali:**
1. non creare un itinerario impossibile da completare
2. non inserire attività incompatibili con gli orari disponibili
3. non suggerire luoghi chiusi senza segnalarlo
4. non presentare prezzi non verificati come definitivi
5. non inventare link
6. non inventare eventi
7. non garantire disponibilità
8. non ignorare la durata degli spostamenti
9. non riempire ogni minuto della giornata
10. non utilizzare dati personali oltre ciò che è necessario
11. non proporre attività rischiose senza avvertenze
12. non consigliare luoghi in base a informazioni non confermate
13. non duplicare la stessa attività
14. non creare contraddizioni tra giornate
15. non proporre prenotazioni già incompatibili con il programma

Quando il sistema non dispone di un dato affidabile, deve scrivere: "Verificare prima della partenza". Non utilizzare formulazioni come "È sicuramente aperto" — usare invece "Gli orari possono cambiare. Verifica sul sito ufficiale prima di organizzare la visita".

## Sezione 25. Fact checking

**Informazioni dinamiche da trattare con cautela:** orari, prezzi, disponibilità, eventi, chiusure, lavori, prenotazioni, trasporti, scioperi, regole di accesso, tasse, restrizioni.

**Per ogni informazione importante salvare:** valore, fonte, URL, data della verifica, responsabile della verifica, livello di affidabilità, data consigliata per una nuova verifica.

**Classificazione delle fonti:**
- **Livello A** — fonte ufficiale della struttura, del museo, del comune, della regione o del servizio di trasporto.
- **Livello B** — fonte affidabile e aggiornata, come una camera di commercio, un ente turistico o un'organizzazione riconosciuta.
- **Livello C** — blog, forum, social, recensione o contenuto individuale.

Le fonti di livello C possono aiutare a trovare idee, ma non devono essere utilizzate da sole per confermare informazioni critiche.

## Sezione 26. Fonti e link

Non creare mai un link partendo da un'ipotesi. Un link deve essere: copiato da una fonte reale, controllato, associato al luogo corretto, aggiornato, presentato con chiarezza.

Se non esiste una fonte verificata, utilizzare una descrizione senza link e indicare cosa l'utente deve cercare. Esempio: "Verifica il sito ufficiale del museo per orari, prezzi e prenotazioni".

**Non utilizzare link:** abbreviati senza conoscere la destinazione, provenienti da fonti dubbie, non più funzionanti, che portano a pagine generiche, che mostrano informazioni obsolete.

Programmare un controllo periodico dei link principali.

## Sezione 27. Date, fusi orari ed export .ics

**Il sistema deve distinguere:** data locale, ora locale, fuso orario, data di arrivo, data di partenza, attività che attraversano la mezzanotte, orari di check-in e check-out, durata dell'attività, orari indicativi e orari confermati.

**Prima di generare un file `.ics`, controllare:** formato della data, fuso orario, data di inizio, data di fine, durata, titolo dell'evento, descrizione, luogo, eventuale link, duplicati, ordine cronologico.

**L'export deve essere testato su almeno:** Google Calendar, Apple Calendar, Outlook, un dispositivo mobile.

Se l'orario non è verificato, non inserirlo come evento definitivo senza una nota. L'utente deve sapere che il calendario è un supporto organizzativo e non sostituisce la conferma ufficiale di una prenotazione.

## Sezione 28. LocalStorage e limiti tecnici

Il localStorage è utile per un prototipo, ma non deve essere trattato come un database professionale.

**Limiti:** dati salvati soltanto sul dispositivo e nel browser, perdita possibile dopo cancellazione dei dati, nessuna sincronizzazione automatica, nessun backup garantito, problemi se l'utente cambia dispositivo, possibile superamento dello spazio disponibile, vulnerabilità se vengono salvati dati sensibili, incompatibilità tra browser o modalità privata.

**Non salvare nel localStorage:** password, dati di pagamento, documenti, informazioni sanitarie, dati personali non necessari, token segreti, chiavi API, informazioni altamente sensibili.

**Per il prototipo, utilizzare localStorage soltanto per:** preferenze non sensibili, stato temporaneo, itinerari salvati localmente, impostazioni, dati di test.

Informare l'utente se i dati non vengono sincronizzati.

**In una versione più avanzata valutare:** autenticazione, database, backup, sincronizzazione, controllo accessi, cancellazione account, esportazione dati, log degli aggiornamenti.

## Sezione 29. API e sicurezza

Le chiavi API non devono essere inserite nel codice frontend pubblico.

**Il frontend non deve contenere:** API key, credenziali, password, token amministrativi, segreti di pagamento, accessi al database.

Utilizzare un backend o un ambiente server-side per proteggere le credenziali.

**Applicare:** limiti di utilizzo, controllo dei costi, autenticazione, validazione degli input, protezione contro richieste automatiche, log, monitoraggio degli errori, gestione dei timeout, fallback quando il servizio AI non risponde.

Non inviare al modello più dati personali del necessario.

**Prima di usare contenuti del creator o commenti degli utenti, stabilire:** quali dati vengono raccolti, perché vengono raccolti, chi può accedervi, quanto tempo vengono conservati, come possono essere cancellati, se vengono utilizzati per addestramento o analisi, come viene informato l'utente.

Per questioni legali specifiche, privacy e GDPR, rivolgersi a un professionista qualificato.

## Sezione 30. Prompt operativo per generare un itinerario

```
Agisci come pianificatore di viaggi per [DESTINAZIONE].

Crea un itinerario per:
- numero di viaggiatori: [NUMERO]
- età: [ETÀ]
- date: [DATE]
- durata: [NUMERO GIORNI]
- arrivo: [LUOGO E ORA]
- partenza: [LUOGO E ORA]
- budget: [BUDGET]
- ritmo: [LENTO, MEDIO O INTENSO]
- interessi: [INTERESSI]
- attività desiderate: [ATTIVITÀ]
- attività da evitare: [ESCLUSIONI]
- trasporto disponibile: [TRASPORTO]
- esigenze particolari: [ESIGENZE]
- prenotazioni esistenti: [PRENOTAZIONI]

Obiettivo: creare un itinerario realistico, personalizzato e facile da seguire.

Regole:
- raggruppa le attività per zona
- considera gli spostamenti
- lascia pause realistiche
- non riempire ogni minuto
- non inventare prezzi, orari, disponibilità o link
- segnala ogni informazione da verificare
- indica quando serve una prenotazione
- proponi almeno un'alternativa in caso di pioggia
- rispetta il budget indicato
- non suggerire attività incompatibili con gli orari
- separa fatti, inferenze e ipotesi
- non presentare una raccomandazione come certezza se non è verificata

Formato:
1. sintesi del viaggio
2. assunzioni utilizzate
3. itinerario giorno per giorno
4. trasporti
5. pasti e ristoranti
6. prenotazioni
7. alternative
8. informazioni da verificare
9. rischi o criticità
10. checklist prima della partenza
```

## Sezione 31. Prompt per analizzare commenti e Creator DNA

```
Usa i commenti e i contenuti di [CREATOR/DESTINAZIONE] per identificare
problemi, desideri e opportunità di prodotto.

Materiale:
[INCOLLA COMMENTI, CAPTION, TRASCRIZIONI O NOTE]

Analizza il materiale senza inventare dati.

Separa:
- fatti verificati
- inferenze
- ipotesi
- informazioni mancanti

Identifica:
- problemi ricorrenti
- desideri
- paure
- ostacoli
- obiezioni
- richieste pratiche
- segnali di intenzione d'acquisto
- domande ripetute
- destinazioni più richieste
- esperienze più richieste
- formato di prodotto più adatto
- elementi coerenti con il Creator DNA
- elementi non coerenti con il creator

Crea un profilo sintetico con:
- pubblico
- problema principale
- trasformazione desiderata
- tono
- valori
- linguaggio
- contenuti migliori
- prodotto consigliato
- motivo per cui il creator è credibile
- rischio principale
- metodo di validazione

Non confondere engagement con intenzione d'acquisto.
Un commento positivo non dimostra automaticamente che una persona comprerebbe.

Indica il livello di evidenza per ogni conclusione: basso, medio, alto.
```

### Sezione 31.1. Analisi del prodotto

```
Analizza questa idea di prodotto:
[DESCRIZIONE DEL PRODOTTO]

Destinazione: [DESTINAZIONE]
Creator: [CREATOR]
Pubblico: [PUBBLICO]
Prezzo: [PREZZO]

Valuta:
- chiarezza della promessa
- problema risolto
- specificità del pubblico
- credibilità del creator
- differenziazione
- facilità di realizzazione
- rischio di sostituzione con strumenti gratuiti
- valore percepito
- rischio operativo
- possibilità di upsell
- possibilità di replica
- dati necessari per validare l'idea

Restituisci:
1. giudizio sintetico
2. punti forti
3. punti deboli
4. obiezioni probabili
5. modifiche consigliate
6. test di validazione
7. KPI
8. decisione: procedere, modificare o fermare
```

### Sezione 31.2. Prompt per valutare i commenti

```
Analizza i commenti seguenti relativi a [CREATOR/DESTINAZIONE].

COMMENTI:
[INCOLLA COMMENTI]

Per ogni commento individua:
- problema esplicito
- problema implicito
- desiderio
- domanda concreta
- livello di urgenza
- livello di intenzione d'acquisto
- destinazione
- periodo
- tipo di viaggiatore
- obiezione
- possibile soluzione

Non attribuire intenzioni che non sono supportate dal testo.
Se un elemento non è presente, scrivi "non specificato".

Alla fine restituisci:
- temi più frequenti
- problemi più urgenti
- richieste più facili da trasformare in prodotto
- domande da approfondire con un sondaggio
- idee di contenuto
- idee di prodotto
- informazioni ancora mancanti
```

### Sezione 31.3. Prompt per classificare i commenti

```
Classifica i commenti seguenti relativi a [CREATOR/DESTINAZIONE].

COMMENTI:
[INCOLLA COMMENTI]

Assegna una o più categorie:
- richiesta pratica
- problema o frustrazione
- desiderio
- obiezione
- domanda su prezzo o budget
- richiesta di destinazione
- richiesta su periodo o durata
- trasporto e logistica
- alloggio
- ristoranti e cibo
- famiglia o bambini
- accessibilità
- sicurezza
- confronto con altre soluzioni
- feedback positivo
- feedback negativo
- intento d'acquisto
- fuori tema

Per ogni commento restituisci:
1. commento originale
2. categoria o categorie
3. sintesi del bisogno
4. intensità del bisogno da 1 a 5
5. intento d'acquisto: alto, medio, basso o assente
6. fatti esplicitamente presenti
7. inferenze ragionevoli
8. elementi non verificabili
9. risposta o prodotto che potrebbe risolvere il bisogno

Non inventare informazioni. Se un dato non è presente, scrivi "non specificato".
Se fai un'inferenza, dichiarala come inferenza.

Alla fine raggruppa i temi più frequenti e indica:
- i 5 problemi più ricorrenti
- i 5 desideri più ricorrenti
- le obiezioni principali
- le richieste che indicano maggiore intenzione d'acquisto
- 3 idee di prodotto
- 3 idee di contenuto
- 3 domande da fare al pubblico per validare i risultati
```

## Sezione 32. Analisi del feedback

```
Usa i feedback raccolti da [PERIODO] relativi a [PRODOTTO/CREATOR].

Dati:
[INCOLLA FEEDBACK, RECENSIONI, RISPOSTE O MESSAGGI]

Classifica ogni feedback come:
- problema tecnico
- problema di chiarezza
- problema di qualità
- problema di utilità
- richiesta di nuova funzione
- obiezione
- elogio
- rischio di rimborso
- opportunità di upsell
- opportunità di referral

Restituisci una tabella con:
- feedback
- categoria
- gravità da 1 a 5
- frequenza
- impatto sull'esperienza
- azione consigliata
- priorità: urgente, alta, media o bassa

Separa sempre fatti, inferenze e ipotesi.
Non proporre modifiche basate su un solo commento isolato, salvo che si
tratti di un errore grave, di sicurezza o di privacy.

Alla fine indica:
- i tre problemi più urgenti
- le tre richieste più frequenti
- cosa correggere subito
- cosa rimandare
- cosa eliminare
- quale domanda fare agli utenti per ottenere informazioni migliori
```

## Sezione 33. Metriche del prodotto

**Monitora almeno:** visite alla landing page, provenienza del traffico, click sulla call to action, tasso di opt-in, tasso di acquisto, costo di acquisizione, completamento del questionario, tempo necessario per completare il questionario, tempo di generazione dell'itinerario, percentuale di utenti che aprono l'itinerario, percentuale che lo consultano più volte, percentuale che esportano il calendario, feedback positivo/negativo, richieste di assistenza, richieste di rimborso, referral, riacquisto, acquisto di prodotti aggiuntivi, margine per cliente, tempo operativo per consegna.

**Diagnosi:**

- Molte visite, pochi opt-in → problema nella promessa, nel titolo, nella fiducia o nella call to action.
- Molti opt-in, pochi acquisti → controllare offerta, prezzo, prova, urgenza e chiarezza.
- Molti acquisti, pochi questionari completati → onboarding troppo lungo, confuso o poco motivante.
- Questionario completato ma itinerario non aperto → controllare consegna, email, notifiche e accesso.
- Itinerari aperti ma non utilizzati → controllare qualità, formato, leggibilità e praticità.
- Molti export ma feedback negativo → verificare qualità dei dati, coerenza degli orari, semplicità del calendario.
- Molti problemi tecnici → fermare temporaneamente l'acquisizione e risolvere il prodotto prima di aumentare il traffico.

## Sezione 34. Template Creator DNA

```
Nome creator: [INSERISCI]
Handle: [INSERISCI]
Piattaforme principali: [INSERISCI]
Nazione: [INSERISCI]
Lingua: [INSERISCI]
Niche: [INSERISCI]
Destinazioni trattate: [INSERISCI]
Tipo di pubblico: [INSERISCI]
Età principale del pubblico: [INSERISCI]
Provenienza principale del pubblico: [INSERISCI]
Problemi ricorrenti: [INSERISCI]
Desideri ricorrenti: [INSERISCI]
Paure: [INSERISCI]
Obiezioni: [INSERISCI]
Domande frequenti: [INSERISCI]
Stile comunicativo: [INSERISCI]
Valori: [INSERISCI]
Parole utilizzate spesso: [INSERISCI]
Parole o temi da evitare: [INSERISCI]
Formato di contenuto: [INSERISCI]
Contenuti con maggiore engagement: [INSERISCI]
Contenuti con maggiore intenzione d'acquisto: [INSERISCI]
Prodotti già venduti: [INSERISCI]
Collaborazioni precedenti: [INSERISCI]
Esperienza reale del creator: [INSERISCI]
Possibili prodotti travel: [INSERISCI]
Elementi da evitare: [INSERISCI]
Prove a supporto: [INSERISCI]
Informazioni ancora da verificare: [INSERISCI]
```

**Regola:** non attribuire al creator esperienze, competenze, opinioni o risultati che non sono presenti nei dati raccolti.

## Sezione 35. Template configurazione prodotto

```
Nome prodotto: [INSERISCI]
Creator: [INSERISCI]
Destinazione: [INSERISCI]
Pubblico specifico: [INSERISCI]
Problema principale: [INSERISCI]
Problemi secondari: [INSERISCI]
Trasformazione promessa: [INSERISCI]
Cosa riceve il cliente: [INSERISCI]
Formato: [ITINERARIO, PDF, DASHBOARD, CALENDARIO, SUPPORTO O ALTRO]
Durata di utilizzo: [INSERISCI]
Prezzo iniziale: [INSERISCI]
Bonus: [INSERISCI]
Call to action: [INSERISCI]
Tono di voce: [INSERISCI]
Elementi distintivi: [INSERISCI]
Dati da verificare: [INSERISCI]
Responsabile degli aggiornamenti: [INSERISCI]
Frequenza degli aggiornamenti: [INSERISCI]
Politica di assistenza: [INSERISCI]
Politica di rimborso: [INSERISCI]
Proprietà degli asset: [INSERISCI]
Percentuale creator: [INSERISCI]
Percentuale operatore: [INSERISCI]
Costi deducibili: [INSERISCI]
```

La promessa deve essere specifica e realistica. Non vendere "il viaggio perfetto". Vendi un risultato concreto, per esempio: "Ricevi un itinerario personalizzato di cinque giorni a Roma, organizzato in base al tuo budget, ai tuoi interessi e al ritmo che preferisci".

## Sezione 36. Aspetti tecnici e operativi

**Il prodotto deve essere organizzato in componenti separati:** interfaccia utente, questionario, motore di pianificazione, database delle destinazioni, controllo delle fonti, generazione AI, controllo qualità, esportazione calendario, sistema di feedback, analytics, supporto.

Separare il core engine dai dati specifici della destinazione. Il core engine deve poter funzionare con Roma, Milano, Firenze, Venezia, Napoli, Sicilia, Toscana, Puglia, Dolomiti, altre destinazioni.

**Quando viene aggiunta una nuova destinazione, non duplicare tutto il codice. Aggiungere invece:** nuove informazioni, nuove regole, nuove categorie, nuove fonti, nuovi esempi, nuovi vincoli, nuove raccomandazioni.

**Ogni modifica importante deve avere:** numero di versione, data, descrizione, motivo, responsabile, risultato del test, eventuali problemi conosciuti.

## Sezione 37. Privacy e sicurezza

Raccogliere soltanto i dati necessari a creare il prodotto.

**Prima della raccolta, chiarire:** quali dati vengono raccolti, perché vengono raccolti, chi può accedervi, quanto tempo vengono conservati, come possono essere cancellati, se vengono utilizzati per analisi, se vengono condivisi con il creator, se vengono inviati a fornitori tecnici, come l'utente può chiedere assistenza.

Non utilizzare dati personali per uno scopo diverso da quello comunicato. Limitare gli accessi in base al ruolo. Usare password sicure e autenticazione a più fattori dove possibile.

**Non condividere pubblicamente:** nomi completi, email, numeri di telefono, documenti, dati di pagamento, itinerari individuali, informazioni sensibili, screenshot non anonimizzati.

Per temi legali, privacy e GDPR, rivolgersi a un professionista qualificato.

## Sezione 38. Supporto e rimborsi

Il cliente deve sapere come chiedere assistenza.

**Definire:** canale di supporto, orari di risposta, tempi stimati, problemi coperti, problemi non coperti, procedura di correzione, procedura di rimborso, responsabile del supporto.

**Distinguere tra:** errore tecnico, errore dell'itinerario, modifica richiesta dal cliente, informazione cambiata dopo la consegna, richiesta fuori dal perimetro, insoddisfazione soggettiva, problema causato da una prenotazione esterna.

Non promettere rimborsi o risultati non previsti dai termini dell'offerta. Gestire ogni richiesta in modo chiaro, documentato e coerente con le condizioni pubblicate.

## Sezione 39. Cosa non fare

Non:

- costruire funzioni soltanto perché sembrano interessanti
- copiare un creator senza capire il suo pubblico
- usare follower come unica metrica
- assumere che i commenti positivi equivalgano a vendite
- inventare dati turistici
- presentare prezzi non verificati come definitivi
- usare link non controllati
- promettere disponibilità
- ignorare tempi di spostamento
- creare giornate impossibili
- raccogliere dati personali inutili
- inserire chiavi API nel frontend
- lanciare con un prodotto non testato
- automatizzare un processo che non è ancora compreso
- espandere a molte destinazioni prima della validazione
- accettare accordi vaghi con un creator
- lasciare indefinita la proprietà degli asset
- ignorare richieste di rimborso
- nascondere errori
- continuare a vendere durante un incidente grave

## Sezione 40. Rischi principali

| # | Rischio | Prevenzione |
|---|---|---|
| 1 | Dati obsoleti | Fonti, data di verifica, avvertenze e controlli periodici |
| 2 | Allucinazioni dell'AI | Fonti controllate, istruzioni anti-invenzione, revisione umana, separazione fatti/ipotesi |
| 3 | Itinerari irrealistici | Calcolo degli spostamenti, pause, orari, test con utenti reali |
| 4 | Bassa disponibilità del creator | Calendario e responsabilità scritte |
| 5 | Bassa intenzione d'acquisto | Vendita o pre-ordine prima dello sviluppo avanzato |
| 6 | Dipendenza da una singola piattaforma | Raccolta email, proprietà dei dati, canali alternativi |
| 7 | Costi API troppo alti | Limiti di utilizzo, caching, monitoraggio, controlli sul numero di generazioni |
| 8 | Reclami o rimborsi | Promessa precisa, condizioni chiare, supporto, controllo qualità |
| 9 | Problemi di privacy | Minimizzazione dei dati, accessi limitati, informativa, procedure di cancellazione |
| 10 | Impossibilità di replicare | Template, documentazione, core engine separato, procedure standard |

## Sezione 41. Piano di incidente

**P0 — incidente critico.** Esempi: perdita di dati, violazione della privacy, pagamento errato, accesso non autorizzato, itinerario potenzialmente pericoloso, informazione gravemente falsa con conseguenze rilevanti, esposizione di una chiave API.

*Rilevazione:* segnalazione del cliente, alert tecnico, controllo interno, monitoraggio di accessi anomali, errore nei log.

*Azione immediata:*
1. bloccare la funzione coinvolta
2. impedire nuove consegne difettose
3. conservare log e prove
4. informare il responsabile
5. valutare gli utenti coinvolti
6. rimuovere o correggere l'output
7. proteggere gli account
8. informare gli utenti quando necessario
9. documentare ogni passaggio
10. valutare assistenza legale o tecnica qualificata

*Comunicazione al cliente:* descrivere il problema senza nasconderlo, spiegare cosa è stato fatto, indicare cosa deve fare il cliente, non inventare tempi di risoluzione, fornire un aggiornamento quando esistono informazioni confermate.

**P1 — incidente grave.** Esempi: link rotti in molti itinerari, export `.ics` non funzionante, destinazioni o orari obsoleti, servizio inutilizzabile per una parte significativa degli utenti, generazione sistematica di itinerari incoerenti, problemi di pagamento per più clienti.

*Azione:* riprodurre il problema; stimare il numero di utenti coinvolti; sospendere la funzione se necessario; pubblicare una comunicazione chiara; offrire una soluzione temporanea; correggere il problema; verificare la correzione; controllare gli output già consegnati; aggiornare la documentazione.

**P2 — incidente limitato.** Esempi: errore in un singolo itinerario, problema di formattazione, contenuto poco chiaro, funzione secondaria non disponibile, link errato in una singola consegna.

*Azione:* registrare il problema; rispondere all'utente; correggere manualmente se necessario; aggiungere alla lista di sviluppo; verificare se si ripete; aggiornare il controllo qualità.

**P3 — problema minore.** Esempi: refuso, miglioramento estetico, testo poco fluido, richiesta non urgente, piccola modifica all'interfaccia.

*Azione:* registrare; raggruppare con problemi simili; risolvere durante il normale ciclo di aggiornamento.

**Regola generale:** prima si proteggono utenti, dati e fiducia. Solo dopo si pensa alla velocità di crescita.

## Sezione 42. Checklist pre-lancio

**Prodotto:** la promessa è comprensibile in una frase; la destinazione è specifica; il pubblico è specifico; il questionario è stato testato; il risultato è leggibile; il risultato sembra realmente personalizzato; gli itinerari sono realistici; gli spostamenti sono considerati; esistono alternative in caso di pioggia; i dati dinamici sono marcati come da verificare; non ci sono informazioni inventate; non ci sono link rotti; l'export `.ics` è stato testato; il prodotto funziona con input incompleti; esiste una procedura per correggere gli errori.

**Business:** prezzo definito; offerta definita; call to action funzionante; termini chiari; politica di rimborso definita; canale di supporto attivo; responsabilità definite; proprietà degli asset definita; revenue share definita; creator approva il prodotto; creator conosce calendario e responsabilità.

**Tecnologia:** chiavi API protette; errori gestiti; costi monitorati; dati sensibili non salvati nel browser; backup definito; accessi limitati; analytics attivi; test eseguiti su browser e mobile.

## Sezione 43. Checklist post-lancio

**Dopo ogni vendita:** verificare il completamento dell'onboarding; controllare che l'utente abbia ricevuto il prodotto; verificare l'apertura dell'itinerario; controllare l'export del calendario; raccogliere feedback entro 24-72 ore; classificare eventuali problemi; registrare richieste ripetute; controllare rimborsi; controllare il tempo operativo; aggiornare la lista delle priorità; inviare al creator un riepilogo settimanale.

**Ogni settimana:** analizzare KPI; leggere i nuovi commenti; controllare dati e link principali; verificare costi tecnici; rivedere i problemi aperti; identificare un solo miglioramento prioritario; aggiornare il changelog.

**Ogni mese:** controllare conversione; verificare margine; valutare qualità dei creator; decidere se continuare, modificare o fermare; aggiornare la base dati; rivedere la promessa; controllare il livello di soddisfazione.

## Sezione 44. Dashboard KPI

**La dashboard deve contenere:** periodo, creator, destinazione, visite, lead, acquisti, fatturato, rimborsi, conversione, tempo medio di consegna, costo medio per cliente, margine, feedback positivo, feedback negativo, problemi tecnici, export calendario, referral, note operative.

**Per ogni KPI indicare:** valore attuale, valore del periodo precedente, obiettivo, variazione, interpretazione, azione successiva.

Non aggiungere metriche che nessuno usa per prendere decisioni. Una metrica è utile solo se modifica il comportamento del team.

## Sezione 45. Decision tree go/no-go

- **Il pubblico non risponde** → controllare il creator, il problema, il messaggio; parlare con utenti reali; non costruire altre funzioni.
- **Il pubblico risponde ma non lascia il contatto** → modificare la call to action, ridurre il rischio, rendere più chiaro il risultato, mostrare un esempio.
- **Lascia il contatto ma non acquista** → controllare prezzo, fiducia, prova, urgenza; parlare con chi ha abbandonato.
- **Acquista ma non completa il questionario** → ridurre le domande, dividere il questionario in passaggi, spiegare perché ogni informazione serve, aggiungere un salvataggio temporaneo.
- **Completa il questionario ma l'itinerario è debole** → controllare input, regole, dati destinazione; introdurre revisione umana; eliminare promesse eccessive.
- **L'itinerario è buono ma non viene usato** → migliorare formato, aggiungere istruzioni, rendere il piano più pratico, controllare la lunghezza, chiedere cosa manca.
- **Il creator non pubblica** → chiarire aspettative, creare un calendario, assegnare responsabilità, stabilire una scadenza, interrompere il pilot se non c'è collaborazione reale.
- **Il prodotto funziona con un creator** → documentare il processo, separare core engine e layer creator, replicare con una destinazione simile, testare un secondo creator, non espandersi troppo velocemente.
- **Dopo il pilot non ci sono vendite, utilizzo o feedback utile** → cambiare promessa, pubblico, creator o destinazione, oppure fermare il progetto.

## Sezione 46. Roadmap finale

| Fase | Deliverable | Criterio di completamento |
|---|---|---|
| 1. Chiarezza | Problema, pubblico, destinazione, promessa, creator, ipotesi di prodotto | Una persona esterna riesce a spiegare il prodotto in una frase |
| 2. Ricerca | Creator DNA, commenti classificati, problemi, desideri, obiezioni, segnali di acquisto, fonti | Esistono segnali concreti che il pubblico ha il problema |
| 3. Demo | Questionario, generatore, esempio di itinerario, controllo qualità, landing page | Una persona reale usa il prodotto senza assistenza continua |
| 4. Pilot | Creator, pubblico, prezzo, calendario, prime consegne, feedback, KPI | Esistono dati reali di utilizzo e pagamento |
| 5. Ottimizzazione | Lista problemi, correzioni, processo standard, supporto, fact checking, sistema di aggiornamento | Il prodotto produce risultati coerenti con meno lavoro manuale |
| 6. Replica | Core engine, layer destinazione/nicchia/creator, template outreach, dashboard, onboarding standardizzato | È possibile lanciare un nuovo pilot senza ricominciare da zero |

## Sezione 47. Prompt Master di Contesto

```
Agisci come operatore strategico per un prodotto digitale travel dedicato
a viaggi in Italia.

Contesto del progetto:
- nome del progetto: [NOME]
- fondatore o operatore: [NOME]
- città di riferimento: Milano
- paese principale: Italia
- destinazioni: [DESTINAZIONI]
- creator: [NOME E HANDLE]
- piattaforma del creator: [PIATTAFORMA]
- pubblico: [DESCRIZIONE]
- lingua: [LINGUA]
- prodotto: [DESCRIZIONE]
- prezzo: [PREZZO]
- fase attuale: [FASE]
- obiettivo: [OBIETTIVO]
- dati disponibili: [DATI]
- vincoli: [VINCOLI]

Il prodotto combina:
1. un core engine per generare itinerari
2. un layer di personalizzazione per destinazione e nicchia
3. un Creator DNA layer basato sul pubblico e sul tono del creator
4. un distribution layer basato su contenuti, landing page e partnership
5. un sistema di feedback e miglioramento continuo

Il core engine deve:
- raccogliere preferenze
- creare itinerari realistici
- raggruppare le attività per zona
- considerare gli spostamenti
- rispettare budget e ritmo
- proporre alternative
- indicare dati da verificare
- evitare contraddizioni
- supportare export calendario
- registrare feedback

Il layer creator deve considerare: esperienze reali, tono, valori, parole
ricorrenti, destinazioni trattate, pubblico, domande frequenti, obiezioni,
contenuti migliori, prodotti esistenti, elementi da evitare.

Regole anti-allucinazione — non inventare mai: luoghi, ristoranti, prezzi,
orari, disponibilità, recensioni, eventi, link, dati del creator, risultati
economici. Non presentare informazioni obsolete come attuali. Non
trasformare una supposizione in un fatto. Non promettere un risultato non
dimostrato.

Se un dato non è disponibile, scrivi: "Informazione non disponibile".
Se un dato deve essere verificato, scrivi: "Da verificare prima della
pubblicazione o della partenza".
Se utilizzi un'inferenza, scrivi: "Inferenza basata sui dati disponibili".
Se proponi un'idea non ancora validata, scrivi: "Ipotesi da validare".

Separazione obbligatoria:
- Fatti: informazioni presenti direttamente nei materiali o confermate da
  una fonte.
- Inferenze: conclusioni ragionevoli ottenute collegando più fatti.
- Ipotesi: idee, previsioni o raccomandazioni che richiedono validazione.

Quando analizzi un creator, restituisci: sintesi, fatti verificati,
inferenze, ipotesi, pubblico, problemi, desideri, obiezioni, segnali di
acquisto, tono, Creator DNA, opportunità, rischi, prossima azione.

Quando analizzi commenti, restituisci: commento originale, categoria,
bisogno, intensità da 1 a 5, intento d'acquisto, destinazione, periodo,
tipo di viaggiatore, fatti, inferenze, elementi non verificabili, azione
consigliata.

Quando generi un itinerario, includi: giorno, data, zona, fascia oraria,
attività, durata stimata, spostamento, pausa, pasto, alternativa in caso
di pioggia, informazioni da verificare, prenotazioni necessarie, motivo
per cui l'attività è adatta all'utente, livello di energia richiesto.
Non riempire ogni minuto della giornata. Non suggerire attività
incompatibili con gli orari. Non trattare un itinerario come una
prenotazione.

Quando proponi un prodotto, includi: pubblico, problema, trasformazione,
meccanismo, deliverable, prezzo ipotetico, obiezioni, rischio, metodo di
validazione, KPI, criteri go/no-go.

Quando valuti il business, considera: domanda, distribuzione, credibilità,
valore percepito, facilità di realizzazione, costi, margini, assistenza,
responsabilità, privacy, possibilità di replica.

Non consigliare di costruire nuove funzioni se il problema principale è
ancora la mancanza di validazione.

Formato di output obbligatorio:
1. Sintesi
2. Fatti verificati
3. Inferenze
4. Ipotesi
5. Problemi principali
6. Opportunità
7. Rischi
8. Raccomandazione
9. Piano operativo
10. Metriche
11. Dati ancora necessari
12. Prossima azione singola più importante

Rispondi in italiano, salvo richiesta diversa. Usa un linguaggio pratico,
diretto e specifico. Evita generalità. Se mancano dati essenziali, non
inventarli: indica quali dati mancano e continua soltanto con ciò che può
essere valutato responsabilmente.
```

## Sezione 48. Checklist conclusiva

**Strategia:** il pubblico è specifico; la destinazione è specifica; il problema è reale; la promessa è chiara; la trasformazione è concreta; il creator è coerente; il prodotto ha un differenziatore.

**Ricerca:** i commenti sono stati classificati; i problemi ricorrenti sono stati identificati; i desideri sono stati identificati; le obiezioni sono state identificate; i segnali di acquisto sono separati dai semplici complimenti; le ipotesi sono state validate o marcate come ipotesi.

**Prodotto:** il questionario è breve; l'itinerario è leggibile; gli spostamenti sono realistici; le attività sono raggruppate per zona; esistono alternative; i dati da verificare sono indicati; l'export `.ics` funziona; non ci sono dati inventati.

**Tecnologia:** le chiavi API sono protette; non vengono salvati dati sensibili nel localStorage; gli errori sono gestiti; i costi sono monitorati; il sistema è testato su mobile; esiste un piano di backup; gli accessi sono controllati.

**Operatività:** il supporto è attivo; le responsabilità sono scritte; la proprietà degli asset è definita; il creator conosce il calendario; la gestione dei rimborsi è chiara; esiste un piano di aggiornamento; il controllo qualità è assegnato.

**Validazione:** esiste una landing page; è stata mostrata una demo; il pubblico ha risposto; sono state raccolte email o pre-iscrizioni; sono state effettuate vendite o pilot; il prodotto è stato usato da persone reali; il feedback è stato classificato; esiste una decisione go/no-go.

**Replica:** il core engine è separato dai layer; il processo è documentato; il Creator DNA è riutilizzabile; il database destinazioni è aggiornabile; il supporto è standardizzato; le metriche sono raccolte; il secondo pilot non richiede di ricominciare da zero.

**Regola finale:**

Non scalare un prodotto che non è ancora stato validato. Non automatizzare un processo che non è ancora compreso. Non promettere ciò che non puoi controllare. Non inventare ciò che non puoi verificare.

Costruisci il sistema in modo che ogni risultato possa essere misurato, corretto e replicato.

---

*FINE DEL MANUALE*
