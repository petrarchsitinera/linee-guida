# Metadata Part di Item Text

I metadati da aggiungere **obbligatoriamente** in un Item Person sono:  
* identificativo;
* autore.

È obbligatorio nei casi che lo richiedono anche:  
* tipologia di testo.

## Metadatum
Ciascun metadato è inserito come un elemento singolo (_metadatum_) - cfr. la sezione [Creare, modificare, eliminare e salvare elementi](Editor_Brick.md).  

Ogni _metadatum_ è strutturato in tre campi: 
* _type_: permette di indicare, da thesaurus, la tipologia del metadato;  
* _name_: permette di indicare l'eventuale nome del metadato (**se la sua compilazione non è pertinente**, compilare con un trattino: **-**);   
* _value_: permette di inserire il valore del metadato.


### Identificativo
Permette di attribuire un identificativo univoco all'_item_, con il quale potrà essere richiamato nel database.  
Le regole relative alla composizione e all'utilizzo degli identificativi sono descritte [qui](identifiers.md).  

* _type_: selezionare il valore _identificativo_;
* _name:_ compilare sempre con la voce **eid**;
* _value_: compilare con l'identificativo prescelto.  

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


## Save ⚠️ 

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
