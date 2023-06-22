.. _linux-1:

Linux
=====

Per installare il Software CIE è necessario disporre di credenziali
linux che possano copiare files all’interno delle cartelle poste sotto
la cartella /usr/local. È necessario effettuare il download dell’ultima
versione del Software dal Portale CIE,
`www.cartaidentita.interno.gov.it <http://www.cartaidentita.interno.gov.it>`__,
sezione “Servizi”, sottosezione “Software CIE” oppure dal sito
developers.italia.it, sezione “CIE” nel caso in cui si sia interessati
alle ultime versioni “beta” del software o al codice sorgente.

Terminato il download del pacchetto la procedura di installazione si
differenzia sulla base della distribuzione Linux scelta.

Distribuzioni “Debian based”
============================

Nel caso di distribuzioni “Debian based” (ad es. Ubuntu Linux), occorre
scaricare il file cie-Software_<VERSIONE>.deb (es.
cie-Software_1.1h_amd64.deb).

Effettuato il download, occorre aprire un terminale e digitare il
seguente comando, dopo essersi posizionati nella directory dove è stato
scaricato il pacchetto di installazione:

*sudo dpkg -i <NOME_FILE>.deb*

Verrà richiesto di inserire la password di root. Inserita la password e
premuto Invio, partirà la procedura di installazione che copierà i
seguenti files:

1. Cartella “CIEID” nel percorso /usr/share/

2. File “libcie-pkcs11.so” nel percorso /usr/local/lib/

3. File “CIE_ID”.desktop nel percorso /usr/share/applications/

Al termine comparirà l’icona di CIEID nella barra dei collegamenti
veloci, come mostrato nella schermata di seguito (che fa riferimento ad
una distribuzione “Ubuntu”).

|Immagine che contiene elettronico Descrizione generata automaticamente|

Figura 11 Software CIE su distribuzioni "Debian based"

Distribuzioni “Red Hat based”
=============================

Nel caso di distribuzioni “Red Hat based” (ad es. Fedora Linux), occorre
scaricare il file cie-Software_<VERSIONE>.rpm (es.
cie-Software_1.1h_x86_64.rpm).

Effettuato il download, occorre aprire un terminale e digitare il
seguente comando, dopo essersi posizionati nella directory dove è stato
scaricato il pacchetto di installazione:

*sudo rpm -i <NOME_FILE>.rpm*

Verrà richiesto di inserire la password di root. Inserita la password e
premuto Invio, partirà la procedura di installazione che copierà i
seguenti files:

1. Cartella “CIEID” nel percorso /usr/share/

2. File “libcie-pkcs11.so” nel percorso /usr/local/lib/

3. File “CIE_ID”.desktop nel percorso /usr/share/applications/

Al termine comparirà l’icona di CIEID nella barra dei collegamenti
veloci, come mostrato nella schermata di seguito (che fa riferimento ad
una distribuzione “Fedora”).

|Immagine che contiene elettronico, monitor, cielo, interni Descrizione
generata automaticamente|

Figura 12 Software CIE su distribuzioni "Red Hat based"

Altre distribuzioni 
====================

Nel caso di altre distribuzioni occorre scaricare il file
cie-Software_<VERSIONE>.zip (es. cie-Software_1.1h_x86_64.tar.gz).

Effettuato il download, occorre aprire un terminale e digitare il
seguente comando, dopo essersi posizionati nella directory dove è stato
scaricato il pacchetto di installazione:

*tar xvzf <NOME_FILE>.tar.gz*

Completata l’estrazione dell’archivio occorrerà copiare i files
costituenti il Software nelle seguenti cartelle:

1. Cartella “CIEID” nel percorso /usr/share/

2. File “libcie-pkcs11.so” nel percorso /usr/local/lib/

3. File “CIE_ID”.desktop nel percorso /usr/share/applications/

Digitare pertanto i seguenti comandi:

1. *sudo cp -rp CIEID /usr/share/.*

2. *sudo cp -rp libcie-pkcs11.so /usr/local/lib/.*

3. *sudo cp -rp CIE_ID.desktop /usr/share/applications/.*

avendo cura di confermare con INVIO e di fornire quando richiesto la
password di root.

Se si intende utilizzare il Software all’interno di applicazioni terze
diverse dal browser, è necessario, prima di avviare l’applicazione,
procedere alla corretta impostazione della variabile d’ambiente
LD_LIBRARY_PATH, utilizzando questo comando.

*export LD_LIBRARY_PATH=/usr/local/lib*

seguito da INVIO.