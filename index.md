# Privacy Policy — Reddit Consensus Pin

**Ultimo aggiornamento: 2 ottobre 2026**

La presente informativa descrive come l'estensione Chrome **"Reddit Consensus Pin - Risposte & Soluzioni Istantanee"** (di seguito "l'Estensione") raccoglie, utilizza, conserva e condivide i dati degli utenti.

---

## 1. Titolare del trattamento e contatti

| | |
|---|---|
| **Sviluppatore / Titolare del trattamento** | Carlo AgentCom |
| **Email di contatto** | `agentcom.carlo@gmail.com` |
| **Sede** | Italia |

Per qualsiasi richiesta relativa ai tuoi dati personali puoi contattare il titolare all'indirizzo indicato sopra.

---

## 2. Sintesi

L'Estensione **non ha server propri**: non esiste alcun backend dello sviluppatore che raccolga, registri o monetizzi dati. L'intero funzionamento avviene nel tuo browser.

L'Estensione **non raccoglie dati di identificazione diretta** dell'utente (nome, cognome, email, telefono, indirizzo IP, identificativi del dispositivo) e **non effettua alcun tracciamento della navigazione**.

L'Estensione legge però **contenuti pubblici appartenenti a terzi** (post e commenti di Reddit) e, **solo se l'utente lo sceglie esplicitamente**, li trasmette a un provider di intelligenza artificiale da lui selezionato. Questa è l'unica forma di condivisione verso terzi e avviene esclusivamente su iniziativa dell'utente.

---

## 3. Quali dati vengono trattati

### 3.1 Dati letti dalle pagine web (fonte: contenuto pubblico)

Quando l'utente attiva l'Estensione su una discussione di Reddit (o su un risultato di Google che rimanda a Reddit), vengono letti e trattati i seguenti elementi, **già pubblici**:

- titolo del post;
- testo del post (autore originale, fino a 1.000 caratteri);
- subreddit di appartenenza;
- nome utente Reddit dell'autore del post;
- punteggio (upvote) e numero di commenti;
- fino a 15 commenti della discussione, ordinati per punteggio, incluenti testo (fino a 500 caratteri ciascuno), nome utente Reddit dell'autore del commento e relativi upvote.

**Non vengono letti** messaggi privati, inbox, profili Reddit protetti da login, né alcun contenuto relativo a utenti che non abbiano pubblicato il proprio nome utente.

### 3.2 Dati inseriti dall'utente

- **Chiave API** (facoltativa): inserita dall'utente se sceglie di utilizzare un provider AI esterno (Groq, Google Gemini, Anthropic Claude, OpenAI). **Viene conservata esclusivamente nella memoria locale del browser del dispositivo in cui è stata inserita** (cfr. § 6 e § 7): non viene sincronizzata sull'account Google dell'utente e non viene trasferita ad altri dispositivi.
- **Preferenze di funzionamento**: provider selezionato, lingua dei riassunti, modalità di attivazione (badge/hover/klick destro), ritardo di attivazione al passaggio del mouse, stato di attivazione della cache e della modalità Google. Queste preferenze sono le uniche informazioni salvate sull'account Google dell'utente (tramite `chrome.storage.sync`) e non contengono dati identificativi.

### 3.3 Dati generati dall'Estensione

I riassunti di consenso generati dall'Estensione sono salvati localmente insieme a: identificativo del post, titolo, autore, subreddit, punteggio, numero di commenti, permalink, testo del riassunto, provider e modello utilizzati, data e ora di generazione.

---

## 4. Finalità e base giuridica

| Dato | Finalità | Base giuridica (GDPR) |
|---|---|---|
| Preferenze e impostazioni | Fornire le funzioni richieste dall'utente | Art. 6(1)(b) — esecuzione del contratto/servizio richiesto |
| Contenuti pubblici di Reddit | Generare il riassunto di consenso richiesto esplicitamente dall'utente | Art. 6(1)(b) |
| Riassunti in cache locale | Consentire l'apertura istantanea delle discussioni già elaborate, migliorando le prestazioni | Art. 6(1)(f) — legittimo interesse al funzionamento tecnico dell'Estensione |
| Trasmissione a provider AI (se attivata) | Generare la sintesi testuale tramite il provider scelto dall'utente | Art. 6(1)(b) — esecuzione del servizio richiesto |

