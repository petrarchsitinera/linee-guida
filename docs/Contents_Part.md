# Contents Part
**Contents Part** permette di fornire la descrizione interna, elencando le opere nella successione attestata dal manoscritto. 

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codcontentspart).

Per aggiungere la parte, selezionare **_contents_** dal menu a tendina, quindi cliccare su **_add part_**. 

## Content 
Per ogni testo è creato un elemento _content_ mediante un [editor](Editor_Brick.md).

⚠️  L'elemento _content_ è utilizzato anche per indicare le carte bianche presenti nel manoscritto. In questo caso nell'elemento sono compilati solo i campi obbligatori: _range_, con l'indicazione della carta; _title_, con il valore "-".

⚠️  Il contenuto di ampie miscellanee, in cui una chiara individuazione interna delle opere risulti troppo onerosa, è indicato da un titolo generale (nel campo _title_), ad es. "antologia poetica", "miscellanea religiosa". Ove sia possibile specificare determinate partizioni (es. sezioni d'autore in miscellanee poetiche), è possibile indicarle nella sezione _Annotations_.

### Eid
Permette di attribuire o richiamare l'identificativo del testo.  
Se il testo è schedato all'interno di Itinera, cercare l'item relativo e copiarne [l'_eid_](identifiers.md), servendosi eventualmente dei [repository](repository.md) e della funzione di [lookup](lookup.md). 
Se il testo non è schedato all'interno di Itinera, lasciare vuoto.  

### Range
Permette di indicare l'intervallo o gli intervalli di carte su cui è trascritto il testo secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

### Tag
🚧 Permette di inserire un'etichetta utile ai fini della ricerca.  
La compilazione del campo è facoltativa.

### Author Id 
Permette di indicare il nome dell'autore dell'opera.  

⚠️ Per determinare la forma del nome dell'autore consultare l'authority file all'indirizzo: 🚧  

Se l'autore non è presente nell'authority file, seguire queste convenzioni:  

> I nomi d’autore del testo sono espressi in forma normalizzata. I nomi degli autori fino al sec. XII sono dati in italiano e in forma breve (Cicerone e non M. Tullio Cicerone); si specifica ulteriormente solo per possibili omonimi (Lattanzio Placido vs. Lattanzio Firmiano); dopo il sec. XII i nomi degli autori sono dati in lingua originale normalizzata; inoltre, il nome dell’autore non deve essere mai accompagnato dalla qualifica di ‘santo’ (Agostino e non Sant’Agostino) e nei casi di omonimia la distinzione è data dalla provenienza (Agostino di Canterbury). 

La compilazione del campo è facoltativa.

### Claimed Author
Permette di inserire l'indicazione d'autore quale è fornita dal testimone, nel caso diverga dall'attribuzione accettata. Il nome è espresso in forma normalizzata.  
La compilazione del campo è facoltativa.

### Title
Permette di indicare il titolo dell'opera.

⚠️ Per determinare la forma del titolo consultare l'authority file all'indirizzo: 🚧  

Se l'opera non è presente nell'authority file, seguire queste convenzioni:  


> I titoli sono dati nella lingua del testo: 🏃 dunque, in latino se il testo è in latino (anche in caso di traduzioni), in italiano o altro volgare se il testo è in italiano o altro volgare (anche in caso di traduzioni). I titoli in volgare si danno sempre senza articolo. Nel caso di opere non identificate, trascrivere il titolo presente nel ms. o, se assente, elaborare un titolo e segnalarlo tra parentesi quadre, es. “[Raccolta di testi astrologici]” 🏃 .

La compilazione del campo è obbligatoria.

### Claimed Title
Permette di indicare il titolo così come è fornito dal testimone, nel caso diverga da quello corrennte.   
La compilazione del campo è facoltativa.

### Location
Permette di precisare la porzione dell'opera trasmessa dal testimone, qualora essa sia suddivisa in partizioni note (capitolo, libro, numero di componimento, etc.; 🚧 aggiungere foto di esempio). 
La compilazione del campo è facoltativa.

### Note
Permette di inserire informazioni che non è possibile esprimere nel modello, come ad es. note filologiche relative al testimone, informazioni sulla patina linguistica, informazioni cronologiche, etc.  
La compilazione del campo è facoltativa.

### Incipit
Permette di registrare l'incipit dell'opera quale è espresso nel testimone, in forma diplomatica.  
La compilazione del campo è facoltativa.

### Explicit
Permette di registrare l'explicit dell'opera quale è espresso nel testimone, in forma diplomatica.  
La compilazione del campo è facoltativa.

### States
Permette di indicare la presenza di eventuali anomalie del testimone dipendenti da cause meccaniche, da difetti della tradizione o da scelte del copista. Selezionare uno o più valori tra:
* acefalo (testo privo dell’inizio)
* mutilo (testo privo della fine)
* lacunoso (testo con mancanze interne dovute a cause meccaniche)
* interrotto (testo la cui trascrizione è rimasta in sospeso)
* incompleto (testo con mancanze non imputabili a cause meccaniche)
* estratti (sezioni di un testo accorpate e trascritte con intento antologico o come citazioni)

La compilazione del campo è facoltativa.

### Annotation
Permette di indicare, descrivere e trascrivere singole partizioni testuali o paratestuali significative. Può essere utilizzato per registrare prefazioni, argomenti, rubriche, testi di dedica, etc.  
Se il contenuto descritto consiste in una silloge di poesie di uno o di più autori, è possibile indicare in questa sezione le suddivisioni ad essa pertinenti (per autore, per genere, etc.).

⚠️ Per i Rvf si segnalano in questa sede eventuali indici o tavole dei contenuti attribuibili al progetto originale di confezione del codice. Se aggiunti successivamente, saranno menzionati nella sezione History.

Per ogni partizione testuale è creato un elemento _annotation_ mediante un [editor](Editor_Brick.md).

La compilazione della sezione è facoltativa. 

⚠️ Per ogni elemento _annotation_ inserito è necessario salvare cliccando sul tasto di spunta blu.

#### Type
Permette di indicare la tipologia della partizione testuale. Selezionare un valore tra: 

* -
* rubrica
* prefazione
* dedica
* capitolo
* altro

La compilazione del campo è obbligatoria.

#### Range
Permette di indicare l'intervallo di carte su cui è trascritto l'elemento secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

#### Incipit
Permette di registrare l'incipit della partizione testuale, in forma diplomatica.  
La compilazione del campo è obbligatoria.

#### Explicit
Permette di registrare l'explicit della partizione testuale, in forma diplomatica.  
La compilazione del campo è obbligatoria.

#### Text
Permette di trascrivere per intero o parzialmente il contenuto della partizione testuale.  
La compilazione del campo è obbligatoria.


## Save ⚠️ 

Per ogni elemento _content_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
