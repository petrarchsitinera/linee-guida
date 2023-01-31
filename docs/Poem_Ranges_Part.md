# Poem Ranges Part

**Poem Ranges Part** permette di inserire informazioni su alcune caratteristiche del testimone dei _Rerum vulgarium fragmenta_, quali:
* l'eventuale presenza della divisione dell'opera in due parti;
* l’ordine dei componimenti;
* la tipologia di impaginazione.

La parte si articola in tre sezioni: ranges, layout, note.

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#codpoemrangespart).

Per aggiungere la parte selezionare **poem ranges** dal menu a tendina della scheda di riepilogo dell'item, quindi cliccare sul comando **add part**.

## Ranges

### Type

Permette di indicare se l'opera presenta divisione in due parti e se essa coincida con quella petrarchesca. Selezionare una voce dal thesaurus:
* assente (non c'è divisione in parti)
* petrarchesca (la divisione in parti cade tra Rvf 263 e 264)
* non petrarchesca (la divisione in parti è presente ma non cade tra Rvf 263 e 264)

La compilazione del campo è obbligatoria.

### Ranges

Permette di registrare la sequenza dei componimenti quale è presentata dal testimone.

> La compilazione del campo deve osservare la seguente sintassi:
> * -i componimenti di Rvf sono rappresentati dal numero d’ordine secondo la redazione definitiva; 
> * -una sequenza di componimenti di Rvf può essere espressa attraverso i suoi estremi separati da trattino orizzontale (“-”); 
> * -eventuali Disperse sono indicate dal numero d’ordine secondo la silloge di Solerti seguito da “d”; 
> * -testi dei Rvf trasmessi in redazioni precedenti a quella definitiva sono indicati dal loro numero d’ordine nei Rvf seguito da “a”; 
> * -ogni elemento o intervallo di elementi è separato da spazio.   

Una volta inserita la sequenza dei componimenti, cliccare il comando _add_ alla destra del campo.   
> ![](/docs/assets/images/sheelabels_add.png)  

Al di sotto del campo comparirà l'elenco dei componimenti inseriti.  

Una volta inserita la sequenza, è possibile eventualmente aggiungere altri componimenti o intervalli di componimenti attraverso il campo _ranges_. Tali componimenti saranno aggiunti in coda alla sequenza già inserita.

Dall'elenco dei componimenti inseriti è possibile:
* eliminare singoli componimenti o intervalli mediante il comando _delete_;  
> ![](/docs/assets/images/sheelabels_delselectedcol.png)  

* modificarne l'ordine relativo mediante i comandi _move up_/_move down_.
> ![](/docs/assets/images/moveup_down.png)

Qualora lo si ritenga preferibile, è possibile procedere inserendo i componimenti e gli intervalli uno per volta nel campo _ranges_, ripetendo ogni volta l'operazione di aggiunta mediante il comando _add_.

Il comando _delete all ranges_ permette di eliminare l'intera sequenza inserita. 
> ![](/docs/assets/images/sheelabels_trimtablerows.png)

La compilazione del campo è obbligatoria.
  
## Layouts 
Permette di indicare la tipologia di impaginazione dei componimenti.

Nella sezione vengono visualizzate celle numerate corrispondenti a ciascun componimento, secondo la selezione e l'ordine indicati precedentemente.

Il campo **layout** permette di indicare attraverso il tipo di impaginazione dei componimenti:

* \---
* 1 colonna
* 2 colonne
  * 2 colonne - verticale
  * 2 colonne - orizzontale 
    * 2 colonne - or. interc. fisso
    * 2 colonne - or. interc. mobile
* prosa 

⚠️ Utilizzare sempre il valore più specifico (ad es. non "2 colonne" ma "2 colonne - verticale"; non "2 colonne - orizzontale" ma "2 colonne - or. interc. fisso").  

Per attribuire una tipologia di impaginazione, occorre selezionare i relativi componimenti.  

La **selezione** dei componimenti può essere effettuata secondo diverse modalità:

* per selezionare tutti i componimenti, utilizzare il comando _select all_;  
> ![](/docs/assets/images/editor_selectall.png)  
* per selezionare un singolo componimento, utilizzare il comando _select this layout_, presente all'interno di ogni singola cella;  
> ![](/docs/assets/images/ranges_selectcella.png)  
* per selezionare un intervallo continuo di componimenti, tenendo premuto il tasto _shift_, selezionare la prima e l'ultima cella dell'intervallo;
* per selezionare una serie discontinua di componimenti, tenendo premuto il tasto _ctrl_, selezionare le relative celle;
* per selezionare i componimenti in base al genere metrico (sonetto, canzone, ballata, madrigale, sestina), selezionare dal campo _presets_, attraverso menu a tendina, il genere metrico desiderato;
* per deselezionare tutti i componimenti, utilizzare il comando _deselect all_;   
> ![](/docs/assets/images/editor_selectall.png)   
* per deselezionare un singolo componimento, utilizzare il comando _clear this layout_, presente all'interno di ogni singola cella.  
> ![](/docs/assets/images/ranges_clearcella.png)  

Per l' **attribuzione** di un tipo di impaginazione al componimento o ai componimenti selezionati, scegliere un'opzione dal thesaurus _layout_.  
Ad ogni selezione può essere attribuito un solo _layout_; se il testimone presenta più tipologie di impaginazione, è necessario ripetere la procedura di selezione e attribuzione più volte.  
⚠️ Dopo ogni attribuzione della tipologia di impaginazione alla selezione di componimenti, è necessario deselezionare tutti i componimenti prima di procedere a una nuova selezione.  

Per **eliminare** tutte le impaginazioni inserite, selezionare tutti i componimenti attraverso il comando _select all_ e scegliere l'opzione "---" dal thesaurus di _layout_.

È possibile aggiungere un **nota** relativa all'impaginazione di un singolo componimento attraverso il comando _edit_, presente all'interno delle celle (ad es. se l'impaginazione cambia all'interno di un singolo componimento).  
> ![](/docs/assets/images/ranges_editcella.png)   

La compilazione della sezione _layouts_ è obbligatoria per le descrizioni analitiche.


## Note

### Tag
Permette di indicare se la coincidenza tra fine componimento e fine pagina è:
* rispettata
* tendenzialmente rispettata
* non rispettata

La compilazione del campo è obbligatoria per le descrizioni analitiche.

### Note
Permette di fornire informazioni aggiuntive rispetto ai dati inseriti nella parte (ad es. per segnalare l’inserimento di materiale non petrarchesco o di poesie di corrispondenti all’interno della sequenza di testi dei Rvf; la presenza di lacune all'interno di singoli componimenti; l’eventuale dipendenza dell’ordine attuale dei componimenti da guasti materiali del codice, etc).

La compilazione del campo è facoltativa.

## Save ⚠️ 

Cliccare sul comando **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul comando **_Close_** per tornare alla schermata di riepilogo dell'item.
