# Referenced Text Part

**Referenced Text Part** permette di registrare:  
* il testo al quale il testo schedato risponde - per le lettere e per le tenzoni poetiche;  
* i testi citati nel testo schedato.

⚠️ Per i testi di corrispondenza, si registrano in questa parte i soli testi di proposta, collegati cioè come antecedenti al testo schedato nella catena di corrispondenza. **Non si registrano dunque eventuali risposte al testo schedato**. La catena di corrispondenza sarà ricostruita a posteriori automaticamente sul grafo semantico.  

⚠️ La parte raccoglie soltanto le citazioni di testi, opere o lettere scritti da: **Petrarca, suoi corrispondenti, corrispondenti di corrispondenti, altri autori contemporanei**. Non vanno dunque registrate eventuali citazioni di testi, opere, lettere di altri autori, come per esempio i classici.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#referencedtextspart).

Per aggiungere la parte, selezionare **_ref-texts_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Text
Per ogni testo da inserire si crea un elemento _text_ mediante [editor](Editor_Brick.md).  

### Type
Permette di specificare il tipo di relazione che il testo schedato intrattiene con l'elemento _text_ inserito:  
* risposta a: quando il _text_ inserito è la proposta del testo schedato;  
* citazione di: quando il _text_ inserito è citato nel testo schedato.  

La compilazione del campo è **obbligatoria**.

### Target ID
Permette di indicare l'identificativo del testo da inserire (testo di proposta o testo citato), secondo il modello [Asserted Id](Asserted_Ids_Brick.md).  
Per individuare [l'_eid_](identifiers.md) di un testo schedato in Itinera, controllare sempre il [repository dei testi](repository.md).  
Se il testo è schedato come Item Text all'interno della banca dati, esso è conseguentemente provvisto di un [_eid_](identifiers.md). È possibile dunque cercare e richiamare l'_eid_ attraverso lo strumento di ricerca integrato in [Asserted Id](Asserted_Ids_Brick.md#target).  
Nel caso in cui al testo da inserire non sia già attribuito un _eid_, il compilatore dovrà selezionare il [flag _external_](Asserted_Ids_Brick.md#altri-identificativi-itinera), procedere all'assegnazione di un nuovo _eid_ seguendo le istruzioni indicate [qui](identifiers.md) e segnalarla su [Clickup](https://clickup.com/) per permettere l'aggiornamento del [repository](repository.md).  

La compilazione del campo è **obbligatoria**.

### Target citation
Il campo è riservato **esclusivamente** ai casi in cui si stia inserendo un testo citato (_type_ = "citazione di"), e occorra indicare la partizione esatta del testo citato. 

Compilare con il luogo del testo citato da cui è tratta la citazione, espresso indicando:

- il paragrafo e/o il verso, non separati da virgole, per i testi petrarcheschi citati di cui il precedente **Id** fornisca già numero di libro e numero d'ordine.

> ⚠️ Se nel _target Id_ è stata inserita una _Familiare_, di cui l'**id** fornisce **già** numero di libro e numero d'ordine, nella _target citation_ si inserisce soltanto il numero di paragrafo eventualmente citato.
> Es.:   
> [Target Id = Fam. XI 1] 12  

  
- il libro e/o il paragrafo e/o il verso, non separati da virgole in tutti gli altri casi. Se si tratta di un intervallo, separare i numeri di paragrafo o di versi con un trattino.
  
 > Es.:  
 > [Target Id = Amor et dolor] 3  
 > [Target Id = Africa] I 65-68  

La compilazione del campo è obbligatoria per i testi citati (_type_ = "citazione di").

### Source
Il campo è riservato **esclusivamente** ai casi in cui si stia inserendo un testo citato (_type_ = "citazione di").  

Compilare con il luogo del testo schedato in cui si trova la citazione, espresso indicando il paragrafo e/o il verso, non separati da virgole. Se si tratta di un intervallo, separare i numeri di paragrafo o di versi con un trattino.   

La compilazione del campo è obbligatoria per i testi citati (_type_ = "citazione di").

### Assertion
Permette di indicare l'attendibilità del collegamento inserito ed eventuali fonti. Per la compilazione del campo, consultare le istruzioni di [Assertion](Assertion_Brick.md).  

## Save ⚠️ 
Per ogni elemento _text_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
