# Bindings Part
**Bindings Part** permette di descrivere la legatura corrente del manoscritto. La parte consente, inoltre, di registrare eventuali legature precedenti, quando note, o di indicare l'assenza di legatura. In quest'ultimo caso, occorre creare comunque un elemento _binding_ e compilare i campi come specificato di seguito.

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codbindingspart).

Per aggiungere la parte, selezionare **_bindings_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Binding
Per ogni legatura è creato un elemento _binding_ mediante [[editor|Editor_Brick]].

### Tag
Permette di indicare se l'elemento aggiunto corrisponde alla legatura attuale, a una legatura precedente, oppure se il manoscritto è privo di legatura. Selezionare una voce dal thesaurus:
* attuale
* precedente
* assente

La compilazione del campo è facoltativa. Se non specificato la segnatura inserita sarà interpretata come quella attuale.

### Cover
Permette di indicare il materiale di copertura. Selezionare una voce dal thesaurus::
* --- (per legatura assente)
* pelle
* cuoio
* membrana
* velluto
* tessuto
* carta
* altro

La compilazione del campo è obbligatoria.

### Board
Permette di indicare il materiale del supporto. Selezionare una voce dal thesaurus:  
* --- (per legatura assente)
* legno
* cartone
* altro

La compilazione del campo è obbligatoria.

### Size
Per esprimere le dimensioni della legatura spuntare la casella _has size_.

Le dimensioni di altezza, larghezza e spessore sono inserite in millimetri secondo il modello [Physical Size](Physical_Size_Brick.md).

La compilazione del campo è facoltativa.

### Description
Permette di fornire una sommaria descrizione della legatura. 

È possibile: descrivere dettagliatamente la legatura, specificando numero di nervi, cucitura, supporti della cucitura, presenza capitelli, presenza di tagli rifilati, colorati o decorati; descrivere la decorazione; segnalare la presenza del titolo o di altre indicazioni (manoscritte o a stampa) presenti sul materiale di copertura; indicare il materiale ed eventualmente la datazione approssimativa delle controguardie; in caso di restauro, indicare in maniera generica la tipologia dell’intervento (es. legatura di restauro con reimpiego della coperta) e l’anno dello stesso (🚧 eventuale rimando a Events: restauro)

⚠️ Se sulla legatura sono presenti elementi (stemmi, anagrammi, etichette, etc.) grazie ai quali è possibile è identificare un possessore del manoscritto, nella [EventsPart](Events_Part.md) dovrà essere creato un evento con type "possesso" che abbia due _related entities_: 1. il possessore del codice (type: "posseduto da"); 2. la dicitura "legatura" (type: "testimoniato da").  

La compilazione del campo è facoltativa.

### Chronotope
Permette di indicare la data e il luogo della legatura secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).

La compilazione del campo è obbligatoria relativamente alla datazione.

## Save ⚠️ 

Per ogni elemento _binding_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.

