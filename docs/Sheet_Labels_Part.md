# Sheet Labels Part

**Sheet Labels Part** permette di descrivere la consistenza del codice, le carte di guardia, la numerazione, la struttura fascicolare, i richiami e i sistemi di segnatura (fascicolare e a registro).  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codsheetlabelspart).

Per aggiungere la parte, selezionare **_sheet labels_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Labels 
La sezione permette di descrivere e rappresentare su una tabella le carte del codice e i relativi sistemi di numerazione e segnatura, nonché la struttura fascicolare.

L'interfaccia presenta due riquadri: _action_ e _adder_. In essi sono contenuti gli operatori che permettono di creare e modificare una tabella. Nella tabella le righe rappresentano le carte reali del manoscritto; le colonne rappresentano la fascicolazione e i sistemi di numerazione e segnatura.  

![Schermata iniziale](docs/assets/images/sheelabels_main.png)

docs/assets/images/sheelabels_main.png

Nel capitolo 'Comandi principali' sono descritte le modalità di funzionamento degli operatori contenuti nei riquadri _adder_ e _action_, e dei comandi interni alle celle della tabella.  
Nel capitolo 'Compilazione' sono illustrati i passaggi da seguire per la compilazione della tabella e per la descrizione di numerazione, fascicolazione, richiami, segnature.  


### Comandi principali

#### Adder
Permette di aggiungere righe e colonne alla tabella.  
Il campo _type_ permette di selezionare il tipo di elemento da aggiungere.   
Gli elementi si suddividono in _rows_ (righe) e _columns_ (colonne).  

Gli elementi di tipo _rows_ sono: _front cover, _front endleaf_, _body_, _back endleaf_, _back cover_.  
Per ogni elemento è possibile, attraverso il campo _count_, indicare il numero di righe da aggiungere.

Gli elementi di tipo _columns_ sono: _quire_, _numbering_, _catchword_, _signature_, _register_.   
Per ogni elemento è possibile, attraverso il campo _name_, attribuire un titolo alla rispetttiva colonna.

⚠️ Il comando _Trim table rows_ cancella le righe non compilate.  
⚠️ Il comando _Trim table rows and columns cancella righe e colonne non compilate.  

#### Action
Permette di selezionare una delle colonne create e di attribuire dei valori alle celle che la costituiscono; inoltre, permette di fornire una descrizione dell'elemento rappresentato dalla colonna.

È costituito da tre campi:

* _column_: permette di selezionare la colonna su cui si vuole intervenire; 
* _edit the selected column definition_: apre un editor che permette di fornire una descrizione dell'elemento prescelto;
* _action_: permette, attraverso una specifica formula, di attribuire dei valori alle celle della colonna.  

⚠️ Il comando _delete the selected column_ permette di eliminare l'intera colonna selezionata.

#### Celle
In ogni cella sono presenti due campi:

* _edit value_: permette di attribuire alla cella un valore;
* _edit note_: permette di aggiungere una nota relativa alla cella.


### Compilazione
Per la creazione e la compilazione della tabella si consiglia di procedere secondo l'ordine presentato di seguito, verificando ad ogni passaggio la correttezza delle informazioni inserite.  
In primo luogo è necessario creare le righe della tabella (_rows_): _body_ (obbligatorio); _front endleaves_ e _back endleaves_ (opzionale); _front cover_ e _back cover_ (opzionale).  
In seguito, è possibile creare le colonne (_columns_), a partire preferibilmente da _quires_ o _numberings_.

#### Rows
Per aggiungere righe alla tabella, utilizzare il riquadro _adder_.  
Il campo _type_ permette di selezionare il tipo di elemento desiderato: _body_, _front endleaf_ o _back endleaf_.  
Il campo _count_ permette di indicare il numero di righe da aggiungere per l'elemento selezionato.

