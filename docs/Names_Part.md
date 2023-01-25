# Names Part

**Names Part** raccoglie il nome e le forme alternative del nome della persona schedata nell'_item person_.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#namespart).  

Per aggiungere la parte, selezionare **_names_** dal menu a tendina, quindi cliccare sul tasto **add part**.  

# Name
Per ogni nome è creato un elemento _name_ mediante un [editor](Editor_Brick.md).

È possibile aggiungere più nomi, uno per ogni forma attestate o in uso. È tuttavia **obbligatorio** inserire la forma del nome individuata come principale, e come tale dichiarata attraverso il tag: consultare il **repository dei nomi di persona**.
🚧in realtà queste raccomandazioni non servono forse più, dal momento che abbiamo scoperto che i nomi "analogici" non sono utilizzati per triple e lookup, che usano l'eid fornito in MetadataPart: ma CHIARIRE 🚧

### Language
Selezionare dal menu a tendina la lingua in cui è espresso il nome. 

La compilazione del campo è obbligatoria.

### Tag
Inserire:  
* principale: per la forma principale del nome, che deve coincidere con il nome indicato nel **repository dei nomi di persona**.
* alternativo: per tutte le altre forme del nome.

La compilazione del campo è obbligatoria. (🚧ma vedi sopra)

### Piece
Cliccando _+add piece_ è possibile inserire le componenti del nome: nome, cognome o nome generico.  
In Itinera, tuttavia, il nome non viene scomposto nelle sue componenti ma inserito integralmente in un unico _piece_ con il _tag_ "nome generico" (🚧 ma forse ora, eliminato vincolo nome=id, si può scomporre).

#### Type
Selezionare dal menu a tendina _solo ed esclusivamente_ **nome generico**.

#### Value
Inserire la stringa di testo con il nome.
> Francesco Petrarca  
> Giovanni Boccaccio  
> Sennuccio Del Bene

### Assertion
Qualora lo si ritenga opportuno è possibile qualificare l'attendibilità del dato o richiamare fonti o voci bibliografiche specifiche mediante [Assertion](Assertion_Brick.md).
 
## Save ⚠️ 
Per ogni elemento _name_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
