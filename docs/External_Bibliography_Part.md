# Bibliography Part e External Bibliography

**Bibliography Part** raccoglie la bibliografia relativa all'_item_, collegando il database di Itinera ad un database bibliografico esterno.  

Grazie a questa _part_ è possibile, all'interno di un'unica schermata:
* creare e gestire l'elenco delle voci bibliografiche relative all'item;  
* gestire il database bibliografico esterno, quindi aggiungere, modificare o cancellare voci bibliografiche.

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#bibliographypart).  

Per aggiungere la parte, selezionare **_bibliography_** dal menu a tendina della scheda di riepilogo dell'_item_, quindi cliccare su **_add part_**. 


## Bibliografia dell'item
Attraverso Bibliography Part è possibile creare una lista di voci bibliografiche (_entries_) relative all'_item_, selezionandole tra quelle presenti nel database bibliografico.  
Di norma vengono registrate in questa parte tutte le voci bibliografiche dedicate all'_item_ nel suo complesso, mentre voci bibliografiche dedicate a specifici aspetti possono essere richiamati nelle _parts_ corrispondenti mediante [DocReference](Docref_Brick.md).  

> 🚧 Esempi

Per aggiungere una _entry_ alla Bibliography Part di un _item_, cercare il titolo di interesse nella lista delle _entries_ già inserite nel database bibliografico.  
Se la voce bibliografica desiderata non è presente nel database bibliografico, occorre [crearla](External_Bibliography_Part.md#database-bibliografico). 

Una volta individuata la _entry_ desiderata, cliccare il tasto _pick this work_
> 🚧 immagine

Le _entries_ selezionate compariranno, in forma di lista, nella parte superiore della schermata.
> 🚧 immagine

Ogni _entry_ dispone di due campi:
* _tag_: permette di specificare la tipologia di voce bibliografica (🚧 arricchire thesaurus, mettere "---" preimpostato)
* _note_: 🚧 inserire, se pertinente, i numeri delle pagine della voce bibliografica relative all'item, preceduti da _p._ o _pp._. 

Per ogni _entry_ sono inoltre disponibili le seguenti funzioni:
* _view work_: permette di visualizzare per esteso la scheda dedicata alla _entry_;
* _edit this work_: permette di modificare la _entry_ all'interno del database bibliografico. ⚠️ Modificare una _entry_ nel database ha ricadute su tutti gli _item_ che vi si riferiscono;
* _remove this work from list_: permette di eliminare la _entry_ dalla bibliografia dell'_item_;
* _move up_ / _move down_: permette di modificare l'ordine delle _entries_ nella bibliografia dell'_item_;
* _copy work's ID_: permette di copiare l'id della _entry_. 
> 🚧 immagine


## Database bibliografico
Il database bibliografico raccoglie la totalità delle _entries_.  
Le _entries_ si distinguono in _entries_ semplici e _containers_ (opere che contengono più _entries_, ad es. periodici). Per visualizzare la lista dei _container_ spuntare la voce corrispondente.  
> 🚧 immagine  

Dalla lista è possibile visualizzare, modificare ed eliminare le _entries_ già inserite.  
⚠️ Modificare o eliminare una _entry_ nel database ha ricadute su tutti gli _item_ che vi si riferiscono.  

### Creare una voce bibliografica semplice (_entry_)
Per creare una nuova _entry_ cliccare il comando _+ new_.  
> 🚧 immagine  

Ogni _entry_ è strutturata nei seguenti campi:  
* _container_: non spuntare la casella;
* _typeId_: permette di specificare la tipologia di voce bibliografica selezionando tra: article; book; journal; proceedings;  
* _key_: chiave identificativa creata automaticamente; può essere utilizzata per richiamare sinteticamente la voce bibliografica in un [DocReference](Docref_Brick.md);   
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
  > 🚧 immagine  
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: non compilare;
    * roleId: selezionare, se pertinente, tra: curatore, traduttore, collaboratore, direttore, organizzatore;
   Dopo aver compilato i campi cliccare _accept authors_.
  > 🚧 immagine 
* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;
* _publisher_: editore;
* _container_: permette di indicare il contenitore, nel caso di articoli su rivista o in volumi miscellanei. Il contenitore può essere cercato digitando le prime lettere del titolo; deve essere già presente nel database nell'elenco dei _container_; in caso contrario, andrà creato prima della compilazione della _entry_ 
* _from-to_: permette di inserire le pagine, nel caso di articoli su rivista o in volumi miscellanei;
* _number_: permette di inserire il numero, nel caso di articoli su rivista o di collane;
* _note_: permette di aggiungere note di vario tipo;
* _location_: 🚧 permette di indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: 🚧 permette di indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca.  


Una volta compilati i campi salvare la _entry_ cliccando sul tasto di spunta blu.

### Creare un contenitore bibliografica (_container_)
Per creare un nuovo _container_ cliccare il comando _+ new_.  
> 🚧 immagine  

Ogni _container_ è strutturato nei seguenti campi: 
* _container_: spuntare la casella;
* _typeId_: permette di specificare la tipologia di voce bibliografica selezionando tra: article; book; journal; proceedings;  
* _key_: chiave identificativa creata automaticamente; può essere utilizzata per richiamare sinteticamente la voce bibliografica in un [DocReference](Docref_Brick.md);  
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
  > 🚧 immagine  
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: non compilare;
    * roleId: selezionare, se pertinente, tra: curatore, traduttore, collaboratore, direttore, organizzatore;
   Dopo aver compilato i campi cliccare _accept authors_.
  > 🚧 immagine 
* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;
* _publisher_: editore;
* _number_: permette di inserire il numero, nel caso di collane;
* _note_: permette di aggiungere note di vario tipo;
* _location_: 🚧 permette di indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: 🚧 permette di indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca.

Una volta compilati i campi salvare il _container_ cliccando sul tasto di spunta blu.

## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'_item_.
