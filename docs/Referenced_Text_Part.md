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
Compilare con l'identificativo del testo da inserire (testo di proposta o testo citato).    
Per individuare l'identificativo ([_eid_](identifiers.md)) dei testi che fanno parte dei _corpora_ di Itinera,  consultare i [repository](repository.md) o ricorrere alla funzione di [lookup](lookup.md).   
Se, diversamente, il testo non fa parte dei _corpora_ di Itinera, attribuire un _eid_ secondo le regole [per la composizione di nuovi _eid_](identifiers.md#regole-di-composizione-di-nuovi-eid) e segnalare l'aggiunta su clickup per permettere l'aggiornamento dei [repository](repository.md).  

La compilazione del campo è **obbligatoria**.

### Target citation
Il campo è riservato **esclusivamente** ai testi citati (_type_ = "citazione di").    
Compilare con il luogo del testo citato da cui è tratta la citazione, espresso indicando il libro e/o il paragrafo e/o il verso, non separati da virgole. Se si tratta di un intervallo, separare i numeri di paragrafo o di versi con un trattino.
 > Es.:  
 > XII 4 3  
 > I 1 65-68  

La compilazione del campo è obbligatoria per i testi citati (_type_ = "citazione di").

### Source
Il campo è riservato **esclusivamente** ai testi citati (_type_ = "citazione di").  
Compilare con il luogo del testo schedato in cui si trova la citazione, espresso indicando il libro e/o il paragrafo e/o il verso, non separati da virgole. Se si tratta di un intervallo, separare i numeri di paragrafo o di versi con un trattino.   

La compilazione del campo è obbligatoria per i testi citati (_type_ = "citazione di").

### Assertion
Permette di indicare l'attendibilità del collegamento inserito ed eventuali fonti. Per la compilazione del campo, consultare le istruzioni di [Assertion](Assertion_Brick.md).  

## Save ⚠️ 
Per ogni elemento _text_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
