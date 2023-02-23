# Bibliography Part e External Bibliography

**Bibliography Part** raccoglie la bibliografia relativa all'_item_, collegando il database di Itinera ad un database bibliografico esterno.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#bibliographypart). 

Grazie a questa _part_ è possibile, all'interno di un'unica schermata:
* creare e gestire l'elenco delle voci bibliografiche relative all'item;  
* gestire il database bibliografico esterno, quindi aggiungere, modificare o cancellare voci bibliografiche.

Il database bibliografico è dunque accessibile:
* direttamente, cliccando la voce Bibliography nel menu orizzontale nella parte alta della schermata: 
> ![](https://github.com/petrarchsitinera/linee-guida/blob/def4a09b59b5012905bebdb1fc6da7358a086762/docs/assets/images/bibl7.png?raw=true)
* dall'interno di un item, aggiungendo Bibliography Part: per aggiungere la parte, selezionare **_bibliography_** dal menu a tendina della scheda di riepilogo dell'_item_, quindi cliccare su **_add part_**. 


## Bibliografia dell'item
Attraverso Bibliography Part è possibile creare una lista di voci bibliografiche (_entries_) relative all'_item_, selezionandole tra quelle presenti nel database bibliografico.  
Di norma vengono registrate in questa parte tutte le voci bibliografiche dedicate all'_item_ nel suo complesso, mentre voci bibliografiche dedicate a specifici aspetti possono essere richiamati nelle _parts_ corrispondenti mediante [DocReference](Docref_Brick.md).  

Per aggiungere una _entry_ alla Bibliography Part di un _item_, cercare il titolo di interesse nella lista delle _entries_ già inserite nel database bibliografico.  

> ![](https://github.com/petrarchsitinera/linee-guida/blob/a774c9e27b3631e2158f67ecded8da7192cee972/docs/assets/images/bibl0.png?raw=true)
 
Se la voce bibliografica desiderata non è presente nel database bibliografico, occorre [crearla](External_Bibliography_Part.md#database-bibliografico). 

Una volta individuata la _entry_ desiderata, cliccare il tasto _pick this work_
> ![](https://github.com/petrarchsitinera/linee-guida/blob/a774c9e27b3631e2158f67ecded8da7192cee972/docs/assets/images/bibl3.png?raw=true)

Le _entries_ selezionate compariranno, in forma di lista, nella parte superiore della schermata.
> ![](https://github.com/petrarchsitinera/linee-guida/blob/a774c9e27b3631e2158f67ecded8da7192cee972/docs/assets/images/bibl1.png?raw=true)

Ogni _entry_ dispone di due campi:
* _tag_: permette di specificare la tipologia di voce bibliografica;  
* _note_: inserire, se pertinente, i numeri delle pagine della voce bibliografica relative all'item, preceduti da _p._ o _pp._.  

Per ogni _entry_ sono inoltre disponibili le seguenti funzioni:
* _view work_: permette di visualizzare per esteso la scheda dedicata alla _entry_;
* _edit this work_: permette di modificare la _entry_ all'interno del database bibliografico.   
⚠️ Modificare una _entry_ nel database ha ricadute su tutti gli _item_ che vi si riferiscono;
* _remove this work from list_: permette di eliminare la _entry_ dalla bibliografia dell'_item_;
* _move up_ / _move down_: permette di modificare l'ordine delle _entries_ nella bibliografia dell'_item_;
* _copy work's ID_: permette di copiare l'id della _entry_. 


## Database bibliografico
Il database bibliografico raccoglie la totalità delle _entries_.  
Le _entries_ si distinguono in _works_ e _containers_ (opere che contengono più _works_, ad es. periodici). Per visualizzare la lista dei _containers_ spuntare la casella relativa.  
> ![](https://github.com/petrarchsitinera/linee-guida/blob/e3eba119e269037d6a7a224fe257d6b897d7c49c/docs/assets/images/bibl2.png?raw=true)  

Dalla lista è possibile visualizzare, modificare ed eliminare le _entries_ già inserite.  
⚠️ Modificare o eliminare una _entry_ nel database ha ricadute su tutti gli _item_ che vi si riferiscono.  

### Creare una voce bibliografica semplice (_work_)
Per creare un nuovo _work_ cliccare il comando _+ new_.  
> ![](https://github.com/petrarchsitinera/linee-guida/blob/38a8a79aa3f74a4443f314f9d08e2dcd996032c7/docs/assets/images/bibl2a.png?raw=true)   

Ogni _work_ è strutturato nei seguenti campi:  
* _container_: non spuntare la casella;
* _typeId_: permette di specificare la tipologia di voce bibliografica selezionando tra: article; book; journal; proceedings;  
* _key_: chiave identificativa della voce biliografica, che può essere utilizzata per richiamare sinteticamente la voce in [DocReference](Docref_Brick.md);
  * la chiave è, di norma, creata automaticamente a partire dal cognome dell'autore o degli autori e dalla data della pubblicazione; in caso di identità (ad es. per   pubblicazioni dello stesso autore uscite nello stesso anno) la chiave è disambiguata automaticamente attraverso l'apposizione di un lettera);  
  * se si desidera attribuire una chiave diversa da quella generata automaticamente (ad es. per opere senza anno o senza autore), spuntare la casella _user key_.  
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/b6f38e89e2d111d405164114fd26681777fd4b03/docs/assets/images/bibl5.png?raw=true)   
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: non compilare;
    * roleId: selezionare, se pertinente, tra: curatore, traduttore, collaboratore, direttore, organizzatore;
   Dopo aver compilato i campi cliccare _accept authors_.

* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;
* _year2_: se l'anno di edizione corrisponde a un intervallo (in questo caso attribuire una _key_ bibliografica arbitraria, poiché quella automatica indica solo il valore inserito in _year_);   
* _publisher_: editore;
* _container_: permette di indicare il contenitore, nel caso di articoli su rivista o in volumi miscellanei. Il contenitore può essere cercato digitando le prime lettere del titolo; deve essere già presente nel database nell'elenco dei _container_; in caso contrario, andrà creato prima della compilazione della _entry_ 
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/4cdc916490f77390f06ed821a68f27d7dd39b224/docs/assets/images/bibl6.png?raw=true)   
* _from-to_: permette di inserire le pagine, nel caso di articoli su rivista o in volumi miscellanei;
* _number_: permette di inserire il numero, nel caso di articoli su rivista o di collane;
* _note_: permette di aggiungere note di vario tipo;
* _location_: permette di indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: permette di indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca.  


Una volta compilati i campi salvare la _entry_ cliccando sul tasto di spunta blu.

### Creare un contenitore bibliografico (_container_)
Per creare un nuovo _container_ cliccare il comando _+ new_.  
> ![](https://github.com/petrarchsitinera/linee-guida/blob/38a8a79aa3f74a4443f314f9d08e2dcd996032c7/docs/assets/images/bibl2a.png?raw=true)  

Ogni _container_ è strutturato nei seguenti campi: 
* _container_: spuntare la casella;
> ![](https://github.com/petrarchsitinera/linee-guida/blob/38a8a79aa3f74a4443f314f9d08e2dcd996032c7/docs/assets/images/bibl4.png?raw=true)  

* _typeId_: permette di specificare la tipologia di voce bibliografica selezionando tra: article; book; journal; proceedings;  
* _key_: chiave identificativa della voce biliografica, che può essere utilizzata per richiamare sinteticamente la voce in [DocReference](Docref_Brick.md);
  * la chiave è, di norma, creata automaticamente a partire dal cognome dell'autore o degli autori e dalla data della pubblicazione; in caso di identità (ad es. per   pubblicazioni dello stesso autore uscite nello stesso anno) la chiave è disambiguata automaticamente attraverso l'apposizione di un lettera);  
  * se si desidera attribuire una chiave diversa da quella generata automaticamente (ad es. per opere senza anno o senza autore), spuntare la casella _user key_.  
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
 > ![](https://github.com/petrarchsitinera/linee-guida/blob/b6f38e89e2d111d405164114fd26681777fd4b03/docs/assets/images/bibl5.png?raw=true)   
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: non compilare;
    * roleId: selezionare, se pertinente, tra: curatore, traduttore, collaboratore, direttore, organizzatore;
   Dopo aver compilato i campi cliccare _accept authors_.  
* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;  
* _year2_: se l'anno di edizione corrisponde a un intervallo (in questo caso attribuire una _key_ bibliografica arbitraria, poiché quella automatica indica solo il valore inserito in _year_);   
* _publisher_: editore;
* _number_: permette di inserire il numero, nel caso di collane;
* _note_: permette di aggiungere note di vario tipo;
* _location_: permette di indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: permette di indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca.

Una volta compilati i campi salvare il _container_ cliccando sul tasto di spunta blu.

## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'_item_.
