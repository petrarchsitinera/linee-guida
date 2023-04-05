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
Permette di attribuire un identificativo univoco all'_item_, con il quale potrà essere richiamato in altre parti del database.  
Gli identificativi dei testi che fanno parte dei _corpora_ di Itinera sono già assegnati secondo le regole descritte [qui](identifiers.md) e sono consultabili nel [repository](repository.md). 
Nel caso di nuove immissioni, gli _eid_ si attribuiscono secondo le medesime [regole](identifiers.md), segnalando le aggiunte in clickup per permettere l'aggiornamento del [repository](repository.md).  

* _type_: selezionare il valore _identificativo_;
* _name:_ compilare sempre con la voce **eid**;
* _value_: compilare con l'identificativo prescelto.  

Esempio. Nell'immagine l'identificativo dell'_item_ Epystole (compilato da Mario Rossi).  

<img width="1136" alt="Schermata 2023-04-05 alle 12 28 12" src="https://user-images.githubusercontent.com/102725489/230055569-eb3e7db9-0049-468a-83df-85ce97819e51.png">

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


## Save ⚠️ 

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
