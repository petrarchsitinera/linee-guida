# Hands Part

**Hands Part** permette di descrivere le mani responsabili della trascrizione del codice.

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-codicology#codhandspart).

Per aggiungere la parte, selezionare **_hands_** dal menu a tendina, quindi cliccare su **_add part_**.  

## Hand

Per ogni mano individuabile nel codice è creato un elemento _hand_ mediante un [editor](Editor_Brick.md).  

⚠️ Per ogni elemento _hand_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Creando un elemento _hand_ si accede a una schermata introduttiva dove è possibile compilare i seguenti campi e sezioni:

* EID
* name
* descriptions
* instances
* subscriptions
* references

### EID 
Permette di attribuire un identificativo convenzionale alla mano.
Per ogni mano utilizzare l'etichetta convenzionale "mano" seguita da trattino basso e lettera alfabetica minuscola (es. "mano_a", "mano_b", etc.).  

⚠️ Se la mano è riconducibile ad un copista noto, questo dato è espresso in un Item Person relativo al copista.  

Se il copista coincide con una persona già schedata come corrispondente nel database di Itinera (es. Giovanni Boccaccio), occorre accedere alla [EventsPart](Events_Part.md) dell'Item Person relativo.  
Creare un evento con _type_ "trascrizione";  nella sezione _related_ inserire una _related entity_ con _type_ "mano" e nel campo _eid_ inserire l'_eid_ della mano.  
L'eid della mano deve essere cercato attraverso la funzione di [lookup](lookup.md) e ad esso deve essere premesso, separato da "/", l'identificativo dell'_item_ (la voce _item ID_ nella finestra di _lookup_).  

Se il copista non ha un Item Person occorre crearlo ex novo. Questa procedura deve essere seguita anche nel caso di copista anonimo noto agli studi per la sua produzione (es. "copista principale del Dante dei Cento").  
Ugualmente, deve essere creato un Item Person per qualsiasi copista la cui mano sia riconosciuta su almeno due manoscritti, e anche in tutti i casi ove sia possibile fornire qualche informazione biografica relativa al copista (es. notaio, copista di professione, etc.).  
Una volta creato l'_item_, accedere alla [EventsPart](Events_Part.md) e procedere come descritto sopra.    

La compilazione del campo è facoltativa.

### Name
Permette di attribuire un nome alla mano.  
Per ogni mano utilizzare l'etichetta convenzionale "mano" seguita da lettera alfabetica maiuscola (es. "mano A", "mano B", etc.).  
Se il copista è noto o se è possibile indicare una denominazione convenzionalmente utilizzata negli studi, il nome o la denominazione sono espressi per esteso tra parentesi dopo l'etichetta: es. "mano A (Giovanni Boccaccio)".  

La compilazione del campo è obbligatoria.

### Instances
La sezione permette di individuare e descrivere i singoli interventi scrittori. La sezione è replicabile.

> Ogni _instance_ rappresenta un distinto intervento scrittorio riconducibile a una stessa mano. Se una stessa mano è responsabile di più interventi scrittori distinti, questi sono tutti espressi all'interno di uno stesso elemento _hand_ come _instances_ distinte.    
> Non è stabilito un criterio univoco per l'individuazione di _instances_ distinte.  
> Una sezione di codice trascritta da un unico copista che non presenti sostanziali differenze di scrittura può essere espressa come un'unica _instance_.  
> Se invece in una porzione di codice trascritta da una stessa mano sono individuabili differenze formali nella scrittura (ad es. mutamento di tipologia grafica), o sono ricostruibili fasi di copia distinte cronologicamente (ad es. grazie a sottoscrizioni) e logicamente (ad es. l'apposizione, da parte del copista stesso, di elementi paratestuali come rubriche, postille, commenti posteriori all'atto di copia), queste possono essere espresse come _instances_ differenti.  
> In ogni caso, la creazione di più _instances_ rimane a discrezione del compilatore, dipendendo, da un lato, dalla presenza di elementi che permettono di distinguere i singoli atti scrittori, dall'altro dal grado di approfondimento con cui si vuole descrivere la mano.  
> Una descrizione più approfondita della mano può essere ospitata nella sezione _description_. È consigliabile compilare la sezione _instance_ prima della sezione _description_.  

La compilazione della sezione è obbligatoria: ogni mano deve avere almeno una _instance_ compilata.

⚠️ Per ogni elemento _instance_ inserito è necessario salvare cliccando sul tasto di spunta blu.

#### Script
Permette di indicare la tipologia grafica della _instance_. Selezionare un valore tra:

