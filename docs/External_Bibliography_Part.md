# Bibliography Part

**Bibliography Part** raccoglie le voci bibliografiche relative all'_item_, collegando il database di Itinera ad un database [bibliografico esterno](bibliodb.md).  

Attraverso Bibliography Part è possibile aggiungere all'_item_ 
- voci bibliografiche già presenti nel [database bibliografico esterno](bibliodb.md), selezionandole dalla lista;
- creare _ad hoc_ nuove voci bibliografiche che saranno automaticmente aggiunte al [database bibliografico esterno](bibliodb.md).

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#bibliographypart). 

Per aggiungere la parte, selezionare **_bibliography_** dal menu a tendina, quindi cliccare sul tasto **add part**.  

## Bibliografia dell'_item_

Di norma vengono registrate nella Bibliography Part sia le voci bibliografiche dedicate all'_item_ nel suo complesso sia le edizioni del testo schedato. (critiche o meno, commentate, ecc.). 

Le voci bibliografiche dedicate ad aspetti specifici sono richiamate invece nelle _parts_ corrispondenti attraverso la compilazione di apposite [DocReference](Docref_Brick.md).

## Aggiungere una voce bibliografica all'_item_

Per aggiungere una voce bibliografica già presente nel database bibliografico alla Bibliography Part di un _item_, cercarla nella lista delle _entries_ come indicato [qui](bibliodb.md#cercare-voci-bibliografiche), quindi selezionarla cliccando il pulsante _pick this work_ (cerchiato in rosso nell'immagine). La voce bibliografica comparirà così nella lista presente nella parte superiore della schermata, entrando a far parte della bibliografia dell'_item_.

<img width="1440" alt="Schermata 2023-04-06 alle 15 45 41" src="https://user-images.githubusercontent.com/102725489/230397366-67dacae5-ce5b-45c0-9965-3b4eb840f646.png">

Se la voce bibliografica desiderata non è presente nel database bibliografico, aggiungerla secondo le istruzioni indicate [qui](bibliodb.md#aggungere-voci-bibliografiche).   
Una volta creata la voce bibliografica, procedere come indicato sopra per aggiungerla alla bibliografia dell'_item_.


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
