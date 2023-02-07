# Watermarks Part
**Watermarks Part** permette di identificare e descrivere le filigrane presenti nei manoscritti cartacei.

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codwatermarkspart).

Per aggiungere la parte, selezionare **_watermarks_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Watermark
Per ogni filigrana è creato un elemento _watermark_ mediante un [editor](Editor_Brick.md).

### Name
Permette di indicare in modo sintetico il soggetto della filigrana. Se la filigrana è presente in uno o più repertori, è consigliabile attenersi alla classificazione già adottata.

La compilazione del campo è obbligatoria.

### Sample
Permette di indicare la carta sulla quale si effetua l'identificazione e la misurazione della filigrana secondo il modello [Cod Location](Cod_Location_Brick.md).

La compilazione del campo è obbligatoria.

### Ranges
Permette di indicare le carte o gli intervalli di carte sulle quali è presente la filigrana secondo il modello [Cod Location](Cod_Location_Brick.md).

La compilazione del campo è facoltativa.

### Description
Permette di fornire una descrizione approfondita del soggetto della filigrana e segnalare eventuali particolarità o differenze rispetto al repertorio.

La compilazione del campo è facoltativa.

### Identifiers
Permette di identificare la filigrana con una o più esemplari presenti nei repertori, secondo il modello [Asserted IDs](Asserted_Ids_Brick.md).
Per ogni riscontro è possibile creare un elemento _ID_ mediante un [editor](Editor_Brick.md).

* _tag_: non compilare;  
* _scope_: indicare il nome del repertorio "Briquet" o "Piccard", in questa forma;  
* _value_: indicare il numero d’ordine della filigrana all'interno del repertorio indicato in _scope_ .
* _Assertion_: permette di esprimere il grado di somiglianza della filigrana rilevata sul manoscritto con l'esemplare del repertorio.
  * _tag_: non compilare;  
  * _rank_: selezionare un valore tra 1 (“identico a”), 2 (“simile a”), 3 (“variante di”);
  * _note_: non compilare;
  * _Assertion References_: compilare il solo campo _citation_ con l'indirizzo web della pagina dedicata alla filigrana individuata.

La compilazione del campo è facoltativa.

### Size
Per esprimere le dimensioni della filigrana spuntare la casella _has size_.

Le dimensioni di altezza e larghezza sono inserite, espresse in millimetri, attraverso il modello [Physical Size](Physical_Size_Brick.md).

La compilazione del campo è facoltativa.

### Chronotope 
Qualora la filigrana rilevata sul manoscritto trovi riscontro in un repertorio (vedi External Id), indicare relativi data e luogo secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).

La compilazione del campo è obbligatoria solo nel caso in cui sia stata compilata la sezione External Id.

## Save ⚠️ 

Per ogni elemento _watermark_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
