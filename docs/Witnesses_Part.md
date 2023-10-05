# Witnesses Part

**Witnesses Part** permette di inserire i testimoni manoscritti conosciuti di un testo.   

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#witnessespart).  

Per aggiungere la parte, selezionare _**witnesses**_ dal menu a tendina, quindi cliccare sul tasto _**add part**_.  

Attualmente, la compilazione della parte è riservata ai testi poetici.  

## Witness
Per ogni testimone è creato un elemento _witness_ mediante un [editor](Editor_Brick.md).

### ID
Compilare con la **segnatura completa** del testimone.  

Se il manoscritto è schedato all'interno di Itinera, la segnatura **deve coincidere** con quella usata come [_title_](Item_Manuscript_Metadata.md#title) dell'_item_ relativo. Per controllare la correttezza del dato, il compilatore può servirsi del [repository](repository.md) e della funzione di [lookup](lookup.md).    

Se il manoscritto non è schedato all'interno di Itinera, si riporta la segnatura completa secondo le medesime [regole](Item_Manuscript_Metadata.md#title).

### Location
Inserire la carta o l'intervallo di carte del manoscritto che trasmettono il testo indicato, specificando se si tratta di carte recto o verso, e la colonna se pertinente, secondo il modello [CodLocationRange](Cod_Location_Brick).  

## Save ⚠️ 

Per ogni elemento _witness_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
