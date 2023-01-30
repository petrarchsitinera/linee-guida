# Decorations Part
**Decorations Part** permette di descrivere la decorazione del manoscritto.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#coddecorationspart).

Per aggiungere la parte, selezionare **_decorations_** dal menu a tendina, quindi cliccare sul comando **_add part_**. 

## Decoration 
Per ogni apparato decorativo unitario è creato un elemento _decoration_ mediante [editor](Editor_Brick.md).

> Con "apparato decorativo unitario" si intende una serie di elementi decorativi eseguiti nell'ambito di una campagna di decorazione che si suppone essere stata realizzata nello stesso luogo, tempo e secondo un progetto unitario.

⚠️ Per ogni elemento _decoration_ inserito è necessario salvare cliccando sul comando di spunta blu.

Creando un elemento _decoration_ si accede a una schermata da cui è possibile compilare i seguenti campi e sezioni:

* ID
* Name
* Features
* Chronotopes
* References
* Artists
* Elements 


### ID
Permette di attribuire un identificativo convenzionale all'apparato decorativo (_decoration_), che può essere richiamato in altre sezioni (_parts_) dell'_item_.
Per ogni apparato decorativo utilizzare l'etichetta convenzionale "dec" seguita senza spazi da un numero progressivo (es. "dec1", "dec2", etc.).  

La compilazione del campo è obbligatoria.


### Name
Permette di attribuire un nome all'apparato decorativo. Compilare il campo ripetendo l'ID, a meno che non sia possibile indicare una denominazione convenzionalmente utilizzata negli studi.


### Features
Se la decorazione è stata eseguita al di fuori del progetto originario del codice spuntare la casella _non originale_.
Se la decorazione è incompleta spuntare la casella _incompleta_.

Ulteriori precisazioni possono essere espresse nel campo _note_.


### Chronotopes
Permette di indicare data e luogo di produzione dell'apparato decorativo, secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).

La compilazione del campo è obbligatoria.
Per la data, in mancanza di indicazione cronologica più specifica, utilizzare datazioni al secolo. 

⚠️ Per ogni elemento _chronotope_ inserito è necessario salvare cliccando sul comando di spunta blu.


### References
Permette di registrare l'eventuale bibliografia relativa all'apparato decorativo, secondo le norme definite per [External Bibliography](External_Bibliography_Part.md).

La compilazione del campo è facoltativa.

⚠️ Per ogni elemento _reference_ inserito è necessario salvare cliccando sul comando di spunta blu.


### Artist
Permette di inserire informazioni sul responsabile (decoratore o bottega) dell'apparato decorativo (d'ora in avanti, per convenzione, "artista").

L'elemento è replicabile. 

⚠️ Per ogni elemento _artist_ inserito è necessario salvare cliccando sul comando di spunta blu.

#### Type
Permette di indicare, attraverso un _thesaurus_, se la decorazione è stata realizzata da:
* miniatore
* bottega
* altro

La compilazione del campo è obbligatoria.

#### EID
Permette di attribuire un identificativo univoco all'artista, che può essere utilizzato per il collegamento con l'eventuale Item Person ad esso dedicato.  
Se il copista coincide con una persona già schedata nel database di Itinera, si utilizza l'_eid_ dell'Item Person già esistente. Cercare l'item e copiarne [l'_eid_](identifiers.md), servendosi eventualmente dei [repository](repository.md) e della funzione di [lookup](lookup.md).   

Dal momento che i decoratori non sono oggetto di studio specifico da parte di Itinera, solo in numerati casi sarà loro dedicato un Item Person apposito; negli altri casi, se una risorsa esterna a Itinera contiene informazioni specifiche sul realizzatore della decorazione, si rimanda ad esse tramite il campo Ids (vedi sotto).

La compilazione del campo è facoltativa.

#### Name
Permette di indicare il nome dell'artista.  
Se si tratta di un miniatore noto, riportare nome e cognome o la denominazione convenzionalmente utilizzata negli studi. 
Se si tratta di una bottega nota, riportare la denominazione convenzionalmente utilizzata negli studi (es.  ). 
Se l'artista non è noto, indicarlo mediante l'etichetta convenzionale "art" seguita da numero progressivo (es. "art1", "art2", etc.).

La compilazione del campo è obbligatoria.

#### Ids
Permette di collegare la scheda con eventuali risorse esterne dedicate all'artista (ad es. VIAF, DBI), secondo il modello [IDs brick](Asserted_Ids_Brick.md).

La compilazione del campo è facoltativa.

