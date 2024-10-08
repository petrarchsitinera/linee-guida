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
* altro (rigature miste; cfr. _Note_)

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

### Layout formula
Permette di esprimere le dimensioni della pagina e dello specchio di scrittura secondo le convenzioni correnti. Tutte le misure, rilevate nella carta _sample_, sono espresse in millimetri; le misure dell’altezza sono rilevate lungo la riga di giustificazione interna, quelle della larghezza lungo la rettrice di testa; per una corretta misurazione è opportuno non spostare lo strumento, ma rilevare le scansioni interne, procedendo per sottrazione.

La formula è introdotta dalle misure di altezza per (x) larghezza, seguite dal segno di uguale (=); seguono, divise dal segno di moltiplicazione, la sezione delle misure relative all’altezza e la sezione delle misure relative alla larghezza, le cui somme devono coincidere con quelle dell’altezza e della larghezza complessive.  
Le misure relative allo specchio di scrittura sono posizionate all’interno di parentesi quadre, quelle relative ai margini non scritti all’esterno delle parentesi.  
La presenza di colonnini è indicata da barre oblique “/”; a seconda che questi contengano o meno scrittura, sono situati all’interno o all’esterno delle parentesi quadre.  
Nei manoscritti a due colonne, tra partentesi quadre vanno incluse, nell'ordine: lo specchio di scrittura della prima colonna, l’intercolumnio tra parentesi tonde, lo specchio di scrittura della seconda colonna; eventuali colonnini interni non scritti figurano all’interno delle parentesi quadre ma sono segnalati da asterisco.  

Si dà la seguente formula esemplificativa, dove sono espressi tutti valori possibili di una carta impaginata su due colonne (i valori sottolineati sono alternativi, quelli in grassetto obbligatori):

> **240** × **150** = **30** / <ins>5 [ 5</ins>/ **170** / <ins>5] 5</ins>/ **40** × **15** / <ins>5 [5</ins> / **50** / 5<ins>\*</ins> (20) 5<ins>\*</ins> / 40 / <ins>5] 5</ins> / **15**  
> 
> 240 × 150 =: altezza e larghezza della pagina, valori obbligatori;  
> 
> 30 / 5 \[5/ 170 / 5] 5/ 40: misure relative all’altezza, ove:   
>              - 30: margine superiore, valore obbligatorio;   
>              - /5 e \[5/: riga di testa vuota o riga di testa con scrittura, valori non obbligatori e alternativi tra loro;   
>              - 170: specchio di scrittura, valore obbligatorio;   
>              - /5] e 5/: riga di piede con scrittura o riga di piede vuota, valori non obbligatori e alternativi tra loro;   
>              - 40: margine inferiore, valore obbligatorio;  
>              
> 15 / 5 \[5 / 50 / 5* (20) 5* / 40 / 5] 5 / 15: misure relative alla larghezza, ove:   
>              - 15: margine sinistro, valore obbligatorio;   
>              - /5 e \[5/: colonnino sinistro vuoto o colonnino sinistro con scrittura, valori non obbligatori e alternativi tra loro;   
>              - 50: specchio di scrittura dell’unica colonna o della prima colonna in manoscritto a due colonne, valore obbligatorio;   
>              - / 5 o / 5*: colonnino destro della prima colonna, con scrittura o vuoto, valori non obbligatori e alternativi tra loro;   
>              - (20): intercolumnio, valore obbligatorio in un manoscritto a due colonne;   
>              - 5 / o 5* /: colonnino sinistro della seconda colonna, con scrittura o vuoto, valori non obbligatori e alternativi tra loro;   
>              - 40: specchio di scrittura della seconda colonna, valore obbligatorio in un manoscritto a due colonne;     
>              - /5] e 5/: colonnino destro della seconda o unica colonna, con scrittura o vuoto, valori non obbligatori e alternativi tra loro;   
>              - 15: margine destro, valore obbligatorio.


Una volta inserita la formula è necessario cliccare sul tasto di spunta blu _apply formula_. 
> ![](https://github.com/petrarchsitinera/linee-guida/blob/1a94390ee30ce0a5b737f4b1fd4dabbf453c4c06/docs/assets/images/layout_applyfor.png?raw=true)   

Tutti i valori inseriti compariranno in _dimensions_ sotto i rispettivi ID.

⚠️ Nel caso di _mise en page_ con assenza di margini, i relativi valori obbligatori andranno compilati con "0", come nell'esempio:
> 250 x 160 = 0 [250] 0 x 0 [160] 0  

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
> ![](https://github.com/petrarchsitinera/linee-guida/blob/1a94390ee30ce0a5b737f4b1fd4dabbf453c4c06/docs/assets/images/layout_updatefor.png?raw=true)

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
⚠️ Per le schede sintetiche è possibile limitarsi ad indicare il numero di righe riscontrato sulla carta _sample_ e, in caso di variabilità, aggiungere il _tag_ "var".

La compilazione del campo è facoltativa, ma fortemente raccomandata.

### Note
Permette di inserire, in forma di testo libero, eventuali precisazioni relative ad irregolarità nello schema di impaginato.  
In questa sezione è possibile precisare le diverse tipologie di rigatura utilizzate, se il sistema è misto.  

La compilazione del campo è facoltativa.

## Save ⚠️ 

Per ogni elemento _layout_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
