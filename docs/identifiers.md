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
* riuso di un _eid_, se l'entità ne possiede già uno.

### Creazione di un nuovo EID

Nei casi in cui sia necessario **creare ed attribuire** un nuovo _eid_, è necessario attenersi alle seguenti regole generali:  
* l'_eid_ deve essere composto esclusivamente con i caratteri a-z, 0-9; 
* non utilizzare lettere maiuscole;  
* utilizzare sempre underscore (\_) e mai trattino semplice (-); 
* il primo carattere dell'_eid_ non può mai essere un numero;
* non utilizzare spazi. 

> Per l'_eid_ degli _item_ utilizzare:   
> 
> Item Person: nome della persona in minuscolo, sostituendo spazi e segni di interpunzione con underscore (\_):  
> es. Per l'_item_ di Giovanni dell’Incisa, l'_eid_ sarà "giovanni_dell_incisa"  
> 
> Item Text: ripetere il _title_ dell'_item_, sostituendo spazi e segni di interpunzione con underscore (\_); nel caso dei testi citati attraverso _incipit_, abbreviare il titolo in modo opportuno:  
>  es. Fam. I 1 diventa "Fam_I_1" 
>  es. Rvf 84 diventa "Rvf_84"    
>  es. "I’provai già quanto la soma è grave" diventa "I_provai".  
> Item Manuscript: indicare sinteticamente la sigla della biblioteca e/o del fondo come riportata nel [repository dei manoscritti](repository.md), seguita da underscore (\_) e dalla segnatura. Nel caso in cui la segnatura del codice comprenda punti, questi sono sostituiti da underscore (\_):  
> es. "Plut_XL_1" 🚧  
> es. "Bodl_Can_It_66" 🚧  

> Per gli _eid_ di singole parti (ad es. Events, Hands, Edits, etc.), consultare le linee guida delle relative _parts_.  

⚠️ È fondamentale che l'_eid_ sia univoco e non abbia doppioni.  
Il compilatore deve perciò in primo luogo verificare nel [repository](repository.md) se all'_item_ da descrivere è già stato attribuito un _eid_, e ricorrere a quello in caso positivo.  
Diversamente, deve procedere ad attribuire un _eid_ all'_item_ facendo attenzione a che non corrisponda ad _eid_ già presenti, ricorrendo sia ai [repository](repository.md) sia alla funzione di [lookup](lookup.md).   


### Riuso di un EID già esistente
Se l'entità di interesse (_item_, _part_, o singolo elemento) è già provvista di un identificativo (_eid_) all'interno di Itinera, occorre copiare quest'ultimo nel campo _EID_/_ID_/_Asserted Id_.    
Per cercare gli _eid_ esistenti è possibile ricorrere ai [repository](repository.md) (solo per determinate entità) o alla funzione di [lookup](lookup.md) (per qualsiasi elemento).   


## External Ids
Per attribuire un identificativo esterno, consultare la sezione relativa in [AssertedId](Asserted_Ids_Brick.md).