#### Element keys
Permette di attribuire all'artista uno specifico elemento decorativo, utilizzando la _key_ inserita nell' _element_ interessato (cfr. infra: 🚧 LINK INTRATESTUALE tramite MARKUP). In presenza di più elementi attribuiti, elencare le key di seguito separate da spazio.

La compilazione del campo è facoltativa.

#### Note
Raccoglie informazioni relative all'artista non esprimibili negli altri campi.

La compilazione del campo è facoltativa.

#### Styles
Permette di indicare un particolare stile decorativo o scuola a cui può essere ricondotto l'artista.  
L'elemento è replicabile.  
Per ogni stile decorativo / scuola possono essere compilati i seguenti campi:

* _Name_: inserire la denominazione convenzionalmente utilizzata negli studi.
* _Chronotope_: permette di indicare l'epoca di attestazione dello stile, secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md). 
* _Assertion_: permette di esprimere, secondo il modello [Assertion](Assertion_Brick.md), il grado di probabilità relativo all'appartenenza dell'artista allo stile indicato, e permette eventualmente di citare fonti a sostegno di tale ipotesi.

⚠️ Per ogni elemento _style_ inserito è necessario salvare cliccando sul comando di spunta blu.

La compilazione del campo è facoltativa.


### Elements - Informazioni generali
Questa sezione permette di descrivere singole tipologie di elementi decorativi.

Ogni elemento decorativo è articolato in tre distinte sottosezioni: general, typologies, description.  
Per prima cosa occorre indicare la tipologia di elemento decorativo che si intende descrivere. La scelta avviene selezionando una tipologia di elemento dal campo _type_ della sottosezione _general_:

* pagina incipitaria
* illustrazione
* ornamentazione
* iniziali-semplici
* iniziali-filigranate
* iniziali-ornate
* iniziali-istoriate
* paragrafematici
* spazi bianchi

A seconda della tipologia di elemento decorativo selezionata risultano compilabili nelle tre sottosezioni campi differenti.

***
⚠️ È possibile creare un _element_ per ogni singolo elemento decorativo o per gruppi di elementi decorativi della stessa tipologia.  
Ad es.:  
-se in un manoscritto sono presenti numerose iniziali filigranate senza differenze sostanziali che si ritenga opportuno segnalare, sarà creato un unico _element_ della tipologia "iniziali-filigranate" che accoglierà la descrizione complessiva delle stesse;  
-se in un manoscritto sono presenti alcune illustrazioni e si ritiene utile descriverle singolarmente, sarà creato un _element_ "illustrazione" per ognuna di esse.

⚠️ 🚧  Ogni _element_ è provvisto di un campo _key_ che può essere utilizzato per attribuire l'elemento prescelto alla paternità di uno specifico artista (tramite il campo _element-keys_ di _artist_ cfr. supra), nel caso in cui alla realizzazione dell'apparato decorativo abbiano partecipato più artisti.

⚠️ Per ogni _element_ inserito è necessario salvare cliccando sul comando di spunta blu.

***

### Elements - Pagina incipitaria
Permette di descrivere la pagina incipitaria o eventuali pagine, anche prive di funzione incipitaria, in cui sia presente una decorazione a piena pagina costituita da diversi elementi decorativi.
Ad es. una miniatura che occupi un'intera pagina ma non sia accompagnata da ulteriori elementi decorativi (cornici, stemmi, iniziali decorate, etc.) andrà descritta come "illustrazione" (e nel campo _positions_ sarà selezionata la voce "a piena pagina").

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _pagina incipitaria_.  
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di elementi decorativi dello stesso tipo che sono descritti nell' _element_ creato.  
Per la pagina incipitaria il campo è normalmente compilato con il valore "1", dal momento che ciascuna è, di norma, descritta singolarmente.  
La compilazione del campo è obbligatoria.

##### Location
Permette di indicare la collocazione della pagina incipitaria secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di indicare alcune caratteristiche della pagina incipitaria. Se pertinente, selezionare uno o più valori tra:

* spazi bianchi (la pagina incipitaria contiene sezioni lasciate in bianco)
* bozza (la pagina incipitaria o una sua parte è a un livello di elaborazione incompleto)
* illustrazione (la pagina incipitaria include illustrazioni)
* ornamentazione (la pagina incipitaria include ornamentazioni)
* iniziali (la pagina incipitaria include iniziali miniate)

La compilazione del campo è facoltativa.