* gotica
* semigotica
* minuscola cancelleresca
* mercantesca antica
* corsiva umanistica
* antiqua
* altro

La compilazione del campo è obbligatoria.

#### Rank
Permette di esprimere il grado di attendibilità con cui la _instance_ è riferibile alla mano in oggetto.  
Compilare solo nei casi dubbi, con il valore "2" per indicare che l'attribuzione ha un minimo grado di incertezza, o "3" per indicare che l'attribuzione è molto incerta.  

#### Location
Permette di indicare le carte interessate dalla _instance_, secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

#### Description key
Permette di collegare la _instance_ a una _description_ richiamando la _key_ corrispondente.  
⚠️  Questo campo compare solo dopo la creazione di almeno un elemento _description_ e la compilazione del relativo campo [_key_](Hands_Part.md#key).  
Cliccando il campo _description key_ appare la lista delle _keys_ già create in _description_. Selezionare una _key_ per collegare la _instance_  alla _description_ corrispondente.  
La compilazione del campo è obbligatoria qualora risulti necessario collegare la _instance_ a una _description_.

#### Typologies
Permette di indicare la tipologia della _instance_. Selezionare uno o più valori tra:

* testo
* postille
* commento 
* correzioni
* integrazione
* rubriche
* segni paragrafematici
* titoli correnti
* segni di attenzione
* indici
* altro

La compilazione del campo è obbligatoria.

#### Colors
Permette di indicare il colore dell'inchiostro utilizzato per la _instance_. Selezionare uno o più valori tra:

* bruno scuro
* bruno chiaro
* rosso
* blu
* altro

La compilazione del campo è obbligatoria.

#### Chronotopes
Permette di indicare i dati cronologici relativi alla _instance_, secondo il modello [Asserted Chronotope](Asserted_Chronotope_Brick.md).   
Se la datazione è derivata da una sottoscrizione (registrata nella sezione _subscriptions_), nel _tag_ relativo a _place_ e/o a _date_ si indica "sottoscrizione".  
Nel caso sia stata individuata e creata una sola _instance_, la compilazione del campo _date_ è obbligatoria (in assenza di date certe, indicando una data al secolo).  
Nel caso siano state individuate e create più _instances_, è obbligatorio compilare il campo _date_ di almeno una di esse (in assenza di date certe, indicando una data al secolo). Se una delle _instances_ risulta datata (da sottoscrizione), sarà sufficiente registrare tale indicazione cronologica; in presenza di più _instances_ datate occorrerà registrare l'indicazione cronologica di ognuna.

#### Images
Per inserire immagini di una o più carte del codice che trasmettono l'intervento scrittorio, cliccare su **add image**. Per la compilazione vedi [Cod_Image](Cod_Image_Brick.md).


### Descriptions
La sezione permette di inserire la descrizione dettagliata di uno o più interventi scrittori. L'elemento è replicabile.  

> _Description_ permette di fornire una descrizione analitica della mano.  
> È sufficiente creare un unico elemento _description_ qualora i tratti caratteristici della scrittura siano uniformi, anche in presenza di distinti interventi scrittori (_instances_). Se, ad esempio, sono state create più _instances_ distinte per dati cronologici ma non per caratteristiche grafiche, queste _instances_ corrisponderanno ad un'unica _description_.  
> Nel caso in cui, invece, le _instances_ risultino distinte per aspetti strettamente grafici, sarà possibile e opportuno riferile a _description_ differenti.  
> Il collegamento di _description_ e _instance_ avviene attraverso i campi _key_ e _description key_: ad ogni _description_ è possibile attribuire un'etichetta attraverso il campo _key_ (vedi oltre); la _key_ può essere richiamata nel campo _description key_ di ciascuna _instance_ per collegarla  alla descrizione corrispondente.

La compilazione del campo è facoltativa.

⚠️ Per ogni elemento _description_ inserito è necessario salvare cliccando sul tasto di spunta blu.

#### Key
Permette di attribuire alla descrizione un'etichetta che ne consenta il collegamento con uno o più elementi _instance_, attraverso il campo [_description key_](Hands_Part.md#description-key).  
Per ogni _description_ utilizzare l'etichetta convenzionale "descr" seguita senza spazi da numero progressivo (es. "descr1", "descr2", etc.).  

La compilazione del campo è obbligatoria qualora risulti necessario collegare la _description_ a una o più _instance_.

#### Description
Permette di inserire, in forma di stringa di testo libero, una descrizione discorsiva delle caratteristiche della mano (o della singola _instance_).  
Questo campo offre la possibilità di fornire una descrizione di tipo tradizionale che si va ad affiancare a quanto espresso, in forma parcellizzata (e dunque computabile), nei singoli campi delle sezioni _instance_ e _description_. Offre inoltre la possibilità di fornire informazioni che non sia possibile esprimere negli altri campi. 

> È possibile descrivere l’aspetto generale della scrittura; segnalare lettere ed elementi grafici caratterizzanti; indicare la presenza di note in margine di mano del copista; segnalare l’eventuale uso di scritture diverse rispetto a quelle del testo ad uso distintivo; indicare la presenza di segni di paragrafatura o segni di attenzione (maniculae, schemi, ecc.), appartenenti a tutti gli effetti al progetto di copia, specificando eventualmente in quali punti del testo si trovano e che funzione hanno.  

La compilazione del campo è obbligatoria.

#### Notes
Permette di descrivere in forma discorsiva aspetti caratterizzanti di iniziali, correzioni, interpunzione e abbreviazioni.  
Selezionare dal menù a tendina la tipologia di intervento da descrivere:

* _initials_:  
si specifica l’eventuale uso di iniziali al tratto con funzione significativa, con eventuali esempi ritenuti particolarmente caratterizzanti.  
* _corrections_:  
si descrivono le tipologie di interventi correttivi, con eventuali esempi ritenuti particolarmente caratterizzanti.  
* _punctuation_:  
si descrive la tipologia del sistema interpuntivo, con eventuali esempi ritenuti particolarmente caratterizzanti.  
* _abbreviations_:  
si descrive la tipologia del sistema abbreviativo, con eventuali esempi ritenuti particolarmente caratterizzanti.  

La compilazione del campo è facoltativa.

#### Signs
Permette di descrivere analiticamente singoli segni grafici. L'elemento è replicabile.  
La sua compilazione è facoltativa.

⚠️ Per ogni elemento _sign_ inserito è necessario salvare cliccando sul tasto di spunta blu.

##### Type
Permette di indicare la tipologia di segno descritto. Selezionare un valore tra:

* lettera
* interpunzione
* abbreviazione
* nesso
* legamento
* altro

La compilazione del campo è obbligatoria.

##### EID
Permette di attribuire al segno un identificativo convenzionale, secondo le regole stabilite per gli [identificativi](identifiers.md) (es. per le lettere: "d_onciale", "g_alambicco", "s_scivolata"; per abbreviazioni: "nota_tironiana", "titulus_nasale"; per i nessi: "ct"; etc.). Consultare il [repository relativo](repository.md).    
La compilazione del campo è facoltativa.  

##### Location
Permette di indicare la collocazione nel codice del segno descritto, secondo il modello [Cod Location](Cod_Location_Brick.md), avendo cura di indicare anche la riga e la parola in cui è testimoniato il segno descritto.  
La compilazione del campo è obbligatoria.

##### Description
Permette di fornire una descrizione discorsiva del segno.  
La compilazione del campo è facoltativa.


### Subscriptions
Permette di elencare e descrivere le eventuali sottoscrizioni del copista cui appartiene la mano in oggetto.  L'elemento è replicabile per ogni singola sottoscrizione. In caso di più sottoscrizioni testualmente identiche è possibile creare un unico elemento _subscription_ registrando nel campo _range_ tutte le carte interessate.  

La compilazione della sezione è obbligatoria in presenza di sottoscrizione. 

⚠️ Per ogni elemento _subscription_ inserito è necessario salvare cliccando sul tasto di spunta blu.

#### Range
Permette di indicare le carte su cui è posta la sottoscrizione, secondo il modello [Cod Location](Cod_Location_Brick.md).  
La compilazione del campo è obbligatoria.

#### Language
Permette di indicare la lingua in cui è espressa la sottoscrizione. Selezionare un valore tra:

* italiano
* latino
* greco
* latino-volgare
* altro

La compilazione del campo è obbligatoria.

#### Text
Permette di riportare il testo integrale della sottoscrizione. La sottoscrizione può anche comparire in forma di sigla, crittografia, nota di possesso, motto e va in ogni caso trascritta.  
La compilazione del campo è obbligatoria.

#### Note
Permette di aggiungere informazioni non raccolte negli altri campi del modello.  
La compilazione del campo è facoltativa.

### References
Permette di registrare l'eventuale bibliografia relativa alla mano in oggetto, secondo il modello [DocReference](Docref_Brick.md).  
L'elemento è replicabile per ogni voce bibliografica.   

La compilazione del campo è facoltativa.

## Save ⚠️ 

Cliccare sul tasto **_save_** per salvare la parte.
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
