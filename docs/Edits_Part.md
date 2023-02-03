# Edits Part
**Edits Part** permette di descrivere gli interventi scrittori successivi alla copia del codice (testi aggiunti, postille e annotazioni di vario tipo, correzioni, note di possesso, etc.).  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codeditspart).

Per aggiungere la parte, selezionare **_edits_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Edit
Per ogni intervento scrittorio è creato un elemento _edit_ mediante [editor](Editor_Brick.md).

⚠️ Per ogni elemento _edit_ inserito è necessario salvare cliccando sul tasto di spunta blu.

### EID
Permette di attribuire un identificativo arbitrario all'intervento scrittorio.  
Per ogni edit utilizzare l'etichetta convenzionale "edit" seguita senza spazi da un numero progressivo (es. "edit1", "edit2", etc.).   
Questo identificativo potrà essere utilizzato, in combinazione con l'identificativo dell'_item_ (cfr. [Regole per identificativi e authority file](identifiers.md), per collegare l'intervento a un evento relativo alla storia del manoscritto. È opportuno creare un collegamento qualora l'_edit_ testimoni un evento rilevante rispetto alla storia del codice.

> Per esplicitare il collegamento tra un _edit_ e la storia del manoscritto occorre registrare e descrivere nella parte Edits l'intervento, cui sarà attribuito un _eid_. In [EventsPart](Events_Part.md) dovrà essere creato un evento con type "editing" che abbia due _related entities_: 1. il nome dell'autore dell'intervento (type: "eseguito da"); 2. l'_eid_ dell'Edit in questione (type: "eid edit"). L'_eid_ dell'_edit_ deve essere cercato attraverso la funzione di [lookup](lookup.md) e ad esso deve essere premesso, separato da "/", l'identificativo dell'_item_ (la voce _item ID_ nella finestra di _lookup_).
   
> Se sul codice è presente una nota di possesso che permette di stabilire che il codice è stato posseduto da un personaggio noto, è necessario procedere nel seguente modo.
> Nella parte Edits registrare, trascrivere e descrivere la nota di possesso. A questa sarà attribuito un _eid_. In [EventsPart](Events_Part.md) dovrà essere creato un evento con type "possesso" che abbia due _related entities_: 1. il possessore del codice (type: "posseduto da"); 2. l'_eid_ dell'Edit in questione (type: "attestato da"). L'_eid_ dell'_edit_ deve essere cercato attraverso la funzione di [lookup](lookup.md) e ad esso deve essere premesso, separato da "/", l'identificativo dell'_item_ (la voce _item ID_ nella finestra di _lookup_).


### Type
Permette di indicare la tipologia dell'intervento scrittorio. Selezionare uno o più valori tra:

* testo avventizio
* postille/annotazioni
* commento
* correzioni
* integrazione
* rubriche
* segni paragrafematici
* titoli correnti
* segni di attenzione
* nota di possesso
* indici
* disegno
* altro

La compilazione del campo è obbligatoria.

### Tag
Può essere utilizzato per attribuire un _edit_ a una specifica mano, diversa da quelle principali, che devono invece essere registrate in HandsPart.  
Per ogni mano utilizzare l'etichetta convenzionale "mano" seguita da lettera alfabetica minuscola (es. "mano a", "mano b", etc.).  
Questo campo permette, in particolare, di collegare _edits_ differenti (es. un testo avventizio e una serie di correzioni) al medesimo _tag_, e quindi alla medesima mano.  
Non è necessario ricorrere al _tag_ nel caso in cui l'autore degli _edits_ sia noto; in questo caso l'attribuzione della paternità degli interventi è registrata in EventsPart (vedi sopra).  

La compilazione del campo è facoltativa.

### Location
Permette di indicare la localizzazione sul codice dell' _edit_, secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

### Techniques
Permette di indicare la tecnica con la quale è stato eseguito l' _edit_. Selezionare uno o più valori tra:
* inchiostro
* lapis
* altro

La compilazione del campo è facoltativa.

### Datation
Permette di indicare l'epoca dell' _edit_, secondo il sottomodello _date_ del modello [Asserted Chronotope](Asserted_Chronotope_Brick.md). 
La compilazione del campo è facoltativa.

### Language
Permette di indicare la lingua dell' _edit_. Selezionare un valore tra:

*  \---
* inglese
* francese
* tedesco
* greco
* neogreco
* italiano
* latino
* latino-volgare
* spagnolo
* altro

La compilazione del campo è obbligatoria (se non pertinente spuntare il campo "\---").


### Colors
Permette di indicare il colore dell'inchiostro utilizzato per l' _edit_. Selezionare uno o più valori tra:

* bruno scuro
* bruno chiaro
* rosso
* blu
* altro

La compilazione del campo è facoltativa.

### Description
Permette di inserire una descrizione discorsiva dell' _edit_, sia nei suoi aspetti grafici che contenutistici.  
La compilazione del campo è facoltativa.

### Text
Permette di riportare il testo integrale (nel caso, ad esempio, di note di possesso) o un estratto dell' _edit_.  
La compilazione del campo è facoltativa.

### References
Permette di registrare l'eventuale bibliografia relativa all' _edit_ in oggetto, secondo le norme definite per [Bibliography Part](External_Bibliography_Part.md).  
L'elemento è replicabile per ogni voce bibliografica.   
La compilazione del campo è facoltativa.


## Save ⚠️ 
Per ogni elemento _edit_ inserito è necessario salvare cliccando sul tasto di spunta blu.  

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