⚠️ I singoli elementi decorativi (illustrazioni, ornamentazioni, iniziali miniate) che compongono la pagina incipitaria potranno eventualmente essere descritti singolarmente come nuovi _element_ ed essere collegati alla pagina incipitaria attraverso l'uso di _key_ e _parentKey_ (cfr. infra).

##### Key
Permette di attribuire un'etichetta alla pagina incipitaria, che sarà possibile richiamare in eventuali _element_ dedicati alla descrizione di illustrazioni, ornamentazioni, iniziali miniate che siano parte di quella pagina incipitaria.  
La _key_ dovrà essere costituita dall'etichetta convenzionale "pag-inc"; in caso di più pagine incipitarie, la formula sarà seguita da un numero progressivo (es. "pag-inc-1", "pag-inc-2", etc.).   
Inoltre, la _key_ può essere utilizzata per attribuire la pagina decorata alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

#### Typologies

##### Text relation
Permette di descrivere in forma di testo libero l’eventuale relazione tra testo e immagini presenti sulla pagina incipitaria.  
La compilazione del campo è facoltativa.

##### Subject
Permette di indicare i soggetti iconografici eventualmente presenti sulla pagina incipitaria.  
La compilazione del campo è facoltativa.

##### Colors
Permette di indicare i colori principali utilizzati nella realizzazione della pagina incipitaria. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale è realizzato la pagina incipitaria. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale è realizzata la pagina incipitaria. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

       
#### Description

##### Description
Permette di descrivere l'elemento decorativo nel suo complesso, attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini dell'elemento decorativo, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi all'elemento decorativo che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


### Illustrazione

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _illustrazione_.  
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di elementi decorativi dello stesso tipo che sono descritti nell' _element_.  
Per l'illustrazione il campo è normalmente compilato con il valore "1", dal momento che ciascuna è, di norma, descritta singolarmente.  
La compilazione del campo è obbligatoria.

##### Location
Permette di indicare la collocazione dell'illustrazione secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di segnalare i seguenti casi:

