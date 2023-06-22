.. _windows-3:

Windows
=======

Di seguito le procedure per la configurazione del servizio di
autenticazione su Windows

MS Internet Explorer, MS Edge, Chrome e Opera
=============================================

L’autenticazione tramite CIE su Internet Explorer (fino alla versione 11
e Edge), su Chrome e su Opera non richiede alcuna operazione di
configurazione aggiuntiva a quanto descritto nei paragrafi precedenti.

Appoggiare la CIE sul lettore smart card e digitare l’indirizzo del
servizio a cui si vuole accedere nella barra degli indirizzi del
browser. Se è la prima volta che si procede all’utilizzo della CIE con
il browser, verrà avviata la procedura descritta nel paragrafo §5. Nel
caso si sia già effettuata la procedura di primo utilizzo della CIE o
dopo averla in ogni caso completata, verrà richiesto quale certificato
utilizzare per l’autenticazione. Selezionare il certificato CIE,
riconoscibile dal codice fiscale del titolare, e premere OK.

|C:\Users\f.ottavi\AppData\Local\Microsoft\Windows\INetCache\Content.Word\cert.png|

Figura 19. Accesso ai servizi in rete, selezione del certificato

Su Chrome e Opera la finestra di selezione del certificato è la
seguente:

|Immagine che contiene testo, elettronica, schermata, schermo
Descrizione generata automaticamente|

Figura 20. Accesso ai servizi in rete, conferma del certificato

Confermato il certificato da utilizzare, verrà richiesto di immettere il
PIN della CIE.

|C:\Users\f.ottavi\AppData\Local\Microsoft\Windows\INetCache\Content.Word\PIN.PNG|

Figura 21. Immissione delle ultime quattro cifre del PIN

Digitare le ultime 4 cifre del PIN, premere su OK e attendere qualche
secondo (la finestra di richiesta PIN non scompare immediatamente).
L’applicazione dovrebbe riconoscere correttamente l’utente e consentire
l’accesso al servizio.

Nel caso in cui venga inserito un PIN errato viene visualizzata una
finestra di errore in cui è specificato il numero rimanente di tentativi
di inserimento PIN primo del blocco:

|Immagine che contiene testo, schermata, schermo, Carattere Descrizione
generata automaticamente|

Figura 22. Nel caso in cui il PIN immesso non sia corretto

Se il PIN viene digitato in modo errato per 3 volte consecutive
quest’ultimo viene bloccato per sicurezza.

|Immagine che contiene testo, schermata, schermo, Carattere Descrizione
generata automaticamente|

Figura 23. CIE bloccata.

In tal caso, è possibile procedere al suo sblocco utilizzando il PUK e
cliccando sull’avviso che compare nell’area di notifica in basso a
destra.

|Immagine che contiene testo, schermata, Carattere, software Descrizione
generata automaticamente|

Figura 24. Notifica per sblocco della CIE

Consultare il paragrafo §9.3 Sblocco per ulteriori dettagli in merito
alla procedura di sblocco PIN.

Firefox per Windows
===================

Per utilizzare la CIE su Windows con il browser Firefox, nel caso in cui
la versione di quest’ultimo sia inferiore o uguale alla v.90.x è
necessario apportare a quest’ultimo una configurazione aggiuntiva,
attenendosi ai passi sottostanti.

Tale configurazione **non è necessaria** con versioni successive alla
v.90.

Accedere alla sezione “Opzioni” del browser:

|Immagine che contiene testo, schermata, schermo, software Descrizione
generata automaticamente|

Figura 25. Configurazione di Firefox

Selezionare la scheda “Avanzate”, quindi la scheda “Certificati”

|Immagine che contiene testo, schermata, software, Icona del computer
Descrizione generata automaticamente|

Figura 26. Configurazione di Firefox

Cliccare su “Dispositivi di sicurezza”.

|Immagine che contiene testo, software, Icona del computer, Software
multimediale Descrizione generata automaticamente|

Figura 27. Aggiunta di un nuovo dispositivo di sicurezza su Firefox

Cliccare su “Carica” e inserire le seguenti informazioni:

-  Nome modulo: Software CIE

-  Nome file modulo: C:\Windows\System32\CIEPKI.dll

|Immagine che contiene testo, schermata, schermo, software Descrizione
generata automaticamente|

Figura 28. Configurazione di un dispositivo di sicurezza su Firefox.

Se è la prima volta che si utilizza la CIE, verrà richiesto di
completare la procedura di prima registrazione riportata nel paragrafo
§5. Se tutto va a buon fine, il modulo comparirà nella lista di
sinistra, con l’elenco dei lettori di smart card installati sul
computer:

|Immagine che contiene testo, software, schermata Descrizione generata
automaticamente|

Figura 29. Configurazione di un dispositivo di sicurezza su Firefox

Appoggiando la CIE sul lettore questa verrà riconosciuta dal browser e
verranno visualizzate delle informazioni.

|Immagine che contiene testo, software, Icona del computer, Pagina Web
Descrizione generata automaticamente|

Figura 30. Configurazione di un dispositivo di sicurezza su Firefox

Per verificare la corretta installazione tornare alla scheda “Avanzate”,
e, lasciando la CIE appoggiata sul lettore, cliccare su “Certificati”.
Verrà richiesto il PIN della CIE. Digitare le ultime 4 cifre del PIN e
premere su OK.

|Immagine che contiene testo, schermata, Carattere, numero Descrizione
generata automaticamente|

Figura 31. Accesso al dispositivo di sicurezza configurato su Firefox

Nella scheda “Certificati Personali” comparirà il certificato di
autenticazione dell’utente, riconoscibile dal codice fiscale.

|Immagine che contiene testo, schermata, software, schermo Descrizione
generata automaticamente|

Figura 32. Accesso al dispositivo di sicurezza configurato su Firefox

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

Figura 33. Accesso ad un servizio in rete con la CIE da Firefox

Verrà poi richiesto quale certificato utilizzare per l’autenticazione
client. Selezionare il certificato CIE, riconoscibile dal codice fiscale
del titolare, e premere OK.

|Immagine che contiene testo, elettronica, schermata, schermo
Descrizione generata automaticamente|

Figura 34. Accesso ad un servizio in rete da Firefox, selezione del
certificato

L’applicazione dovrebbe riconoscere correttamente l’utente e consentire
l’accesso al servizio desiderato.

Attenzione: nel caso in cui venga inserito un PIN errato o il PIN sia
bloccato, Firefox non restituisce alcun messaggio d’errore all’utente,
ma ripropone la finestra di inserimento PIN. Verificare accuratamente il
PIN inserito per evitare il blocco accidentale della CIE.

Consultare il paragrafo §9.3 Sblocco per ulteriori dettagli in merito
alla procedura di sblocco PIN.