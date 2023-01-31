# Layouts Part

**Layouts Part** raccoglie le indicazioni relative alle dimensioni e allo schema di impaginato. Nel caso di manoscritti compositi o caratterizzati da più schemi di impaginato è possibile creare più elementi Layout.

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codlayoutspart).

Per aggiungere la parte, selezionare **_layouts_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Layout
Per ogni schema di impaginato è creato un elemento _layout_ mediante un [editor](Editor_Brick.md).

### Tag
Permette di attribuire all'elemento un'etichetta utile ai fine della ricerca.  
⚠️ Se lo schema di impaginato include o coincide con la sezione dedicata ai _Rerum vulgarium fragmenta_ utilizzare il tag "RVF". Negli altri casi la compilazione del campo è facoltativa.

### Sample
Permette di indicare la carta sulla quale è effettuata la rilevazione dello schema di impaginato, secondo il modello [Cod Location](Cod_Location_Brick.md). Di norma è preso a riferimento il recto della seconda carta del foglio centrale del secondo fascicolo.

La compilazione del campo è obbligatoria.

### Ranges
Permette di indicare l'intervallo di carte che presentano lo schema di impaginato descritto, secondo il modello [Cod Location](Cod_Location_Brick.md).

La compilazione del campo è obbligatoria.

### Ruling
Permette di indicare la tecnica di rigatura utilizzata per tracciare lo schema di impaginato. Selezionare un valore tra:
* --- (non individuabile)
* a secco
* a colore
* a mina di piombo
* a inchiostro
* per piegatura
* altro

La compilazione del campo è facoltativa.

### Derolez
Permette di indicare il numero dello schema di rigatura secondo il repertorio Derolez.

La compilazione del campo è facoltativa.

### Pricking
Permette di indicare, mediante una stringa di testo libero, la tecnica di foratura, se presente.

La compilazione del campo è facoltativa.

### Cols
Permette di indicare il numero delle colonne.  
⚠️ Se non è possibile identificare la distribuzione del testo su una o più colonne compilare il campo con il valore “0”.  

La compilazione del campo è obbligatoria.

### Count
Permette di inserire il numero di linee e di righe della pagina. 

Per creare un nuovo elemento cliccare _+add count_. Ogni _count_ è provvisto di: 
* _ID_: selezionare "righe" o "linee";
* _value_: indicare il valore misurato; 
* _tag_: permette di inserire un'etichetta utile ai fini della ricerca;
* _note_: permette di aggiungere eventuali annotazioni.  


Si registrano di norma i valori riscontrati sulla carta _sample_.  
Se tali valori non sono rappresentativi della prassi osservata dal copista nel _range_ di carte del _layout_ in oggetto (perché ad esempio le righe finali della carta _sample_ sono lasciate vuote dopo la fine di un testo), è necessario creare ulteriori elementi _count_ con _ID_ "righe" o "linee" per esprimere il numero di righe o di linee generalmente utilizzate per quel _layout_, aggiungendo a questi valori il _tag_ "prevalente".  
Per layout fortemente irregolari è possibile inserire, oltre ai valori riscontrati sulla carta _sample_, i valori corrispondenti al numero di linee e righe minimo e massimo, aggiungendovi i tag "max" o "min"; è altresì possibile, per semplicità, segnalare l'irregolarità nel campo _note_ dei singoli valori.  

La compilazione del campo è facoltativa, ma fortemente raccomandata.

### Layout formula
Permette di esprimere le dimensioni della pagina e dello specchio di scrittura secondo le convenzioni correnti. Tutte le misure, rilevate nella carta _sample_, sono espresse in millimetri; le misure dell’altezza sono rilevate lungo la giustificazione interna, quelle della larghezza lungo la rettrice di testa; per una corretta misurazione è opportuno non spostare lo strumento, ma rilevare le scansioni interne, procedendo per sottrazione.

