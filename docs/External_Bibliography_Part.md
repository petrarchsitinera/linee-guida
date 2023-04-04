# Bibliography Part e External Bibliography

**Bibliography Part** raccoglie la bibliografia relativa all'_item_, collegando il database di Itinera ad un database bibliografico esterno.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#bibliographypart). 

Grazie a questa _part_ è possibile, all'interno di un'unica schermata:
* creare e gestire l'elenco delle voci bibliografiche relative all'_item_;  
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