* spazi bianchi (l'illustrazione o una sua parte non è stata eseguita)
* bozza (l'illustrazione o una sua parte è a un livello di elaborazione incompleto)

La compilazione del campo è facoltativa.

##### Key
Può essere utilizzata per attribuire l'illustrazione alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

La _key_ dovrà essere costituita dall'etichetta convenzionale "ill"; in caso di più illustrazioni, la formula sarà seguita da un numero progressivo (es. "ill-1", "ill-2", etc.).   

La compilazione del campo è facoltativa.

##### ParentKey
Permette di collegare l'illustrazione alla pagina incipitaria di cui dovesse eventualmente far parte. Selezionare la _key_ precedentemente attribuita alla pagina incipitaria dal menu a tendina.  
La compilazione del campo è facoltativa.

#### Typologies

##### Typologies
Permette di indicare la tipologia di illustrazione. Selezionare uno o più valori tra:

* miniatura
* disegno
* tabellare
* papyrus style

La compilazione del campo è facoltativa.

##### Text relation
Permette di descrivere in forma libera l’eventuale relazione tra testo e illustrazione.  
La compilazione del campo è facoltativa.

##### Subject
Permette di descrivere i soggetti iconografici dell'illustrazione.  
La compilazione del campo è facoltativa.

##### Colors
Permette di indicare i colori utilizzati nella realizzazione dell'illustrazione. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale è realizzata l'illustrazione. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale è realizzata l'illustrazione. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

##### Positions
Permette di indicare la posizione dell'illustrazione sulla pagina. Selezionare uno o più valori tra:

* a piena pagina
* intercalata
* intercolumnio
* margine est.
* margine int.
* margine sup.
* margine inf.
* altro

La compilazione del campo è facoltativa.

#### Description

##### Description
Permette di descrivere l'illustrazione nel suo complesso, in un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini dell'illustrazione, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi all'illustrazione che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


### Ornamentazione

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _ornamentazione_.   
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di elementi di ornamentazione dello stesso tipo che sono descritti nell' _element_.   
La compilazione del campo è facoltativa.

##### Location
Permette di indicare la collocazione dell'ornamentazione secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di segnalare i seguenti casi:

* spazi bianchi (l'ornamentazione o una sua parte non è stata eseguita)
* bozza (l'ornamentazione o una sua parte è a un livello di elaborazione incompleto)

La compilazione del campo è facoltativa.

##### Key
Può essere utilizzata per attribuire l'ornamentazione alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

La _key_ dovrà essere costituita dall'etichetta convenzionale "orn"; in caso di più ornamentazioni, la formula sarà seguita da un numero progressivo (es. "orn-1", "orn-2", etc.).   

La compilazione del campo è facoltativa.

##### ParentKey
Permette di collegare l'ornamentazione alla pagina incipitaria di cui dovesse eventualmente far parte. Selezionare la _key_ precedentemente attribuita alla pagina incipitaria dal menu a tendina.  
La compilazione del campo è facoltativa.

#### Typologies

##### Typologies
Permette di indicare la tipologia dell'ornamentazione. Selezionare uno o più valori tra:

* fregio con figura
* fregio ornato
* stemma
* tabula ansata
* altro

La compilazione del campo è facoltativa.

##### Colors
Permette di indicare i colori utilizzati nella realizzazione dell'ornamentazione. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale è realizzata l'ornamentazione. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale è realizzata l'ornamentazione. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

##### Positions
Permette di indicare la posizione dell'ornamentazione attraverso un campo a testo libero.
 
La compilazione del campo è facoltativa.

#### Description

##### Description
Permette di descrivere l'ornamentazione nel suo complesso, in un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini dell'elemento decorativo, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi all'elemento decorativo che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


### Iniziali semplici

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _iniziali-semplici_.  
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di iniziali dello stesso tipo che sono descritti nell' _element_.  
La compilazione del campo è facoltativa.

##### Location
Permette di indicare la collocazione delle iniziali secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di segnalare i seguenti casi:

* spazi bianchi (una o più iniziali non sono stata eseguite) [🚧  CFR. ###SPAZI BIANCHI]
* bozza (una o più iniziali sono a un livello di elaborazione incompleto)
* lettere guida (una o più iniziali sono accompagnate da lettere guida)

La compilazione del campo è facoltativa.

##### Key
Può essere utilizzata per attribuire le iniziali alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

La _key_ dovrà essere costituita dall'etichetta convenzionale "ini-pla"; in caso di più _element_ relativi ad iniziali semplici, la formula sarà seguita da un numero progressivo (es. "ini-pla-1", "ini-pla-2", etc.).   

La compilazione del campo è facoltativa.

##### ParentKey
Permette di collegare le iniziali alla pagina incipitaria di cui dovessero eventualmente far parte. Selezionare la _key_ precedentemente attribuita alla pagina incipitaria dal menu a tendina.  
La compilazione del campo è facoltativa.

#### Typologies

##### Line height
Permette di indicare l’altezza delle iniziali in numero di righe.
La compilazione del campo è obbligatoria (se possibile rilevarla).

##### Colors
Permette di indicare i colori utilizzati nella realizzazione delle iniziali. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

##### Positions
Permette di indicare la posizione delle iniziali rispetto al testo. Selezionare uno o più valori tra:

* allineata
* annegata
* sporgente

La compilazione del campo è facoltativa.

#### Description

##### Description
Permette di descrivere le iniziali nel loro complesso, attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini delle iniziali, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi alle iniziali che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


### Iniziali filigranate

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _iniziali-filigranate_.  
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di iniziali dello stesso tipo che sono descritti nell' _element_.   
La compilazione del campo è facoltativa.

##### Location
Permette di indicare la collocazione delle iniziali secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di segnalare i seguenti casi:

* spazi bianchi (una o più iniziali non sono stata eseguite) [🚧  CFR. ###SPAZI BIANCHI]
* bozza (una o più iniziali sono a un livello di elaborazione incompleto)
* lettere guida (una o più iniziali sono accompagnate da lettere guida)

La compilazione del campo è facoltativa.

##### Key
Può essere utilizzata per attribuire le iniziali alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

La _key_ dovrà essere costituita dall'etichetta convenzionale "ini-wat"; in caso di più _element_ relativi ad iniziali filigranate, la formula sarà seguita da un numero progressivo (es. "ini-wat-1", "ini-wat-2", etc.).   

La compilazione del campo è facoltativa.

##### ParentKey
Permette di collegare le iniziali alla pagina incipitaria di cui dovessero eventualmente far parte. Selezionare la _key_ precedentemente attribuita alla pagina incipitaria dal menu a tendina.  
La compilazione del campo è facoltativa.

#### Typologies

##### Line height
Permette di indicare l’altezza delle iniziali in numero di righe.  
La compilazione del campo è obbligatoria (se possibile rilevarla).

##### Colors
Permette di indicare i colori utilizzati nella realizzazione delle iniziali. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

##### Positions
Permette di indicare la posizione delle iniziali rispetto al testo. Selezionare uno o più valori tra:

* allineata
* annegata
* sporgente

La compilazione del campo è facoltativa.

#### Description

##### Description
Permette di descrivere le iniziali nel loro complesso, attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini delle iniziali, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi alle iniziali che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.

### Iniziali ornate

#### General

###### Type
Nel _thesaurus_ è selezionata la voce _iniziali-ornate_.  
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di iniziali dello stesso tipo che sono descritti nell' _element_.  
La compilazione del campo è facoltativa.

##### Location
Permette di indicare la collocazione delle iniziali secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di segnalare i seguenti casi:

* spazi bianchi (una o più iniziali non sono stata eseguite) [🚧  CFR. ###SPAZI BIANCHI]
* bozza (una o più iniziali sono a un livello di elaborazione incompleto)
* lettere guida (una o più iniziali sono accompagnate da lettere guida)

La compilazione del campo è facoltativa.

##### Key
Può essere utilizzata per attribuire le iniziali alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

La _key_ dovrà essere costituita dall'etichetta convenzionale "ini-orn"; in caso di più _element_ relativi ad iniziali ornate, la formula sarà seguita da un numero progressivo (es. "ini-orn-1", "ini-orn-2", etc.).   

La compilazione del campo è facoltativa.

##### ParentKey
Permette di collegare le iniziali alla pagina incipitaria di cui dovessero eventualmente far parte. Selezionare la _key_ precedentemente attribuita alla pagina incipitaria dal menu a tendina.  
La compilazione del campo è facoltativa.


#### Typologies

##### Line height
Permette di indicare l’altezza delle iniziali in numero di righe.
La compilazione del campo è obbligatoria (se possibile rilevarla).

##### Typologies
Permette di indicare la tipologia di lettera ornata. Selezionare uno o più valori tra:

* zoomorfa
* fitomorfa
* antropomorfa
* prismatica
* bianchi girari
* caleidoscopica
* geometrica
* altro

La compilazione del campo è facoltativa.

##### Subject
Permette di indicare il soggetto iconografico eventualmente rappresentato nell'iniziale.  
La compilazione del campo è facoltativa.

##### Colors
Permette di indicare i colori utilizzati nella realizzazione delle iniziali. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

##### Positions
Permette di indicare la posizione delle iniziali rispetto al testo. Selezionare uno o più valori tra:

* allineata
* annegata
* sporgente

La compilazione del campo è facoltativa.

#### Description

##### Description
Permette di descrivere le iniziali nel loro complesso, attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini delle iniziali, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi alle iniziali che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


### Iniziali istoriate

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _iniziali-istoriate_.  
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di iniziali dello stesso tipo che sono descritti nell' _element_.  
La compilazione del campo è facoltativa.

##### Location
Permette di indicare la collocazione delle iniziali secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di segnalare i seguenti casi:

* spazi bianchi (una o più iniziali non sono stata eseguite) [🚧  CFR. ###SPAZI BIANCHI]
* bozza (una o più iniziali sono a un livello di elaborazione incompleto)
* lettere guida (una o più iniziali sono accompagnate da lettere guida)

La compilazione del campo è facoltativa.

##### Key
Può essere utilizzata per attribuire le iniziali alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

La _key_ dovrà essere costituita dall'etichetta convenzionale "ini-fig"; in caso di più _element_ relativi ad iniziali istoriate, la formula sarà seguita da un numero progressivo (es. "ini-fig-1", "ini-fig-2", etc.).   

La compilazione del campo è facoltativa.

##### ParentKey
Permette di collegare le iniziali alla pagina incipitaria di cui dovessero eventualmente far parte. Selezionare la _key_ precedentemente attribuita alla pagina incipitaria dal menu a tendina.  
La compilazione del campo è facoltativa.


#### Typologies

##### Line height
Permette di indicare l’altezza delle iniziali in numero di righe.
La compilazione del campo è obbligatoria (se possibile rilevarla).

##### Text relation
Permette di indicare l’eventuale relazione tra testo e raffigurazioni presenti nell'iniziale.  
La compilazione del campo è facoltativa.

##### Subject
Permette di indicare il soggetto iconografico eventualmente rappresentato nell'iniziale.  
La compilazione del campo è facoltativa.

##### Colors
Permette di indicare i colori utilizzati nella realizzazione delle iniziali. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale sono realizzate le iniziali. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

##### Positions
Permette di indicare la posizione delle iniziali rispetto al testo. Selezionare uno o più valori tra:

* allineata
* annegata
* sporgente

La compilazione del campo è facoltativa.

#### Description

##### Description
Permette di descrivere le iniziali nel loro complesso, attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini delle iniziali, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi alle iniziali che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


### Paragrafematici 

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _paragrafematici_.  
La compilazione del campo è obbligatoria.

##### Count
Non compilare il campo.

##### Location
Permette di indicare la collocazione dei paragrafematici secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Features
Permette di segnalare i seguenti casi:

* spazi bianchi (uno o più elementi paragrafematici non sono stati eseguiti) [🚧  CFR. ###SPAZI BIANCHI]
* bozza (uno o più elementi paragrafematici sono a un livello di elaborazione incompleto)

La compilazione del campo è facoltativa.

##### Key
Può essere utilizzata per attribuire gli elementi paragrafematici alla paternità di uno specifico artista; la key attribuita all' _element_ andrà richiamata nel campo _element-keys_ di _artist_ (cfr. supra 🦅).

La _key_ dovrà essere costituita dall'etichetta convenzionale "par"; in caso di più _element_ relativi ad elementi paragrafematici, la formula sarà seguita da un numero progressivo (es. "par-1", "par-2", etc.).   

La compilazione del campo è facoltativa.

##### ParentKey
Permette di collegare gli elementi paragrafematici alla pagina incipitaria di cui dovessero eventualmente far parte. Selezionare la _key_ precedentemente attribuita alla pagina incipitaria dal menu a tendina.  
La compilazione del campo è facoltativa.

#### Typologies

##### Typologies
Permette di indicare la tipologia degli elementi paragrafematici. Selezionare uno o più valori tra:

* titoli correnti
* rubricatura
* segni di paragrafo
* cartulazione
* altro

La compilazione del campo è facoltativa.

##### Colors
Permette di indicare i colori utilizzati nella realizzazione degli elementi paragrafematici. Selezionare uno o più valori tra:

* blu
* rosso
* verde
* giallo
* bianco
* viola
* turchese
* altro

La compilazione del campo è facoltativa.

##### Gildings
Permette di indicare la presenza di doratura e di specificare la tecnica con cui è realizzata. Selezionare uno o più valori tra:

* foglia
* polvere

La compilazione del campo è facoltativa.

##### Techniques
Permette di indicare la tecnica con la quale sono realizzati gli elementi paragrafematici. Selezionare uno o più valori tra:

* acquerello
* tempera
* inchiostro
* altro

La compilazione del campo è facoltativa.

##### Tools
Permette di indicare lo strumento con il quale sono realizzati gli elementi paragrafematici. Selezionare uno o più valori tra:

* penna
* pennello
* altro

La compilazione del campo è facoltativa.

##### Positions
Permette di indicare la posizione degli elementi paragrafematici attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

#### Description

##### Description
Permette di descrivere gli elementi paragrafematici nel loro complesso, attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini degli elementi paragrafematici, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi agli elementi paragrafematici che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


### Spazi bianchi
Questo campo è compilato solo nel caso in cui non sia possibile stabilire a quale tipologia di elemento decorativo corrispondano gli spazi bianchi.  
Se invece è possibile ricollegare uno spazio bianco ad un determinato elemento decorativo (ad es. uno spazio bianco in una serie di iniziali), esso viene registrato nell' _element_ corrispondente spuntando il flag _spazi bianchi_ nel _thesaurus_ del campo _features_.

#### General

##### Type
Nel _thesaurus_ è selezionata la voce _spazi bianchi_.  
La compilazione del campo è obbligatoria.

##### Count
Permette di indicare il numero di spazi bianchi descritti nell' _element_.  
La compilazione del campo è facoltativa.

##### Location
Permette di indicare la collocazione degli spazi bianchi secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

##### Key
Non compilare il campo.

##### ParentKey
Non compilare il campo.

#### Description

##### Description
Permette di fornire informazioni relative allo spazio bianco (dimensioni, posizione sulla carta, etc.), attraverso un campo a testo libero.  
La compilazione del campo è facoltativa.

##### Image
Per inserire immagini dell'elemento decorativo, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).

##### Note
Si raccolgono qui dati e informazioni relativi all'elemento che non è possibile inserire altrove.  
La compilazione del campo è facoltativa.


## Save ⚠️ 

Per ogni elemento _decoration_ inserito è necessario salvare cliccando sul comando di spunta blu.

Cliccare sul comando **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul comando **_Close_** per tornare alla schermata di riepilogo dell'item.

