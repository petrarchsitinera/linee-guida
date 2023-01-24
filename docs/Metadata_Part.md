# Metadata Part

**_Metadata Part_** permette di inserire alcune informazioni generali sull' _item_.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#metadatapart).

La parte è comune a tutti gli _item_: comprende sia voci generiche, da compilare in tutti gli item (_id_; _author_), sia voci specifiche (_tipologia testo_; _tipologia ms_; _modalità di esame ms_).

Per aggiungere la parte, selezionare **_meta_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Metadatum
Per ogni metadato è creato un elemento _metadatum_ mediante un [editor](Editor_Brick.md).

Ogni _metadatum_ è strutturato in tre campi: 
* _type_: permette di indicare, da thesaurus, la tipologia del metadato;  
* _name_: permette di indicare l'eventuale nome del metadato (se la sua compilazione non è pertinente, compilare con un trattino (**-**);  
* _value_: permette di inserire il valore del metadato.

La compilazione dei campi _name_ e _value_ dipende dalla tipologia di _metadatum_ che si intende creare, determinata attraverso il campo _type_.  
Nel campo _type_ è possibile selezionare un valore tra: 
* identificativo (da compilare per tutti gli _item_, obbligatorio);
* autore (da compilare per tutti gli _item_, obbligatorio);
* tipologia di testo (compilare solo per _Work Item_, ove pertinente); 
* modalità di esame ms (compilare solo per _Manuscript Item_, obbligatorio); 
* tipologia ms (compilare solo per _Manuscript Item_, obbligatorio); 
* altro (facoltativo).

### Identificativo
Permette di attribuire un identificativo univoco all'_item_, con il quale potrà essere richiamato nel database.  
Le regole relative alla composizione e all'utilizzo degli identificativi sono descritte [qui](Asserted_Ids_Part.md).  

* _type_: selezionare il valore _identificativo_;
* _name:_ compilare sempre con la voce **eid**;
* _value_: compilare con l'identificativo prescelto.  
⚠️ L'identificativo deve essere composto esclusivamente con i caratteri A-Z, 0-9; utilizzare sempre underscore (_) e mai trattino semplice (-); evitare l'uso di un numero come primo carattere dell'identificativo. 

La compilazione del campo è obbligatoria.

### Autore
Permette di indicare l'autore della scheda.  

* _type_: selezionare il valore _autore_;
* _name:_ compilare sempre con un trattino semplice (**-**).
* _value_: compilare con il nome e cognome del compilatore.  

La compilazione del campo è obbligatoria.


### Tipologia di testo
Permette di segnalare, relativamente ad un _Work Item_, il caso in cui il testo costituisca un frammento o una raccolta.  

* _type_: selezionare il valore _tipologia di testo_;
* _name:_ compilare sempre con un trattino semplice (**-**).
* _value_: compilare con _frammento_ se si tratta di un frammento di testo; con _raccolta_ se si tratta di una raccolta di testi (ad es. per l'item Rerum vulgarium fragmenta).  

Compilare se pertinente.

### Modalità di esame del manoscritto
Permette di indicare, relativamente ad un _Manuscript Item_, la modalità di esame del manoscritto.  

* _type_: selezionare il valore _modalità di esame ms_;
* _name:_ compilare sempre con un trattino semplice (**-**);
* _value_: compilare il campo con una delle seguenti opzioni: _autoptica_; _da riproduzione_; _da catalogo_; _da banca dati_.

⚠️ Nel caso in cui la scheda sia _da catalogo_ o _da banca dati_, compilare il campo _name_ con la _key_ bibliografica relativa alla fonte. [🚧 ma forse è più sensato invertire qui e per gli altri item name/value: valutare se ci sono controindicazioni 🚧]  

La compilazione del campo è obbligatoria.

### Tipologia manoscritto
* _type_: selezionare il valore _tipologia ms_;
* _name_:  compilare sempre con un trattino semplice (**-**);
* _value_: compilare il campo con una delle seguenti opzioni: _unitario_; _composito_; _fattizio_ (quando l'assemblaggio delle unità codicologiche non risale al progetto originario del manoscritto).

La compilazione del campo è obbligatoria.
