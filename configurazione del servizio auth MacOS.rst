.. _macos-3:

MacOS
=====

Di seguito le procedure per la configurazione del servizio di
autenticazione su MacOS

Safari e Chrome
===============

L’autenticazione tramite CIE su Safari e Chrome non richiede alcuna
operazione di configurazione aggiuntiva a quanto descritto nei paragrafi
precedenti.

Appoggiare la CIE sul lettore smart card e digitare l’indirizzo del
servizio a cui si vuole accedere nella barra degli indirizzi del
browser. Nel caso si sia già effettuata la procedura di primo utilizzo
della CIE o dopo averla in ogni caso completata, verrà richiesto quale
certificato utilizzare per l’autenticazione. Selezionare il certificato
CIE, riconoscibile dal codice fiscale del titolare, e premere OK.

|Immagine che contiene testo, schermata, software, schermo Descrizione
generata automaticamente|

Figura 35. Selezione del certificato

Su Chrome la finestra di selezione del certificato è la seguente:

|Immagine che contiene testo, schermata, schermo, software Descrizione
generata automaticamente|

Figura 36. Conferma del certificato

Confermato il certificato da utilizzare, verrà richiesto di immettere il
PIN della CIE.

Su Safari:

|Immagine che contiene testo, schermata, schermo, software Descrizione
generata automaticamente|

Figura 37. Immissione PIN su Safari

Su Chrome:

|Immagine che contiene testo, schermata, schermo, software Descrizione
generata automaticamente|

Figura 38. Immissione PIN su Chrome

Digitare le ultime 4 cifre del PIN, premere su OK e attendere qualche
secondo (la finestra di richiesta PIN non scompare immediatamente).
L’applicazione dovrebbe riconoscere correttamente l’utente e consentire
l’accesso al servizio.

Nel caso in cui venga inserito un PIN errato viene mostrata nuovamente
la finestra di inserimento PIN.

Se il PIN viene digitato in modo errato per 3 volte consecutive
quest’ultimo viene bloccato per sicurezza. Per sbloccarlo sarà
necessario lanciare l’app “Sblocca PIN” nella cartella “Applicazioni”.

Consultare il paragrafo §9.3 Sblocco per ulteriori dettagli in merito
alla procedura di sblocco PIN.

Firefox per MacOS
=================

Per utilizzare la CIE con il browser Firefox è necessario apportare a
quest’ultimo una configurazione diversa, attenendosi ai passi
sottostanti.

Accedere alla sezione “Preferenze” del browser:

|Immagine che contiene testo, schermata, numero, Carattere Descrizione
generata automaticamente|

Figura 39. Preferenze Firefox

Selezionare la scheda “Privacy e Sicurezza”

|Immagine che contiene testo, elettronica, schermata, software
Descrizione generata automaticamente|

Figura 40. Preferenze Firefox

Cliccare su “Dispositivi di sicurezza”.

|Immagine che contiene testo, software, Icona del computer, Software
multimediale Descrizione generata automaticamente|

Figura 41. Dispositivi di sicurezza Firefox

Cliccare su “Carica” e inserire le seguenti informazioni:

-  Nome modulo: software CIE

-  Nome file modulo: /Library/ipzs/libcie-pkcs11.dylib

|Immagine che contiene testo, schermata, software, Carattere Descrizione
generata automaticamente|

Figura 42. Configurazione Software CIE su Firefox

Se è la prima volta che si utilizza la CIE, sarà necessario completare
preventivamente la procedura di prima registrazione riportata nel
paragrafo §5. Se tutto va a buon fine, il modulo comparirà nella lista
di sinistra, con l’elenco dei lettori di smart card installati sul
computer:

|Immagine che contiene testo, software, schermata Descrizione generata
automaticamente|

Figura 43. Dispositivo di sicurezza CIE su Firefox

Appoggiando la CIE sul lettore questa verrà riconosciuta dal browser e
verranno visualizzate delle informazioni.

|Immagine che contiene testo, software, Icona del computer, Pagina Web
Descrizione generata automaticamente|

Figura 44. Accesso al dispositivo di sicurezza Firefox

Per verificare la corretta installazione tornare alla scheda “Avanzate”,
e, lasciando la CIE appoggiata sul lettore, cliccare su “Certificati”.
Verrà richiesto il PIN della CIE. Digitare le ultime 4 cifre del PIN e
premere su OK.

|Immagine che contiene testo, schermata, Carattere, numero Descrizione
generata automaticamente|

Figura 45. Immissione del PIN su Firefox

Nella scheda “Certificati Personali” comparirà il certificato di
autenticazione dell’utente, riconoscibile dal codice fiscale.

|Immagine che contiene testo, schermata, software, schermo Descrizione
generata automaticamente|

Figura 46. Certificato CIE utente su Firefox

La configurazione a questo punto è stata eseguita correttamente.
All’avvio successivo di Firefox non sarà necessario ripetere questa
operazione.

Per utilizzare la CIE nell’accesso ad un servizio erogato da una
Pubblica Amministrazione, appoggiare la carta sul lettore smart card e
digitare l’indirizzo del servizio a cui si vuole accedere nella barra
degli indirizzi del browser Firefox.

All’avvio della connessione verrà richiesto il PIN della CIE. Inserire
le ultime 4 cifre del PIN.

|Immagine che contiene testo, schermata, palla, software Descrizione
generata automaticamente|

Figura 47. Accesso ad un servizio, immissione del PIN

Verrà poi richiesto di selezionare il certificato da utilizzare per
l’autenticazione client. Selezionare il certificato CIE, riconoscibile
dal codice fiscale del titolare, e premere OK.

|Immagine che contiene testo, elettronica, schermata, schermo
Descrizione generata automaticamente|

Figura 48. Conferma del certificato

L’applicazione dovrebbe riconoscere correttamente l’utente e consentire
l’accesso al servizio desiderato.

Attenzione: nel caso in cui venga inserito un PIN errato o il PIN sia
bloccato, Firefox non restituisce alcun messaggio d’errore all’utente,
ma ripropone la finestra di inserimento PIN. Verificare accuratamente il
PIN inserito per evitare il blocco accidentale della CIE.

Consultare il paragrafo §9.3 Sblocco per ulteriori dettagli in merito
alla procedura di sblocco PIN.