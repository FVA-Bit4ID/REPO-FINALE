.. _linux-3:

Linux
=====

Di seguito le procedure per la configurazione del servizio di
autenticazione su Linux

Accesso ad un servizio online mediante il browser Firefox e la CIE
==================================================================

La CIE può essere utilizzata per accedere ai servizi online erogati
dalle Pubbliche Amministrazioni, che accettano la modalità di
autenticazione mediante Carta di identità elettronica per il tramite
dello schema “Entra con CIE”.

La procedura di autenticazione richiede sempre l’inserimento del PIN e
richiede delle operazioni di configurazione aggiuntive, come descritto
nel seguito.

Avviare Firefox e accedere alla sezione “Preferenze” del browser:

|Immagine che contiene testo, schermata, numero, Carattere Descrizione
generata automaticamente|

Figura 49. Preferenze Firefox

Selezionare la scheda “Privacy e Sicurezza” o “Privacy & Security” nel
caso di distribuzioni in inglese.

|Immagine che contiene screenshot Descrizione generata automaticamente|

Figura 50. Dispositivi di sicurezza su Firefox

Cliccare su “Dispositivi di sicurezza” o “Security Devices”.

|Immagine che contiene testo, software, Icona del computer, Software
multimediale Descrizione generata automaticamente|

Figura 51. Dispositivi di sicurezza su Firefox

Cliccare su “Carica” e inserire le seguenti informazioni:

-  Nome modulo: CIE PKI

-  Nome file modulo: /usr/local/lib/libcie-pkcs11.so

Se è la prima volta che si utilizza la CIE, sarà necessario completare
preventivamente la procedura di abbinamento riportata nel paragrafo §5.
Se tutto va a buon fine, il modulo comparirà nella lista di sinistra,
con l’elenco dei lettori di smart card installati sul computer:

|Immagine che contiene screenshot, monitor Descrizione generata
automaticamente|

Figura 52. Dispositivi di sicurezza su Firefox

Per verificare la corretta installazione tornare alla scheda delle
preferenze e, lasciando la CIE appoggiata sul lettore, cliccare su
“Certificati” o “View Certificates”. Verrà richiesto il PIN della CIE.
Digitare le ultime 4 cifre del PIN e premere su OK.

|Immagine che contiene screenshot Descrizione generata automaticamente|

Figura 53. Caricamento del Software CIE su Firefox

Nella scheda “Certificati Personali” comparirà il certificato di
autenticazione dell’utente, riconoscibile dal codice fiscale.

|Immagine che contiene screenshot, monitor Descrizione generata
automaticamente|

Figura 54. Caricamento del Software CIE su Firefox

La configurazione a questo punto è stata eseguita correttamente.
All’avvio successivo di Firefox non sarà necessario ripetere questa
operazione.

Per utilizzare la CIE nell’accesso ad un servizio erogato da una
Pubblica Amministrazione, appoggiare la carta sul lettore smart card e
digitare l’indirizzo del servizio a cui si vuole accedere nella barra
degli indirizzi del browser Firefox.

All’avvio della connessione verrà richiesto il PIN della CIE. Inserire
le ultime 4 cifre del PIN.

|Immagine che contiene screenshot, computer, interni Descrizione
generata automaticamente|

Figura 55. Accesso ad un servizio in rete con la CIE, mediante Firefox

Con alcune versioni di Firefox potrebbe essere poi richiesto di
selezionare il certificato da utilizzare per l’autenticazione client.
Selezionare il certificato CIE, riconoscibile dal codice fiscale del
titolare, e premere OK.

|Immagine che contiene testo, elettronica, schermata, schermo
Descrizione generata automaticamente|

Figura 56. Scelta del certificato in fase di autenticazione

L’applicazione dovrebbe riconoscere correttamente l’utente e consentire
l’accesso al servizio desiderato.

Nel caso in cui venga inserito un PIN errato viene mostrata nuovamente
la finestra di inserimento PIN.

|Immagine che contiene screenshot, computer, interni Descrizione
generata automaticamente|

Figura 57. Immissione del PIN

Se il PIN viene digitato in modo errato per 3 volte consecutive
quest’ultimo viene bloccato per sicurezza. Per sbloccarlo sarà
necessario lanciare l’app “CIE ID”.

Consultare il paragrafo §9.3 Sblocco per ulteriori dettagli in merito
alla procedura di sblocco PIN.
