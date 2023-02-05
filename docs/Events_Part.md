# Events Part

**Events Part** permette di inserire e descrivere singolarmente:   
* gli eventi biografici relativi alle persone;
* gli eventi relativi alla storia dei manoscritti;
* gli invii, le ricezioni e le consegne dei testi di corrispondenza schedati.

⚠️ La descrizione analitica e il ricorso a tassonomie predefinite, che permettono l'indicizzazione automatica dei dati e la loro esportazione in più formati, richiedono la **massima attenzione** durante la compilazione, al fine di evitare errori a cascata.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#historicaleventspart).   

Per aggiungere la parte, selezionare **events** dal menu a tendina, quindi cliccare sul tasto **add part**.

## Event
Ciascun evento è inserito come elemento singolo (_event_) - cfr. la sezione [Creare, modificare, eliminare e salvare elementi](Editor_Brick.md).

La schermata principale, _general_ permette di fornire le informazioni fondamentali sull'evento (1). 

La schermata _related_, cui si accede attraverso il menu orizzontale in alto, permette di registrare le entità (persone, testi, manoscritti, etc.) collegate all'evento schedato (2). 

<img width="930" alt="Schermata 2023-02-05 alle 18 27 46" src="https://user-images.githubusercontent.com/102725489/216835381-26a94505-55f8-4fcf-8b82-51ca0871c47d.png">

⚠️⚠️⚠️ In Itinera, gli eventi che interessano più _item_, come ad esempio un incontro tra due persone schedate, vanno inseriti una sola volta. In questi casi, il compilatore deve perciò verificare sempre che l'evento non sia già stato inserito, consultando la _Events Part_ degli _item_ interessati dall'evento e il [grafo](semantic_graph.md).  

### Eid
Permette di creare un identificativo univico dell'evento.  
Per le regole di composizione degli identificativi cliccare [qui](identifiers.md).

La compilazione del campo è obbligatoria.

### Type 
Permette di indicare la tipologia di evento inserito, selezionando una voce dal _thesaurus_ eventi.  

A seconda dell'evento inserito, sarà possibile, nella schermata _related_, creare diverse tipologie di entità (persone, testi, manoscritti, etc.) collegate all'evento.  

La compilazione del campo è obbligatoria.

### Description
Permette di inserire, in forma di testo libero, una descrizione breve e concisa dell'evento.  

La compilazione del campo è obbligatoria.

### Note    
Permette di inserire, in forma di testo libero, eventuali informazioni aggiuntive che non è possibile inserire nei campi a disposizione.

### Chronotope 
Permette di indicare la data e il luogo dell'evento secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).  
La compilazione del campo è obbligatoria.  

### Assertion 
Permette di assegnare un indice di affidabilità all'evento schedato e di indicarne le fonti attraverso [Assertion](Assertion_Brick.md).  

### Related Entities
In questa sezione è possibile registrare le entità (persone, testi, manoscritti, etc.) collegate all'evento schedato.  

Ciascuna entità legata all'evento creato è inserita come elemento singolo (_related_) - cfr. la sezione [Creare, modificare, eliminare e salvare elementi](Editor_Brick.md).

Ogni elemento_related_ deve essere salvato cliccando il tasto di spunta blu a fianco.  

⚠️ Un evento (_a_) inserito in un _item_ (_item_ 1) che abbia tra i _related_ un altro _item_ (_item_ 2) non **non deve essere inserito una seconda volta** nella _events Part_ di quest'ultimo, indipendentemente dalla tipologia di _item_ 1 e 2. Una volta salvato in _item_ 1, infatti, l'evento _a_ è subito e contestulmente proiettato sul [grafo](semantic_graph.md) a collegare _item_ 1 e _item_ 2. Va tuttavia specificato che l'evento _a_ non risulta visibile nella _events Part_ di _item_ 2. 




#### Relation 
Permette di indicare la tipologia della relazione tra l'entità e l'evento .  
Per ulteriori chiarimenti sulle tipologie di eventi e sulle entità collegate cliccare [qui](Events_Thesaurus.md)

#### Id
Permette di indicare attraverso un identificativo l'entità collegata all'evento.  
Se l'entità corrisponde a un Item Person, Work o Manuscript o a una _part_, copiarne [l'_eid_](identifiers.md), servendosi eventualmente dei [repository](repository.md) e della funzione di [lookup](lookup.md).   


## Save ⚠️ 

Per ogni elemento _event_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