Il trattamento noniede attività di profilazione, decisioni automatizzate che producano effetti giuridici, né finalità di marketing.

---

## 5. Condivisione con terzi

L'Estensione **non condivide dati con terzi se non nelle modalità indicate nell'apposito pannello delle impostazioni**.

### 5.1 Modalità "Smart Instant" (predefinita)

Nessun trasferimento verso terzi. La sintesi viene calcolata interamente e localmente nel browser, senza alcuna chiamata di rete verso servizi esterni.

### 5.2 Modalità AI con chiave fornita dall'utente (BYOK)

Se — e solo se — l'utente seleziona un provider AI e inserisce una propria chiave API, i dati descritti al §3.1 (titolo, subreddit, nome utente dell'autore del post, punteggio, testo del post e dei commenti selezionati) vengono **trasmessi ai seguenti destinatari**, per consentire la generazione del riassunto:

| Destinatario | Dati trasmessi | Finalità |
|---|---|---|
| **GroqCloud, Inc.** — `api.groq.com` | contenuti del thread | generazione della sintesi |
| **Google LLC (Gemini / AI Studio)** — `generativelanguage.googleapis.com` | contenuti del thread | generazione della sintesi |
| **Anthropic PBC** — `api.anthropic.com` | contenuti del thread | generazione della sintesi |
| **OpenAI, L.L.C.** — `api.openai.com` | contenuti del thread | generazione della sintesi |

La chiave API dell'utente non viene trasmessa ad alcun destinatario diverso dal provider selezionato, non viene condivisa con altri utenti e non viene utilizzata per finalità diverse dalla chiamata di inferenza richiesta.

L'utente può in qualsiasi momento annullare questo comportamento riportando la modalità su "Smart Instant" ed eliminando la chiave API dalle impostazioni.

### 5.3 Trasferimenti extra SEE

I destinatari di cui al §5.2 possono trattare i dati al di fuori dello Spazio Economico Europeo. In tal caso si applicano le garanzie contrattuali previste dalla normativa vigente (quali le Clausole Contrattuali Standard) e le policies di protezione dei dati dei rispettivi fornitori. Cliccando "Testa Connessione" l'utente può verificare in anticipo il provider effettivamente utilizzato.

### 5.4 Assenza di altri trasferimenti

Non sono presenti trasferimenti a fini pubblicitari, di profilazione, di misurazione dell'audience, né integrazioni con script di terze parti, telemetria, tracker o SDK pubblicitari.

---

## 6. Conservazione dei dati

- **Preferenze di funzionamento**: conservate sull'account Google dell'utente tramite `chrome.storage.sync` e, in copia di sicurezza, sulla memoria locale del dispositivo. Non contengono dati identificativi. L'utente può revocarne la sincronizzazione in qualsiasi momento dalle impostazioni di Chrome ("Impostazioni → passwords e dati > Controlla la sincronizzazione").
- **Chiave API**: conservata **soltanto** nella memoria locale del dispositivo in cui è stata inserita, per il tempo necessario all'utilizzo della funzione di sintesi. Non viene sincronizzata su altri dispositivi tramite l'account Google. L'utente può eliminarla definitivamente, in qualsiasi momento, con il pulsante "Elimina la chiave API da questo dispositivo" presente nelle impostazioni dell'Estensione.
- **Cache dei riassunti**: conservata esclusivamente sulla memoria locale del dispositivo (`chrome.storage.local`) per un periodo massimo di **14 giorni** dalla generazione. Scaduto tale termine, la voce viene eliminata automaticamente in modo silenzioso. L'utente può eliminare l'intera cache in qualsiasi momento con il pulsante "Svuota Cache" presente nelle impostazioni o nel popup dell'Estensione.
- **Nessun dato viene conservato sui sistemi dello sviluppatore**: lo sviluppatore non riceve, non registra e non archivia alcun dato derivante dall'uso dell'Estensione.

