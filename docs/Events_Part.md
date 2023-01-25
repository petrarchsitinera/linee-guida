# Events Part

**Events Part** permette di inserire e descrivere singolarmente:   
* gli eventi biografici relativi alle persone;
* gli eventi relativi alla storia dei manoscritti;
* gli invii, le ricezioni e le consegne dei testi di corrispondenza schedati.

La descrizione analitica e il ricorso a tassonomie predefinite, che permettono l'indicizzazione automatica dei dati e la loro esportazione in più formati, richiedono la **massima attenzione** durante la compilazione, al fine di evitare errori a cascata.  

La descrizione del modello è disponibile su [[Github|https://github.com/vedph/cadmus-general#historicaleventspart]].   

Per aggiungere **Events Part**, selezionare **events** dal menu a tendina, quindi cliccare sul tasto **add part**.

## Event
Per ogni evento è creato un elemento _event_ mediante un [editor](Editor_Brick.md).  
La schermata principale permette di fornire le informazioni fondamentali sull'evento.  
La schermata _related_, cui si può accedere attraverso il menu orizzontale in alto permette di registrare le entità (persone, testi, manoscritti, etc.) collegate all'evento schedato. 

🚧 Spiegare thesauri quindi relazioni a seconda degli item.
🚧 Spiegare impatto su grafo e quando usare grafo (forse mai!). 
🚧 Spiegare come evitare doppioni.

### Eid
È l'identificativo dell'evento da inserire. 
🚧 Spiegare come evitare doppioni: controllo con lookup.

La compilazione del campo è obbligatoria.

### Type 
Permette di indicare la tipologia di evento inserito.  
Per ulteriori chiarimenti sulle tipologie di eventi e sulle entità collegate cliccare [qui](Events_Thesaurus.md).

La compilazione del campo è obbligatoria.

### Description
**Description** è un campo a testo libero.  
Inserire una descrizione breve e concisa dell'evento.  

La compilazione del campo è obbligatoria.

### Note    
Permette di inserire, in forma di testo libero, eventuali informazioni aggiuntive non riportabili nei campi a disposizione.

### Chronotope 
Permette di indicare la data e il luogo dell'evento secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).  
La compilazione del campo è obbligatoria.  

### Assertion 
Permette di assegnare un indice di affidabilità all'evento schedato e di indicarne le fonti attraverso [Assertion](Assertion_Brick.md).


### Related Entities
In questa sezione è possibile registrare le entità (persone, testi, manoscritti, etc.) collegate all'evento schedato.  
Per ogni entità è creato un elemento _related_ mediante un [editor](Editor_Brick.md).   
Ogni _related_ deve essere salvato cliccando il tasto di spunta blu a fianco.  

🚧 Spiegare come evitare doppioni; come lookup; come agisce sul grafo questa roba

#### Relation 
Permette di indicare la tipologia della relazione tra l'entità e l'evento .  
Per ulteriori chiarimenti sulle tipologie di eventi e sulle entità collegate cliccare [qui](Events_Thesaurus.md)

#### Id
Permette di indicare, attraverso il suo identificativo [🚧 link e lookup] l'entità collegata all'evento.

## Save ⚠️ 

Per ogni elemento _event_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