##### Body
Permette di inserire le carte che compongono il corpo del manoscritto.  
Nel campo _type_ selezionare _body_; nel campo _count_ inserire il numero complessivo delle carte del corpo del manoscritto.  
Cliccando il comando _+ add_, viene creato un numero di righe pari al numero delle facciate (recto o verso) delle carte del corpo del manoscritto.  
Ad ogni riga è attribuita automaticamente un'etichetta costituita da un numero arabo progressivo seguito dall'indicazione r/v: 1r, 1v, 2r, 2v, etc..

##### Front endleaf
Permette di inserire le carte di guardia anteriori.  
Nel campo _type_ selezionare _front endleaf_; nel campo _count_ inserire il numero complessivo delle carte di guardia anteriori.  
Cliccando il comando _+ add_, viene creato un numero di righe pari al numero delle facciate (recto o verso) delle carte di guardia anteriori.  
Ad ogni riga è attribuita automaticamente un'etichetta costituita da un numero arabo progressivo seguito dall'indicazione r/v, tra parentesi tonde: (1r), (1v), (2r), (2v), etc. La numerazione standard in numeri romani andrà registrata sulla colonna _n_ (cfr. [Numbering](Sheet_Labels_Part.md#numbering)).   
Ulteriori informazioni relative alle carte di guardia potranno essere inserite nella sezione [Endleaves](Sheet_Labels_Part.md#endleaves).  

##### Back endleaf
Permette di inserire le carte di guardia posteriori.  
Nel campo _type_ selezionare _back endleaf_; nel campo _count_ inserire il numero complessivo delle carte di guardia posteriori.  
Cliccando il comando _+ add_, viene creato un numero di righe pari al numero delle facciate (recto o verso) delle carte di guardia posteriori.  
Ad ogni riga è attribuita automaticamente un'etichetta costituita da un numero arabo progressivo preceduto da /, seguito dall'indicazione r/v, tra parentesi tonde: (/1r), (/1v), (/2r), (/2v), etc. La numerazione standard in numeri romani andrà registrata sulla colonna _n_ (cfr. [Numbering](Sheet_Labels_Part.md#numbering)).    
Ulteriori informazioni relative alle carte di guardia potranno essere inserite nella sezione [Endleaves](Sheet_Labels_Part.md#endleaves).  

##### Front cover
Permette di inserire il piatto e il contropiatto anteriori.  
Nel campo _type_ selezionare _front cover_.  
Cliccando il comando _+ add_, vengono create due righe, una relativa al piatto anteriore ed una relativa al contropiatto anteriore, a cui sono attribuite rispettivamente le etichette [r] e [v]. Gli stessi valori andranno poi riportati sulla colonna _n_ (cfr. [Numbering](Sheet_Labels_Part.md#numbering)).      
La creazione di _front cover_ è necessaria qualora, in altre _parts_, si debbano descrivere elementi presenti sul piatto o sul contropiatto anteriori (es. note di possesso), richiamando la rispettiva [CodLocation](Cod_Location_Brick.md).   

##### Back cover
Permette di inserire il piatto e il contropiatto posteriori.  
Nel campo _type_ selezionare _back cover_.  
Cliccando il comando _+ add_, vengono create due righe, una relativa al piatto posteriore ed una relativa al contropiatto posteriore, a cui sono attribuite rispettivamente le etichette [/r] e [/v]. Gli stessi valori andranno poi riportati sulla colonna _n_ (cfr. [Numbering](Sheet_Labels_Part.md#numbering)).      
La creazione di _back cover_ è necessaria qualora, in altre _parts_, si debbano descrivere elementi presenti sul piatto o sul contropiatto posteriori (es. note di possesso), richiamando la rispettiva [CodLocation](Cod_Location_Brick.md).

#### Columns
Per aggiungere colonne alla tabella, utilizzare il riquadro _adder_.  
Il campo _type_ permette di selezionare il tipo di elemento desiderato: _quire_, _numbering_, _catchword_, _signature_, _register_.    
Il campo _name_ permette di attribuire un titolo alla colonna selezionata.

Per compilare le colonne create, utilizzare il riquadro _action_.  
Il campo _column_ permette di selezionare la colonna su cui si vuole intervenire.  
Il campo _edit the selected column definition_ apre un editor che permette di fornire una descrizione dell'elemento corrispondente alla colonna selezionata.
Il campo _action_ permette, attraverso una specifica formula, di attribuire dei valori alle celle della colonna selezionata. 

##### Quire 
Permette di creare e compilare una colonna relativa alla fascicolazione del manoscritto.  
È possibile creare un solo elemento del tipo _quire_.  

Per creare la colonna utilizzare i comandi del riquadro **_adder_**.
Nel campo _type_ selezionare _quire_; il campo _name_ non deve essere compilato.  
Cliccando il comando _+ add_, viene creata una colonna identificata dal titolo "q", deputata alla descrizione della struttura fascicolare del manoscritto.  

Per compilare la colonna utilizzare i comandi del riquadro **_action_**.
Nel campo _column_ selezionare "q".  
Il campo _edit the selected column definition_ non è attivo per _quire_.  
Il campo _action_ permette, attraverso una specifica formula, di attribuire dei valori alle celle della colonna selezionata.  
La formula consente di inserire in una sola volta fascicoli dello stesso tipo e consecutivi. Per serie di fascicoli di tipo diverso occorrerà ripetere l'operazione cambiando i relativi valori. Per serie molto irregolari o casi specifici, è possibile intervenire direttamente sulle singole celle (vedi oltre).

La **formula** deve rispettare la seguente sintassi: 
n1 x n2 = q n3 / n4  
* n1 = il numero della carta fisica, senza indicazione di recto o verso, da cui parte la fascicolazione che si intende inserire.   
* n2 = la quantità di fascicoli dello stesso tipo e consecutivi che si intende inserire; 
* q = operatore specifico per l'aggiunta dei fascicoli, da inserire sempre;
* n3 = il numero di fascicolo iniziale della serie che si intende inserire;
* n4 = il numero delle carte che compongono ogni fascicolo della serie che si intende inserire.  

> es. 1x2=q1/4 permette la creazione di due fascicoli di 4 carte a partire dalla prima carta fisica del corpo del codice:
>           -1: la fascicolazione parte dalla carta contrassegnata "1r" nella colonna relativa alla carte fisiche (colonna grigia a sinistra);  
>           -2: sono creati due fascicoli dello stesso tipo;  
>           -q1: il primo fascicolo della serie inserita è il fascicolo n. 1;  
>           -/4: sono creati fascicoli della consistenza di 4 carte.    

Dopo avere inserito la formula, cliccare il comando _Execute_.
L'applicazione della formula assegna alle celle interessate delle etichette, così strutturate:  
"n1.n2/n3"  
* n1 = numero di fascicolo;
* n2 = posizione della carta all'interno del fascicolo;
* n3 = consistenza del fascicolo.  
⚠️ Le etichette vengono ripetute identiche per il _recto_ e il _verso_ delle carte.  

> La formula dell'esempio precedente assegna alle carte 1-8 delle etichette, così strutturate:
> etichetta c. 1 = 1.1/4, ove:  
>          -1.: indica che la carta fa parte del fascicolo 1;  
>          -1/: indica che c. 1 è la prima carta del fascicolo 1;  
>          -4: indica che il fascicolo 1 è di 4 carte.  
> c. 2 sarà etichettata "1.2/4", c. 3 "1.3/4", c. 4 "1.4/4", c. 5 "2.1/4", c. 6 "2.2/4", etc.

>     Ulteriori esempi:  
>     es. 5x3=q2/8 permette la creazione di  trefascicoli di 8 carte a partire da c. 5
>     -5: la fascicolazione parte da carta 5;  
>     -3: sono creati tre fascicoli dello stesso tipo;  
>     -q2: il primo fascicolo della serie inserita è il fascicolo n. 2;    
>     -/8: sono creati fascicoli della consistenza di 8 carte;  
>     Questa formula assegna assegna alle celle delle carte 5-28 (24 carte totali) le seguenti etichette: c. 5 "2.1/8", c. 6 "2.2/8",..., c. 12 "2.8/8", c. 13 "3.1/8", ..., c. 20 "3.8/8", c. 21 "4.1/8", ..., c. 28 "4.8/8".  

⚠️ Per rappresentare un fascicolo a cui è stata aggiunta una carta, è necessario compilare manualmente l'etichetta della cella attraverso il suo campo _edit value_.  
Ad esempio, se il primo fascicolo è un quaderno con aggiunta di una carta (cc. 1-5), dopo aver inserito un quaderno regolare attraverso la formula (1x1=q1/4), occorrerà compilare il campo _edit value_ delle celle relative alle c. 5r e 5v con l'etichetta "1.5/4".  
È possibile segnalare quale sia la carta aggiunta utilizzando il campo _edit note_ della relativa cella, che andrà compilato con il segno "+".  

⚠️ Per rappresentare un fascicolo a cui è stata sottratta una carta, è necessario compilare manualmente l'etichetta della cella attraverso il suo campo _edit value_.  
Ad esempio, se il primo fascicolo è un quaderno con perdita di una carta (cc. 1-3), dopo aver inserito un quaderno regolare attraverso la formula (1x1=q1/4), occorrerà, attraverso il campo _edit value_ delle celle relative alle c. 4r e 4v, cancellare l'etichetta ("1.4/4") generata automaticamente dalla formula. In questo modo il fascicolo terminerà a c. 3 con l'etichetta "1.3/4".  
È possibile segnalare quale sia la carta caduta utilizzando il campo _edit note_ della cella della carta precedente (o della successiva se la caduta interessa la prima carta), che andrà compilato con il segno "-".  


##### Numbering
Permette di creare e compilare una o più colonne relative alla numerazione del manoscritto.  
È possibile infatti creare un elemento del tipo _numbering_ per ogni differente numerazione presente sul codice.   

Per creare la colonna utilizzare i comandi del riquadro **_adder_**.
Nel campo _type_ selezionare _numbering_.  
Il campo _name_ non deve essere compilato per la numerazione di riferimento.  
Cliccando il comando _+ add_, viene creata una colonna identificata dal titolo "n", deputata alla descrizione della numerazione di riferimento.  
⚠️ Tale numerazione sarà utilizzata ogni volta che nell' _item_ sarà compilato il campo [Cod Location](Cod_Location_Brick.md).  

Per tutte le altre numerazioni compilare il campo _name_ con un'etichetta convenzionale (es. "num2", "num.moderna").  
Cliccando il comando _+ add_, viene creata una colonna identificata dal titolo "n." seguito dall'etichetta scelta.  

Per compilare la colonna utilizzare i comandi del riquadro **_action_**.
Nel campo _column_ selezionare "n" (o "n.etichetta" per le numerazioni secondarie).  

Il campo _edit the selected column definition_ apre un **editor** che permette di descrivere alcune caratteristiche della numerazione attraverso i seguenti campi:
* _rank_: non compilare;
* _pagination_: spuntare nel caso di paginazione (e non di cartulazione);
* _system_: selezionare un valore tra: arabo; romano; arabo+romano (nel caso di valori espressi con uso di cifre arabiche e numeri romani: es. C20 per 120), misto (nel caso di numerazione che adotta su alcune carte il sistema arabo e su altre quello romano); altro;
* _technique_: selezionare un valore tra: inchiostro; lapis; n. meccanico; altro;
* _position_: selezionare un valore tra: marg. sup. est.; marg. sup. cen.; marg. sup. int.; marg. inf. est.; marg. inf. cen.; marg. inf. int.; intercol. sup.; intercol. inf.; altro;
* _colors_: selezionare un valore tra: bruno scuro, bruno chiaro, rosso, altro;
* _date_: permette di esprimere la datazione, secondo il modello [Asserted Date](Asserted_Chronotope_Brick.md);
* _note_: si raccolgono qui dati e informazioni che non è possibile inserire altrove, segnalando in particolare eventuali salti o errori nella numerazione.

⚠️ Dopo aver compilato la sottoparte, salvarla cliccando sul tasto di spunta blu.  

Il campo _action_ permette, attraverso una specifica formula, di attribuire dei valori alle celle della colonna selezionata.  
La formula consente di compilare rapidamente la colonna relativa a una numerazione permettendo l'inserimento automatico di serie continue (cifre arabiche, numeri romani, serie di lettere in ordine alfabetico).  
Per una numerazione regolare, senza interruzioni o errori, sarà sufficiente l'inserimento di un sola formula; per numerazioni irregolari sarà possibile ricorrere a inserimenti successivi e/o intervenire direttamente sulle singole celle.  

La **formula** per l'inserimento di una **cartulazione** deve rispettare la seguente sintassi:  
n1 * n2 = n3  
* n1 = il numero della carta fisica, senza indicazione di recto o verso, da cui parte la cartulazione che si intende inserire.  
* \* = comando preposto all'inserimento di una cartulazione.
* n2 = la quantità di carte consecutive interessate dalla cartulazione che si intende inserire.  
* n3 = il valore iniziale della serie che si intende inserire (arabo, romano o alfabetico).  

> es. 1\*10=1 permette la creazione di una cartulazione 1-10 a partire dalla prima carta fisica del corpo del codice:
>           -1: la cartulazione parte dalla carta contrassegnata "1r" nella colonna relativa alla carte fisiche (colonna grigia a sinistra);
>           -10: la cartulazione interessa 10 carte (20 caselle);  
>           -1: la cartulazione inizia con il valore "1", e prosegue automaticamente con le cifre arabiche successive.  
  
Dopo avere inserito la formula, cliccare il comando _Execute_.
L'applicazione della formula assegna alle celle interessate delle etichette corrispondenti alla cartulazione inserita, distinte automaticamente in _recto_ e _verso_.  

> La formula dell'esempio precedente assegna a partire dalla carta fisica "1r" i valori: 1r, 1v, 2r, 2v, ..., 10r, 10v.  

La **formula** per l'inserimento di una **paginazione** deve rispettare la seguente sintassi:  
n1r/v % n2 = n3  
* n1r/v = il numero della carta fisica, seguito dall'indicazione _r_ (recto) o _v_ (verso), da cui parte la paginazione che si intende inserire.  
* % = comando preposto all'inserimento di una paginazione.
* n2 = la quantità di facciate consecutive interessate dalla paginazione che si intende inserire.  
* n3 = il valore iniziale della serie che si intende inserire (arabo, romano o alfabetico).  

> es. 11v%4=XI permette la creazione di una paginazione XI-XIV a partire dalla carta fisica 11v:
>           -11v: la paginazione parte dalla carta contrassegnata "11v" nella colonna relativa alla carte fisiche (colonna grigia a sinistra);
>           -4: la paginazione interessa 4 facciate (4 caselle);  
>           -XI: la cartulazione inizia con il valore "XI", e prosegue automaticamente con i numeri romani successivi.  
  
Dopo avere inserito la formula, cliccare il comando _Execute_.
L'applicazione della formula assegna alle celle interessate delle etichette corrispondenti alla paginazione inserita. 

> La formula dell'esempio precedente assegna a partire dalla carta fisica "11v" i valori: 11v=XI, 12r=XII, 12v=XIII, 13r=XIV.  


È sempre possibile editare manualmente il valore di una cella cliccando sul suo campo _edit value_.  
Si ricorre a questa modalità di compilazione nel caso in cui:  
* i valori della numerazione presentino errori e discontinuità;
* la numerazione sia costituita da segni diversi da cifre arabiche, numeri romani, serie di lettere in ordine alfabetico:  
   * se la numerazione presenta un valore completamente arbitrario, il campo  deve essere compilato con il numero 0 seguito dal valore presente sul manoscritto riportato tra virgolette (es. 0"abc", 0"prima", etc.);
   * se la numerazione presenta un valore tipo '13bis', il campo deve essere compilato con il numero 13 seguito da "bis" riportato tra virgolette;
* una o più carte non siano numerate:
   * se in una cartulazione 1-3, c. 1 è numerata '1', c. 2 non è numerata, c. 3 è numerata '3', alla c. 2 è attribuita l'etichetta '2' e nel campo _edit note_ della cella è inserita l'annotazione 'non numerata'.  
   * se in una cartulazione 1-3, c. 1 è numerata '1', c. 2 non è numerata, c. 3 è numerata '2', alla c. 2 è attribuita l'etichetta 1"bis" e nel campo _edit note_ della cella è inserita l'annotazione 'non numerata'.  

⚠️ Sulla colonna relativa alla numerazione di riferimento (_n_) è necessario attribuire sempre, attraverso il campo _edit value_, valori predefiniti alle celle relative a:
* coperta e controcoperta anteriore (_front cover_): riportare i valori [r], [v];
* guardia anteriore (_front endleaf_): inserire numeri romani progressivi, seguiti da indicazione di recto o verso (es. Ir, Iv, IIr, IIv, ...);
* guardia posteriore (_back endleaf_): inserire numeri romani progressivi con apice, seguiti da indicazione di recto o verso (es. I'r, I'v, II'r, II'v, ...);
* coperta e controcoperta posteriore (_back cover_): riportare i valori [/r], [/v].  

⚠️ In presenza di due numerazioni complementari, e dunque nell'impossibilità di individuare una numerazione che possa fungere da riferimento per l'intera estensione del codice, è opportuno creare tre numerazioni:
* una numerazione 'n.etichetta1' per la prima numerazione, fornendone la descrizione nell'editor;
* una numerazione 'n.etichetta2' per la seconda numerazione, fornendone la descrizione nell'editor;
* una numerazione 'n' risultante dalla somma dei valori delle due numerazioni complementari, compilando i campi _system_, _technique_ e _position_ con il valore '\---'.  

> Questa soluzione può essere adottata in diversi casi, ad esempio:
> * una numerazione antica copre le cc. 1-50 e una numerazione moderna copre le cc. 51-100;  
> * una numerazione antica copre tutto il codice ma su alcune carte è stata integrata da numerazione moderna perché non visibile (a causa di rifilatura, inchiostro evanido, dimenticanza, etc.). Se non lo si ritiene opportuno (ad es. se il numero degli interventi moderni è molto ridotto), è possibile creare una sola numerazione (quella antica) e segnalare il fenomeno di integrazione nel campo _note_ dell'editor o nel campo _edit note_ delle singole celle.  


#### Catchword

Permette di creare e compilare una o più colonne relative al sistema di richiami presente sul manoscritto.  
È possibile infatti creare un elemento del tipo _chatchword_ per ogni differente tipologia di richiami presente sul codice.   

Per creare la colonna utilizzare i comandi del riquadro **_adder_**.
Nel campo _type_ selezionare _catchword_.  
Il campo _name_ può essere compilato con un'etichetta convenzionale (es. "rich-1", "rich-mano2", "rich-vert").
Cliccando il comando _+ add_, viene creata una colonna identificata dal titolo "c" (eventualmente seguito dall'etichetta scelta), deputata alla descrizione del sistema di richiami.  

Per compilare la colonna utilizzare i comandi del riquadro **_action_**.
Nel campo _column_ selezionare "c" (o "c.etichetta").  

Il campo _edit the selected column definition_ apre un **editor** che permette di descrivere alcune caratteristiche del sistema di richiami attraverso i seguenti campi:
* _rank_: non compilare;
* _position_: selezionare un valore tra: marg. inf. est.; marg. inf. cen.; marg. inf. int.; altro;  
* _vertical_: spuntare nel caso di richiami sono verticali;  
* _decoration_: descrizione di eventuali motivi decorativi relativi ai richiami (colore, presenza di cartiglio, presenza di disegni, etc.);
* _note_: si raccolgono qui dati e informazioni che non è possibile inserire altrove, con particolare riferimento a eventuali irregolarità nell'uso dei richiami.

⚠️ Dopo aver compilato la sottoparte, salvarla cliccando sul tasto di spunta blu.  

Il campo _action_ permette, attraverso una specifica formula, di attribuire dei valori alle celle della colonna selezionata.  
La formula consente di compilare rapidamente la colonna relativa ai richiami permettendo l'inserimento di un valore convenzionale ('R') per segnalare su quali carte sono presenti i richiami.  

La **formula** per l'inserimento dei richiami deve rispettare la seguente sintassi:  
range := R  
* range = la carta fisica o l'intervallo, anche discontinuo, di carte fisiche sulle quali sono presenti i richiami.  
* \: = comando preposto all'inserimento di un valore convenzionale fisso.  
* R = valore convenzionale per segnalare la presenza di richiami.  

> es. 8v 16v 24v:=R permette l'inserimento di tre richiami alle carte 8v 16v 24v:  
>           -8v 16v 24v: carte fisiche sulle quali sono inseriti i richiami;
>           -R: valore convenzionale con cui viene compilato automaticamente il campo _edit value_ delle celle.  
  
Dopo avere inserito la formula, cliccare il comando _Execute_.
L'applicazione della formula assegna alle celle interessate l'etichetta 'R'.  

È sempre possibile editare manualmente il valore di una cella cliccando sul suo campo _edit value_.  
Si ricorre a questa modalità di compilazione nel caso in cui si voglia registrare la parola-richiamo.  


#### Signature

Permette di creare e compilare una o più colonne relative alla segnatura fascicolare.  
È possibile infatti creare un elemento del tipo _signature_ per ogni differente tipologia di segnatura fascicolare.  

Per creare la colonna utilizzare i comandi del riquadro **_adder_**.
Nel campo _type_ selezionare _signature_.  
Il campo _name_ può essere compilato con un'etichetta convenzionale (es. "sign-alfab", "sign-rom").
Cliccando il comando _+ add_, viene creata una colonna identificata dal titolo "s" (eventualmente seguito dall'etichetta scelta), deputata alla descrizione della segnatura fascicolare.  

Per compilare la colonna utilizzare i comandi del riquadro **_action_**.
Nel campo _column_ selezionare "s" (o "s.etichetta").  

Il campo _edit the selected column definition_ apre un **editor** che permette di descrivere alcune caratteristiche della segnatura fascicolare attraverso i seguenti campi:
* _rank_: non compilare;
* _system_: selezionare un valore tra: arabo, romano, alfabetico, altro;
* _position_: selezionare un valore tra: marg. sup. est., marg. sup. cen., marg. sup. int., marg. inf. est., marg. inf. cen., marg. inf. int., altro;  
* _note_: si raccolgono qui dati e informazioni che non è possibile inserire altrove, con particolare riferimento a eventuali irregolarità nella segnatura fascicolare.

⚠️ Dopo aver compilato la sottoparte, salvarla cliccando sul tasto di spunta blu.  

Il campo _action_ permette, attraverso una specifica formula, di attribuire dei valori alle celle della colonna selezionata.  
La formula consente di compilare rapidamente la colonna relativa alla segnatura fascicolare permettendo l'inserimento di un valore convenzionale ('SF') per segnalare su quali carte è presente.  

La **formula** per l'inserimento della segnatura fasciolare deve rispettare la seguente sintassi:  
range := SF  
* range = la carta fisica o l'intervallo, anche discontinuo, di carte fisiche sulle quali sono presenti i richiami.  
* \: = comando preposto all'inserimento di un valore convenzionale fisso.  
* SF = valore convenzionale per segnalare la presenza di segnatura fascicolare.  

> es. 1r 9r 17r:=SF permette di segnalare la presenza di segnatura fascicolare alle carte 1r 9r 17r:  
>           -1r 9r 17r: carte fisiche sulle quali è segnalata la presenza di segnatura fascicolare;
>           -SF: valore convenzionale con cui è compilato automaticamente il campo _edit value_ delle celle.  
  
Dopo avere inserito la formula, cliccare il comando _Execute_.
L'applicazione della formula assegna alle celle interessate l'etichetta 'SF'.  

È sempre possibile editare manualmente il valore di una cella cliccando sul suo campo _edit value_.  
Si ricorre a questa modalità di compilazione nel caso in cui si vogliano registrare i valori esatti con cui è espressa la segnatura fascicolare.  


#### Register

Permette di creare e compilare una o più colonne relative alla segnatura a registro.  
È possibile infatti creare un elemento del tipo _register_ per ogni differente tipologia di segnatura a registro.   

Per creare la colonna utilizzare i comandi del riquadro **_adder_**.
Nel campo _type_ selezionare _register_.  
Il campo _name_ può essere compilato con un'etichetta convenzionale (es. "reg-1", "reg-mano2").
Cliccando il comando _+ add_, viene creata una colonna identificata dal titolo "r" (eventualmente seguito dall'etichetta scelta), deputata alla descrizione della segnatura a registro.  

Per compilare la colonna utilizzare i comandi del riquadro **_action_**.
Nel campo _column_ selezionare "r" (o "r.etichetta").  

Il campo _edit the selected column definition_ apre un **editor** che permette di descrivere alcune caratteristiche della numerazione attraverso i seguenti campi:
* _rank_: non compilare;
* _position_: selezionare un valore tra: marg. sup. est., marg. sup. cen., marg. sup. int., marg. inf. est., marg. inf. cen., marg. inf. int., altro;  
* _note_: si raccolgono qui dati e informazioni che non è possibile inserire altrove, con particolare riferimento a eventuali irregolarità nella segnatura a registro.

⚠️ Dopo aver compilato la sottoparte, salvarla cliccando sul tasto di spunta blu.  

Il campo _action_ permette, attraverso una specifica formula, di attribuire dei valori alle celle della colonna selezionata.  
La formula consente di compilare rapidamente la colonna relativa alla segnatura a registro permettendo l'inserimento di un valore convenzionale ('SR') per segnalare su quali carte è presente.  

La **formula** per l'inserimento della segnatura a registro deve rispettare la seguente sintassi:  
range := SR  
* range = la carta fisica o l'intervallo, anche discontinuo, di carte fisiche sulle quali è presente la segnatura a registro.  
* \: = comando preposto all'inserimento di un valore convenzionale fisso.  
* SR = valore convenzionale per segnalare la presenza di segnatura a registro.  

> es. 1r 2r 3r 4r 9r 10r 11r 12r :=SR permette di segnalare la presenza di segnatura fascicolare alle carte 1r 2r 3r 4r 9r 10r 11r 12r:  
>           -1r 2r 3r 4r 9r 10r 11r 12r: carte fisiche sulle quali è segnalata la presenza di segnatura fascicolare;  
>           -SR: valore convenzionale con cui sarà compilato automaticamente il campo _edit value_ delle celle.  
  
Dopo avere inserito la formula, cliccare il comando _Execute_.
L'applicazione della formula assegna alle celle interessate l'etichetta 'SR'.  

È sempre possibile editare manualmente il valore di una cella cliccando sul suo campo _edit value_.  
Si ricorre a questa modalità di compilazione nel caso in cui si vogliano registrare i valori esatti (es. a1, a2,..., b1, b2, etc.) con cui è espressa la segnatura a registro. 


## Endleaves
La sezione permette di elencare e descrivere le carte di guardia.  
Per descrivere le carte di guardia aggiungere un elemento _endleaf_ mediante [[editor|Editor_Brick.md]].  

Per ogni elemento _endleaf_ è possibile compilare i seguenti campi:  
* _location_: permette di indicare la carta di guardia da descrivere, selezionandola tra quelle precedentemente create (da menu a tendina);  
* _material_: selezionare un valore tra: membr.; cart.
* _tag_: permette di inserire un'etichetta utile ai fine della ricerca;
* _chronotope_: indicare data e luogo della carta di guardia secondo il modello [Asserted Date](Asserted_Chronotope_Brick.md).

⚠️ Dopo aver compilato la sottoparte, salvarla cliccando sul tasto di spunta blu.


## Help
Offre una pagina di aiuto con le istruzioni per la compilazione della sezione label.


## Save ⚠️ 

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
