# Bibliography Part

**Bibliography Part** raccoglie le voci bibliografiche relative all'_item_, collegando il database di Itinera ad un database [bibliografico esterno](bibliodb.md).  

Attraverso Bibliography Part è possibile aggiungere all'_item_ 
- voci bibliografiche già presenti nel [database bibliografico esterno](bibliodb.md), selezionandole dalla lista;
- creare _ad hoc_ nuove voci bibliografiche che saranno automaticamente aggiunte al [database bibliografico esterno](bibliodb.md).

La descrizione del modello è disponibile [qui](https://github.com/vedph/cadmus-general#bibliographypart). 

Per aggiungere la parte, selezionare **_bibliography_** dal menu a tendina, quindi cliccare sul tasto **add part**.  

## Bibliografia dell'_item_

Di norma vengono registrate nella Bibliography Part sia le voci bibliografiche dedicate all'_item_ nel suo complesso sia le edizioni del testo schedato (critiche o meno, commentate, ecc.). 

Le voci bibliografiche dedicate ad aspetti specifici sono richiamate invece nelle _parts_ corrispondenti attraverso la compilazione di apposite [DocReference](Docref_Brick.md).

## Aggiungere una voce bibliografica all'_item_

Per aggiungere una voce bibliografica già presente nel database bibliografico alla Bibliography Part di un _item_, cercarla nella lista delle _entries_ come indicato [qui](bibliodb.md#cercare-voci-bibliografiche), quindi selezionarla cliccando il pulsante _pick this work_ (cerchiato in rosso nell'immagine). La voce bibliografica comparirà così nella lista presente nella parte superiore della schermata, entrando a far parte della bibliografia dell'_item_.

<img width="1440" alt="Schermata 2023-04-06 alle 15 45 41" src="https://user-images.githubusercontent.com/102725489/230397366-67dacae5-ce5b-45c0-9965-3b4eb840f646.png">

Se la voce bibliografica desiderata non è presente nel database bibliografico, aggiungerla secondo le istruzioni indicate [qui](bibliodb.md#aggungere-voci-bibliografiche).   
Una volta creata la voce bibliografica, procedere come indicato sopra per aggiungerla alla bibliografia dell'_item_.

Per ogni voce bibliografica aggiunta all'_item_, è **obbligatorio** compilare due campi:
* _tag_: selezionare la tipologia di voce bibliografica tra _edizioni_ (per le edizioni, anche commentate), _studi_ (per gli studi), _-_ (in tutti gli altri casi)  
* _note_: inserire, se pertinente, il numero di pagina/e della voce bibliografica **specificamente dedicate all'item** (non i numeri di pagina della voce bibliografica!), preceduti da _p._ o _pp._.  

## Eliminare una voce bibliografica all'_item_

Per eliminare una voce bibliografica dalla lista della bibliografia di un _item_, cliccare su _delete this work_ (cerchiato in rosso nell'immagine).  

L'eliminazione della voce dalla bibliografia dell'_item_ NON comporta l'eliminazione della voce dal database bibliografico.

<img width="1434" alt="Schermata 2023-04-06 alle 16 06 36" src="https://user-images.githubusercontent.com/102725489/230402420-a533f576-4fc3-429f-8dff-f486de0fc3e1.png">


## Altre operazioni

Nella lista delle voci bibliografiche di un _item_ è possibile effettuare inoltre le seguenti azioni:

* _view work_: per [visualizzare la voce bibliografica](bibliodb.md#visualizzare-voci-bibliografiche);
* _edit this work_: per [modificare la voce bibliografica](bibliodb.md#modificare-voci-bibliografiche);   
* _move up_ / _move down_: per modificare l'ordine delle voci nella lista;
* _copy work's ID_: per copiare l'identificativo non _human-friendly_ della voce bibliografica.


## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'_item_.