La formula è introdotta dalle misure dell’altezza moltiplicata per la larghezza, seguite dal segno di uguale; seguono, divise dal segno di moltiplicazione, la sezione delle misure relative all’altezza e la sezione delle misure relative alla larghezza, le cui somme devono coincidere con quelle dell’altezza e della larghezza complessive; le misure relative allo specchio di scrittura sono posizionate all’interno di parentesi quadre, quelle relative ai margini non scritti all’esterno; la presenza di colonnini è indicata da barre oblique “/”, a seconda che questi contengano o meno scrittura, sono situati all’interno o all’esterno delle parentesi quadre; nei manoscritti a due colonne l’intercolumnio è indicato all’interno delle parentesi quadre, racchiuso tra parentesi tonde; eventuali colonnini non scritti figurano all’interno delle parentesi quadre ma sono segnalati da asterisco.

Si dà la seguente formula esemplificativa, dove sono espressi tutti valori possibili di una carta impaginata su due colonne (i valori sottolineati sono alternativi, quelli in grassetto obbligatori):

> “**240** × **150** = **30** / <u>5 [ 5</u>/ **170** / <u>5] 5</u>/ **40** × **15** / <u>5 [5</u> / **50** / 5<u>\*</u> (20) 5<u>\*</u> / 40 / <u>5] 5</u> / **15**”  
>     - “240 × 150 =”: altezza e larghezza della pagina;  
>      - “30 / 5 [ 5/ 170 / 5] 5/ 40”: misure relative all’altezza, ove:  
>              - “30” rappresenta il valore del margine superiore, obbligatorio;   
>              - “/5” e “[5/”, non obbligatori e alternativi, indicano la riga di testa, vuota o con scrittura;   
>              - “170” indica lo specchio di scrittura, obbligatorio;   
>              - “/5]” e “5/”, non obbligatori e alternativi, indicano la riga di piede, vuota o con scrittura;   
>              - “40” indica il margine inferiore, obbligatorio;  
>       - “15 / 5 [5 / 50 / 5* (20) 5* / 40 / 5] 5 / 15”: misure relative alla larghezza, ove:   
>              - “15” indica il margine sinistro, obbligatorio;   
>              - “/5” e “[5/”, non obbligatori e alternativi, indicano il colonnino sinistro, vuoto o con scrittura;   
>              - “50” indica lo specchio di scrittura dell’unica colonna o della prima colonna in manoscritto a due colonne, obbligatorio;   
>              - “/ 5” o “/ 5*”, non obbligatori e alternativi, indicano il colonnino sinistro, con scrittura o vuoto;   
>              - “(20)” indica l’intercolumnio in un manoscritto a due colonne;   
>              - “5/” o “5*/” , non obbligatori e alternativi, indicano il colonnino sinistro della seconda colonna, con scrittura o vuoto;   
>              - “40” indica lo specchio di scrittura della seconda colonna;   
>              - “/5]” e “5/”, non obbligatori e alternativi, indicano il colonnino destro della seconda colonna, con scrittura o vuoto;   
>              - “15” indica il margine destro, obbligatorio.


Una volta inserita la formula è necessario cliccare sul tasto di spunta blu _apply formula_. 
> ![](/docs/assets/images/layout_applyfor.png)   

Tutti i valori inseriti compariranno in _dimensions_ sotto i rispettivi ID.

La compilazione del campo è obbligatoria. Ove la sintassi non sia rispettata, non risulterà possibile validare la formula.

### Figure
Permette di visualizzare graficamente lo schema di impaginato inserito attraverso _layout formula_.

### Dimensions 
La sezione viene compilata automaticamente attraverso l'inserimento di _layout formula_: gli _ID_ sono creati automaticamente e l’unità di misura è espressa in millimetri. 

Ogni elemento _dimension_ è provvisto di: 
* _ID_: identificativo della dimensione misurata, automaticamente determinato in base alla sintassi della formula; 
* _value_: valore misurato; 
* _unit_: unità di misura prescelta, automaticamente impostata come “mm”. 

È possibile modificare il valore dei singoli elementi ed aggiornare conseguentemente la formula cliccando, all’interno del campo _layout formula_, il tasto _update formula_.  
> ![](/docs/assets/images/layout_updatefor.png)


### Note
Permette di inserire, in forma di testo libero, eventuali precisazioni relative ad irregolarità nello schema di impaginato.

La compilazione del campo è facoltativa.

## Save ⚠️ 

Per ogni elemento _layout_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