La rimozione dell'Estensione da Chrome determina l'eliminazione automatica di tutti i dati locali ad essa associati.

---

## 7. Come vengono protetti i dati

- Tutte le comunicazioni verso i provider AI avvengono su canali **HTTPS** con autenticazione tramite chiave.
- La chiave API è conservata esclusivamente nella memoria locale del dispositivo dell'utente; **non viene mai scritta su `chrome.storage.sync`**, non raggiunge quindi altri dispositivi tramite la sincronizzazione dell'account Google, e **non è mai incorporata nel codice dell'Estensione**. Agli altri utenti dell'Estensione non è accessibile in alcun modo.
- Nel caso di utenti che avevano installato una versione precedente dell'Estensione, all'aggiornamento la chiave API viene automaticamente trasferita dalla memoria sincronizzata alla memoria locale del dispositivo e rimossa da quella sincronizzata.
- L'Estensione non raccoglie dati di autenticazione, credenziali bancarie, dati sanitari, informazioni sensibili o dati relativi a minori.
- L'interfaccia dell'Estensione è isolata in un **Shadow DOM**, riducendo la superficie di esposizione dei dati alle pagine visitate.

---

## 8. I tuoi diritti (GDPR)

In qualunque momento puoi esercitare, per i dati trattati sotto la tua titolarità:

- **diritto di accesso** (art. 15);
- **diritto di rettifica** (art. 16);
- **diritto di cancellazione / diritto all'oblio** (art. 17);
- **diritto di limitazione del trattamento** (art. 18);
- **diritto di portabilità del dato** (art. 20);
- **diritto di revoca del consenso** (art. 7, c. 3);
- **diritto di opposizione** (art. 21).

Come esercitarli: la cancellazione e la limitazione possono essere esercitate direttamente dall'Estensione tramite i comandi "Svuota Cache" e "Elimina la chiave API da questo dispositivo". Per qualsiasi altra richiesta, scrvi a `agentcom.carlo@gmail.com`. Il titolare risponderà entro 30 giorni.

**Nota sui dati di terzi.** I contenuti di Reddit che l'Estensione legge sono dati pubblici appartenenti ai rispettivi autori e subreddit. Il titolare dell'Estensione agisce su istruzione dell'utente e non determina le finalità né i mezzi del trattamento effettuato dalla piattaforma Reddit; per richieste relative a tali contenuti è necessario rivolgersi direttamente al rispettivo titolare (Reddit, Inc.).

---

## 9. Modifiche alla presente informativa

La presente informativa può essere aggiornata per riflettere modifiche tecniche o funzionali dell'Estensione. La data di aggiornamento è indicata in testa al documento. Le modifiche sostanziali saranno evidenziate dalla revisione della data. L'utilizzo continuato dell'Estensione dopo la pubblicazione di una revisione implica l'accettazione dell'informativa aggiornata.

---

## 10. Dettagli tecnici per la revisione

Riepilogo dei permessi dichiarati nel `manifest.json` e del loro utilizzo effettivo:

| Permesso | Utilizzo reale |
|---|---|
| `storage` | salvataggio di preferenze (area sincronizzata), chiave API (solo area locale) e cache dei riassunti (solo area locale) |
| `contextMenus` | aggiunta del comando di menu contestuale "Estrai Consenso della Community" |
| `https://*.reddit.com/*` | lettura dei dati pubblici del thread selezionato |
| `https://*.redd.it/*` | risoluzione dei link brevi `redd.it` |
| `https://api.groq.com/*` | chiamate al provider AI **solo se selezionato dall'utente** |
| `https://generativelanguage.googleapis.com/*` | chiamate al provider AI **solo se selezionato dall'utente** |
| `https://api.anthropic.com/*` | chiamate al provider AI **solo se selezionato dall'utente** |
| `https://api.openai.com/*` | chiamate al provider AI **solo se selezionato dall'utente** |
| `https://*.google.com/*` | lettura dei risultati di ricerca per individuare discussioni di Reddit |

**Contenuto del pacchetto**: l'Estensione non include codice di terze parti, librerie di analytics, telemetria o codice remoto caricato a runtime.
