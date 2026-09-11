# Travel Brief Generator

Generatore di brief di viaggio: un questionario guidato raccoglie destinazione, date, budget e preferenze, e produce un brief testuale pronto da dare a un'AI (Claude, ChatGPT, Gemini...) per generare una dashboard di viaggio personalizzata (itinerario, budget, packing list, info pratiche).

Il repository contiene anche la landing page e il flusso di accesso alla beta:

- **`index.html`** — landing page pubblica del prodotto
- **`richiesta-accesso.html`** — form (Netlify Forms) per richiedere l'accesso alla beta, con segmentazione per tipo di viaggiatore
- **`grazie.html`** — conferma post-richiesta, con link al prodotto
- **`app/generatore-viaggio.html`** — il prodotto: questionario e generazione del brief
- **`feedback.html`** — form di feedback post-uso per i tester
- **`grazie-feedback.html`** — conferma post-feedback
- **`netlify.toml`** — configurazione di deploy e redirect (`/app` → `app/generatore-viaggio.html`)

Nessun framework, nessun backend custom: solo HTML/CSS/JS vanilla lato client, form gestiti da Netlify Forms.

## Uso in locale

Sono pagine statiche: basta aprirle direttamente nel browser, oppure servirle con un server locale qualsiasi, ad esempio:

```bash
npx serve .
```

Per testare anche i redirect di `netlify.toml` e il rilevamento dei form Netlify, usare il Netlify CLI:

```bash
npx netlify-cli dev
```

## Versione live

**https://yourtripbrief.netlify.app**

- Landing: `/`
- Richiesta accesso: `/richiesta-accesso.html`
- Prodotto: `/app/`
- Feedback: `/feedback.html`

<!-- deploy automatico verificato -->
