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

[INSERIRE ESEMPIO SCREENSHOT]

Una volta inserita la sequenza dei componimenti, cliccare il comando _add_ [ICONA] alla destra del campo.  
Al di sotto del campo comparirà l'elenco dei componimenti inseriti.  

[INSERIRE STESSO ESEMPIO SCREENSHOT]

Una volta inserita la sequenza, è possibile eventualmente aggiungere altri componimenti o intervalli di componimenti attraverso il campo _ranges_. Tali componimenti saranno aggiunti in coda alla sequenza già inserita.

Dall'elenco dei componimenti inseriti è possibile, attraverso l' [editor](Editor_Brick.md), eliminare singoli componimenti o intervalli mediante il comando _delete_ [ICONA], oppure modificarne l'ordine relativo mediante i comandi _move up_/_move down_ [ICONE].

Qualora lo si ritenga preferibile, è possibile procedere inserendo i componimenti e gli intervalli uno per volta nel campo _ranges_, ripetendo ogni volta l'operazione di aggiunta mediante il comando _add_ [ICONA].

Il comando _delete all ranges_ [ICONA] permette di eliminare l'intera sequenza inserita.

La compilazione del campo è obbligatoria.
  
## Layouts 🚧 [VERIFICARE MODIFICHE DANIELE = 🌵]
Permette di indicare la tipologia di impaginazione dei componimenti.

Nella sezione vengono visualizzate celle numerate corrispondenti a ciascun componimento, secondo la selezione e l'ordine indicati precedentemente.

Il campo **layout** permette di indicare attraverso un 🌵 thesaurus gerarchico 🌵 il tipo di impaginazione dei componimenti:

🌵 
* \---
* 1 colonna
* 2 colonne
  * verticale
  * orizzontale
    * intercolumnio fisso
    * intercolumnio mobile
* prosa
🌵 

Per attribuire una tipologia di impaginazione, occorre selezionare i relativi componimenti.  

La **selezione** dei componimenti può essere effettuata secondo diverse modalità:

* per selezionare tutti i componimenti, utilizzare il comando_select all_ [ICONA];
* per selezionare un singolo componimento, utilizzare il comando_select this layout_ [ICONA], presente all'interno di ogni singola cella;
* per selezionare un intervallo continuo di componimenti, tenendo premuto il tasto _shift_, selezionare la prima e l'ultima cella dell'intervallo;
* per selezionare una serie discontinua di componimenti, tenendo premuto il tasto _ctrl_ [🌵 con Mac utilizzare il tasto XXX? 🌵], selezionare le relative celle;
* per selezionare i componimenti in base al genere metrico (sonetto, canzone, ballata, madrigale, sestina), selezionare dal campo _presets_, attraverso thesaurus, il genere metrico desiderato;
* per deselezionare tutti i componimenti, utilizzare il comando _deselect all_ [ICONA]; 
* per deselezionare un singolo componimento, utilizzare il comando _clear this layout_ [ICONA], presente all'interno di ogni singola cella.

Per l' **attribuzione** di un tipo di impaginazione al componimento o ai componimenti selezionati, scegliere un'opzione dal thesaurus _layout_.  
Ad ogni selezione può essere attribuito un solo _layout_; se il testimone presenta più tipologie di impaginazione, è necessario ripetere la procedura di selezione e attribuzione più volte.  
**Nb**. Dopo ogni attribuzione della tipologia di impaginazione alla selezione di componimenti, è necessario deselezionare tutti i componimenti prima di procedere a una nuova selezione.  

Per **eliminare** tutte le impaginazioni inserite, selezionare tutti i componimenti attraverso il comando _select all_ e scegliere l'opzione "---" dal thesaurus di _layout_.

È possibile aggiungere un **nota** relativa all'impaginazione di un singolo componimento attraverso il comando _edit_, presente all'interno delle celle (🚧 ad es. se l'impaginazione cambia all'interno di un singolo componimento).

La compilazione della sezione _layouts_ è obbligatoria per le descrizioni analitiche.


## Note

### Tag
Permette di indicare se la coincidenza tra fine componimento e fine pagina è:
* rispettata
* tendenzialmente rispettata
* non rispettata

La compilazione del campo è obbligatoria per le descrizioni analitiche.

### Note
Permette di fornire informazioni aggiuntive rispetto ai dati inseriti nella parte, 🚧 ad es. per l’inserimento di materiale non petrarchesco o di poesie di corrispondenti all’interno della sequenza di testi dei Rvf; la segnalazione di trascrizioni interrotte; l’eventuale dipendenza dell’ordine attuale dei componimenti da guasti materiali del codice, etc.

La compilazione del campo è facoltativa.

## Save ⚠️ 

Cliccare sul comando **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul comando **_Close_** per tornare alla schermata di riepilogo dell'item.
