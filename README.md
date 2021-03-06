# Progetto-L19

## Suddivisione ruoli
* _Documentazione dei requisiti_: Andrea Secchi <br>
* _Documentazione del progetto_: Luca Goretti <br>
* _Documentazione del codice_: Davide Previte <br>
* _Verifica e convalida_: Giulio Lunghi <br>
* _Qualità del codice_: Mauro Finiguerra <br>
* _Progettazione dell’interfaccia_: Alessandro Zuccolo <br>

## Requirements
 * Ambiente di sviluppo Java
 * MySQL Workbench
 * Java JDK versione 12.0.1
 * mysql-connector-java-8.0.16

## Come avviare il programma
 Per avviare il programma è necessario prima di tutto avere il database a disposizione e funzionante.
 Per evitare di dover modificare parametri all'interno del codice creare il db tramite la workbench con gli stessi parametri
 presenti all'interno della classe "ServizioDAO" del progetto UfficioPubblicoVF. Creare quindi un nuovo schema in localhost
 e chiamarlo "ufficiopubblico-data"; la tabella utilizzata dal programma si chiama "listaservizi".
 Per creare la tabella e inserire i record necessari al programma utilizzare il codice MySQL contenuto nel file "Cod-MySQL-DB.txt".
 
 ***************************************************************************************************************************************
 Parte di codice della classe ServizioDAO con i dati generali per la connessione al db:
 
 private String nomeTabella = "listaservizi"; <br>
 private String host = "jdbc:mysql://localhost:3306/ufficiopubblico-data?useTimezone=true&serverTimezone=UTC"; <br>
 private String user = ""; // username della propria workbench <br>
 private String password = ""; // password della propria workbench <br>
 ***************************************************************************************************************************************
 
 Una volta che si è in possesso di tutti i requisiti del sistema è possibile avviare il programma.
 Può essere eseguito su uno stesso dispositivo o su più dispositivi.
 1) Aprire il progetto UfficioPubblicoVF, mandare in esecuzione tramite la classe "StartApplication" e premere sul pulsante
    "AVVIA SERVER" per avviare il sistema principale di gestione dell'ufficio postale.
 2) Aprire il progetto ClientUfficioVF, nella classe "StartApplication" inserire nella variabile "host" l'indirizzo IP della
    macchina su cui gira UfficioPubblicoVF e mandare in esecuzione il programma.
 3) Aprire il progetto ClientSportelloVF, nella classe "StartApplication" inserire nella variabile "host" l'indirizzo IP della
    macchina su cui gira UfficioPubblicoVF e mandare in esecuzione il programma.
 4) Aprire il progetto ClientUtenteVF, nella classe "StartApplication" inserire nella variabile "host" l'indirizzo IP della
    macchina su cui gira UfficioPubblicoVF e mandare in esecuzione il programma.
