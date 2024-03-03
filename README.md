# BHPC-Manager
A one stop center to control all the processes for the distribution of BHPC porducts in EU and LATAM.

FUNZIONI DA IMPLEMENTARE
- Tenere traccia dello stock di magazzino. Registrati i valori dell'ultimo inventario. Inserendo tutte le movimentazioni in entrata e in uscita si dovrebbero avere sempre aggiornate le disponibilità in stock. Questo permetterebbe all'applicativo di fornire in tempo reale informazioni al management sulle disponibilità.
- Pulsante SHIP IT. Selezionando un ordine in stato "ALL READY" l'applicativo dovrebbe dare la possibilità di schiacciare un pulsante che in automatico stampa tutti i documenti necessari
- Duplicazione di ordini. Utile per duplicare le spedizioni registrate in valuta estera che non vanno contabilizzate. Duplicarle applicando un tasso di cambio specificato dall'utente.

BHPC MANAGER 1.5

Prima versione abbastanza stabile e testabile anche da utenti terzi. Qua di seguito descriverò le funzioni funzionanti dell'applicativo.

L'applicativo si forma di 5 TAB principali che permettono di muoversi tra le principali funzioni.
CONTROL BOARD - Un centro di controllo delle spedizioni in entrata e in uscita dei prodotti BHPC
ORDER DETAILS - Un pannello dove poter prendere visiione e modificare i dettagli logistici e generici di un ordine BHPC
ORDERED PRODUCTS - Pannello dove inserire e/o visuaìlizzare i prodotti facente parte dell'ordine selezionato
WAREHOUSE(non ancora disponibile)
ADMINISTRATION - alcune semplici funzioni di amministrazione come la selezione della cartella di salvataggio dei dati

SISTEMA DI SINCRONIZZAZIONE (Ancora in fase di test, ma apparentemente funzionante)
- L'applicativo excel è studiato per essere utilizzato come un client che si connette a un "database server" per lavorare i dati. Questo approccio è molto utile perchè permette a più utenti contemporaneamente di utilizzare una propria copia del client e manipolare i dati su server restando sempre con dati aggiornati (anche da altri utenti)
- Dalla control board è possibile effettuare delle sincronizzazioni manuali che comprendono allo stato attuale il sync di:
  - Gli ordini, file order_data
  - I prodotti degli ordini, file sales_data
  - I clienti, tabella client_lookup
- E' stato inoltre implementato un sistema di sincronizzazione a tempo, preimpostato a 3 minuti di delay tra un aggiornamento e l'altro
- Infine ogni qual volta un utente effettua operazioni che modificano i dataset lato client le stesse modifiche vengono riportate nei files lato server in modo da renderle disponibili a tutti gli altri utenti.

CONTROL BOARD
- Permette di tenere traccia degli ordini BHPC sia in entrata che in uscita
- La tabella permette il filtraggio delle spedizioni per:
  - Cliente
  - Stato dell'ordine
- Dovrebbe permettere a chi si occupa degli ordini una maggiore consapevolezza di ciò che sta succedendo e delle cose da fare

ORDER DETAILS
- Qui è possibile inserire qualsiasi dettaglio relativo all'ordine.
- Di conseguenza è possibile anche recuperare tali informazioni in un interfaccia user friendly (modifiche alla UI della tab ORDER DETAILS sono previste nelle prossime release)
- Sono previste tutta una serie di celle NOTE che danno la possibilità all'utente di prendere appunti e legarli all'ordine in maniera tale da non dimenticare nulla.
- E' stata implementata una status bar per permettere una visione immediata dello stato dell'ordine, di ciò che stato già fatto e di cosa invece dev'essere ancora fatto prima di poter spedire.

ORDERED PRODUCTS
- In questa sezione è presente una entry form per l'inserimento delle referenze ordinate dai clienti o quelle ricevute dal fornitore.
- E' stata studiata per essere il più user friendly possibile e allo stesso tempo considerare la possibilità di prodotti venduti a prezzo pieno, altri a prezzo scontato e ancora altri gratuiti (FOC)
- E' possibile che in futuro vengano implementati miglioramenti ulteriori per rendere l'inserimento di nuove spedizioni ancora più immediato.
