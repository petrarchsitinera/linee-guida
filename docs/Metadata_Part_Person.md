# Metadata Part di Item Person

I metadati da aggiungere **obbligatoriamente** in un Item Person sono:  
* identificativo;
* autore.

## Metadatum
Ciascun metadato è inserito come un elemento singolo (_metadatum_) - cfr. la sezione [Creare, modificare, eliminare e salvare elementi](Editor_Brick.md).

Ogni _metadatum_ è strutturato in tre campi: 
* _type_: permette di indicare, da thesaurus, la tipologia del metadato;  
* _name_: permette di indicare l'eventuale nome del metadato (**se la sua compilazione non è pertinente**, compilare con un trattino: **-**);  
* _value_: permette di inserire il valore del metadato.

### Identificativo
Permette di attribuire un identificativo univoco all'_item_, con il quale potrà essere richiamato in altre parti del database.  
Gli identificativi delle persone che fanno parte dei _corpora_ di Itinera sono già assegnati secondo le regole descritte [qui](identifiers.md) e sono consultabili nel [repository](repository.md). 
Nel caso di nuove immissioni, gli _eid_ si attribuiscono secondo le medesime [regole](identifiers.md), segnalando le aggiunte in clickup per permettere l'aggiornamento del [repository](repository.md).  

* _type_: selezionare il valore _identificativo_;
* _name:_ compilare sempre con la voce **eid**;
* _value_: compilare con l'identificativo prescelto.  

<img width="1135" alt="Schermata 2023-04-05 alle 12 23 37" src="https://user-images.githubusercontent.com/102725489/230054099-f6f59ae1-080c-4670-bc49-ffb58fc646d7.png">

La compilazione del campo è **obbligatoria**.

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
Permette di indicare, relativamente ad un _Manuscript Item_, la modalità di esame e di schedatura del manoscritto.  

* _type_: selezionare il valore _modalità di esame ms_;
* _name:_ compilare il campo con una delle seguenti opzioni: _analatica_; _sintetica_:  
* _value_: compilare il campo con una delle seguenti opzioni: _autoptica_; _da riproduzione_; _da catalogo_; _da banca dati_.

⚠️ Nel caso in cui la scheda sia _da catalogo_ o _da banca dati_, creare un ulteriore _metadatum_ con:  
* _type_: selezionare il valore _altro_;
* _name:_ compilare con la voce **fonte**;
* _value_: se la scheda è tratta _da catalogo_, compilare con la _key_ bibliografica relativa alla fonte (cfr. [Bibliography Part](External_Bibliography_Part.md)); se la scheda è tratta _da banca dati_, compilare il campo con il nome o la sigla della banca dati (ad es. "Mirabile", "RDP", "Manus", etc.)

La compilazione del campo è obbligatoria.

### Tipologia manoscritto
* _type_: selezionare il valore _tipologia ms_;
* _name_:  compilare sempre con un trattino semplice (**-**);
* _value_: compilare il campo con una delle seguenti opzioni: _unitario_; _composito_; _fattizio_ (quando l'assemblaggio delle unità codicologiche non risale al progetto originario del manoscritto).

La compilazione del campo è obbligatoria.

## Save ⚠️ 

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
