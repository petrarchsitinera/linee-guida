# Witnesses Part

**Witnesses Part** permette di inserire il testimoniale di un testo.   

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#witnessespart).  

Per aggiungere la parte, selezionare _**witnesses**_ dal menu a tendina, quindi cliccare sul tasto _**add part**_.  

Attualmente, la compilazione della parte è riservata ai testi poetici.  

## Witness
Per ogni testimone è creato un elemento _witness_ mediante un [editor](Editor_Brick.md).

### ID
Compilare con l'identificativo del manoscritto in cui è localizzato il testimone.  
L'identificativo coincide con la segnatura del codice per esteso, i cui elementi sono separati da **virgola**:

**Città, Biblioteca (nome ufficiale), fondo, collocazione**.  

Controllare se il manoscritto è presente sul **repository dei manoscritti Itinera** e in tal caso utilizzare il medesimo identificativo.
🚧 ma vedi lookup


### Location
Inserire la carta o l'intervallo di carte del manoscritto che trasmettono il testo indicato, specificando se si tratta di carte recto o verso, e la colonna se pertinente, secondo il modello [CodLocationRange](Cod_Location_Brick).  

## Save ⚠️ 

Per ogni elemento _witness_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
