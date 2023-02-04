# Regole per identificativi e authority file
Per ogni _item_ e per alcune _parts_ e _elements_, Itinera si serve di:
* un identificativo interno _human readable_ (**EID**), che permette di identificare e, ove necessario, richiamare le entità di interesse all'interno del database;  
* eventuali identificativi esterni (**External Ids**), che permettono di collegare gli _item_ a risorse esterne al database Itinera.  

⚠️ La compilazione dell'_eid_ degli _item_ è obbligatoria: senza di esso risulta impossibile stabilire qualsiasi collegamento tra gli _item_. Cfr. [Metadata Part](Metadata_Part.md) 

⚠️⚠️⚠️ Il compilatore non deve confondere _eid_ e _title_ dell'_item_, che sono due proprietà diverse e con diverse funzioni.

## EID
Nella banca dati Itinera gli _eid_ si indicano in campi diversi a seconda della tipologia di entità da identificare. I campi in cui si inseriscono gli _eid_ sono: _EID_ o _ID_ o [_Asserted Id_](Asserted_Ids_Brick.md).  

Ogni volta che si incontra uno di questi campi sono disponibili due possibilità, tra loro alternative:  
* assegnazione di un nuovo _eid_, se l'entità ne è sprovvista;  
* richiamo dell'_eid_ già assegnato all'entità, nel caso in cui l'entità esista e sia già identificata all'interno del database.

### Attribuire un EID

Quando si renda necessario **creare ed attribuire** un nuovo _eid_, occorre attenersi alle seguenti regole generali:  
* l'_eid_ si compone di caratteri a-z, 0-9; 
* l'_eid_ non può contenere lettere maiuscole;  
* l'_eid_ non può contenere spazi;
* l'_eid_ non può contenere trattino semplice (-), sostituito eventualmente dall'underscore (\_); 
* il primo carattere dell'_eid_ non può mai essere un numero;

Per l'_eid_ degli _item person_, si ricorre al nome della persona nella forma indicata nel [repository dei nomi di persona](repository.md), ponendo tutte le lettere in minuscolo e sostituendo eventuali spazi e segni di interpunzione con underscore (\_):  
> es.  Giovanni dell’Incisa > giovanni_dell_incisa   
> 
Per l'_eid_ degli _item text_, si ricorre al _title_ dell'_item_, sostituendo spazi e segni di interpunzione con underscore (\_). Nel caso dei testi citati attraverso l'_incipit_, il titolo va abbreviato in modo opportuno:  
>  es. Fam. I 1 > Fam_I_1.  
>  es. Rvf 84 > Rvf_84    
>  es. I’provai già quanto la soma è grave > I_provai 
>       
Per l'_eid_ degli _item manuscript_, si indica sinteticamente la sigla della biblioteca e/o del fondo come riportata nel [repository dei manoscritti](repository.md), seguita da underscore (\_) e dalla segnatura. Nel caso in cui la segnatura del codice comprenda punti, questi sono sostituiti da underscore (\_):  
> es. "Plut_XL_1" 🚧  
> es. "Bodl_Can_It_66" 🚧  

Per gli _eid_ di singole parti (ad es. Events, Hands, Edits, etc.), consultare le linee guida delle relative _parts_.  

⚠️ È di fondamentale importanza che l'_eid_ sia univoco e non abbia doppioni. Il compilatore deve perciò verificare sempre e in primo luogo se nel [repository](repository.md) sia già stato attribuito un _eid_ all'_item_ da descrivere. In caso positivo, il compilatore ricorrerà all'_eid_ già assegnato. Diversamente, procederà ad una nuova attribuzione, facendo attenzione a che il nuovo _eid_ non corrisponda ad alti già presenti a sistema. Per le verifiche necessarie all'attribuzione, il compilatore può ricorrre ai [repository predisposti](repository.md) e allo strumento di [lookup](lookup.md).   


### Riuso di un EID già esistente
Se l'entità di interesse (_item_, _part_, o singolo elemento) è già provvista di un identificativo (_eid_) all'interno di Itinera, occorre copiare quest'ultimo nel campo _EID_/_ID_/_Asserted Id_.    
Per cercare gli _eid_ esistenti è possibile ricorrere ai [repository](repository.md) (solo per determinate entità) o alla funzione di [lookup](lookup.md) (per qualsiasi elemento).   


## External Ids
Per attribuire un identificativo esterno, consultare la sezione relativa in [AssertedId](Asserted_Ids_Brick.md).
