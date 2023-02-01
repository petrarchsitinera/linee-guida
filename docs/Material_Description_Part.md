# Material Description Part
**Material Description Part** permette di inserire alcune informazioni relative agli aspetti materiali del manoscritto o, se composito o fattizio, delle singole unità codicologiche. La parte è deputata anche alla descrizione degli elementi palinsesti. 

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codmaterialdscpart).

Per aggiungere la parte, selezionare **_material_** dal menu a tendina, quindi cliccare su **_add part_**.  


## Units
Per ogni unità codicologica è creato un elemento _unit_ mediante [editor](Editor_Brick.md).
Se il manoscritto è unitario, è creato un unico elemento _unit_.


### Eid
Rappresenta l'identificativo dell'unità codicologica, che può essere richiamato in altre sezioni (_parts_) dell'_item_.  

Per ogni unità codicologica utilizzare la formula convenzionale "u" seguita senza spazi dal numero progressivo dell'unità (es. "u1", "u2", etc.).  
Per ulteriori informazioni sull'utilizzo degli _eid_ vedi [qui](identifiers.md).   
Se il manoscritto è unitario, lasciare il campo vuoto.

### Tag
Permette di inserire un'etichetta descrittiva utile ai fini della ricerca.

La compilazione del campo è facoltativa.

### Material
Permette di indicare la materia scrittoria del manoscritto o dell'unità codicologica. Selezionare un valore tra:
* membr. (per manoscritti membranacei/unità codicologiche membranacee)
* cart. (per manoscritti cartacei/unità codicologiche cartacee)
* misto (per manoscritti/unità codicologiche con fogli cartacei e membranacei)

La compilazione del campo è obbligatoria.

### NoGregory
Il flag viene spuntato nel caso in cui la regola di Gregory non sia rispettata.

La compilazione del campo è riservata ai manoscritti membranacei.

### Format
Permette di indicare il formato del manoscritto o dell'unità codicologica. Selezionare un valore tra:
* --- (per i manoscritti membranacei)
* in-folio
* in-4°
* in-8°
* in-16°
* altro

La compilazione del campo è riservata ai manoscritti cartacei.

### State
Permette di indicare lo stato di conservazione del manoscritto o dell'unità codicologica. Selezionare un valore tra:
* ottimo
* buono
* discreto
* precario
* pessimo

La compilazione del campo è obbligatoria.

### Range
Permette di indicare l'intervallo di carte di ciascuna unità codicologica secondo il modello [Cod Location](Cod_Location_Brick.md).

Nel caso di manoscritto unitario si indicano la prima e l'ultima carta del codice (escluse le carte di guardia).

La compilazione del campo è obbligatoria.

### Chronotopes
Permette di indicare la data e il luogo di produzione del manoscritto o dell'unità codicologica secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).

⚠️ Per manoscritti datati indicare "datato" nel campo _tag_ di _date_. L'eventuale sottoscrizione del copista è descritta e riportata nella sezione Subscriptions di [Cod Hands Part](Hands_Part.md).  
⚠️ In presenza di più sottoscrizioni datate, è possibile, a discrezione del compilatore, esprimere i dati cronologici creando differenti elementi Asserted Chronotope.  
⚠️ In presenza di differenti datazioni della critica che si ritengano ugualmente probabili, è possibile esprimere le ipotesi creando differenti elementi Asserted Chronotope, precisandone l'attendibilità attraverso il campo _rank_ di [Assertion](Assertion_Brick.md).

La compilazione del campo è obbligatoria.  
 
Per il luogo, compilare il campo _place_ con un unico valore, corrispondente all'indicazione geografica più precisa tra città/regione/area/stato.  
Solo nel caso in cui sia possibile fornire un'indicazione topografica più precisa rispetto alla città (ad es. un edificio, una via, un quartiere, etc.), si indica il nome della città seguito da tale indicazione, separate da virgola.

> place= "Venezia"  
> place= "Lazio"  
> place= "Italia meridionale"  
> place= "Firenze, carcere delle Stinche"  
 
Per la data, se non è possibile offrire un'indicazione cronologica più specifica, utilizzare datazioni al secolo.  

### Note
Si raccolgono qui dati e informazioni che non è possibile inserire ricorrendo ai modelli. In questo campo è possibile segnalare l’eventuale presenza di carte danneggiate (con indicazione della posizione e della tipologia del danneggiamento) e di eventuali carte sciolte.

La compilazione del campo è facoltativa.

### ⚠️ Save
Per ogni elemento _unit_ inserito è necessario salvare cliccando sul tasto di spunta blu.


## Palimpsests
Per ogni carta palinsesta o per gruppi di carte palinseste di comune provenienza, è creato un elemento _palimpsest_ mediante [editor](Editor_Brick.md).

### Range
Permette di indicare la collocazione della carta palinsesta o del gruppo di carte palinseste secondo il modello [Cod Location](Cod_Location_Brick.md).

La compilazione del campo è obbligatoria.

### Chronotopes
Permette di indicare i dati cronologici relativi alla _scriptio inferior_ secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).

La compilazione del campo è facoltativa.

### Note
Si raccolgono qui dati e informazioni che non è possibile inserire ricorrendo ai modelli. In questo campo è possibile fornire una breve caratterizzazione della _scriptio inferior_, specificando il tipo di documento e le caratteristiche generali della scrittura.

La compilazione del campo è facoltativa.


### ⚠️ Save
Per ogni elemento _palimpsest_ inserito è necessario salvare cliccando sul tasto di spunta blu.


## ⚠️ Save
Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
