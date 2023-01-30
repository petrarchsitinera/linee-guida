# Regole per identificativi e authority file
Per ogni _item_ e per alcune delle sue parti, Itinera si serve di:
* un identificativo interno _human readable_ (**EID**), che permette di identificare e, ove necessario, richiamare le entità di interesse all'interno del database;  
* eventuali identificativi esterni (**External Ids**), che permettono di collegarli a risorse esterne al database Itinera.  

⚠️ La compilazione dell'_eid_ degli _item_ è obbligatoria [cfr. Metadata Part](Metadata_Part.md): senza di esso risulta impossibile stabilire un collegamento tra gli _item_.  

## EID
Nei casi in cui sia necessario **creare ed attribuire** un _eid_, è necessario attenersi alle seguenti regole generali:  
* l'_eid_ deve essere composto esclusivamente con i caratteri a-z, 0-9; 
* non utilizzare lettere maiuscole;  
* utilizzare sempre underscore (\_) e mai trattino semplice (-); 
* il primo carattere dell'_eid_ non può mai essere un numero;
* non utilizzare spazi. 

> Per l'_eid_ degli _item_ utilizzare:   
> 
> 🚧 Item Person: nome della persona in minuscolo, senza spazi né segni di interpunzione:  
> es. Per l'_item_ di Giovanni dell’Incisa, l'_eid_ sarà "giovannidellincisa"  
> 
> 🚧 Item Text: ripetere il _title_ dell'_item_ sostituendo gli spazi con punto:
>  es. Fam. I 1 diventa "Fam.I_1" "Fam_I_1" "Fam.I1" "Fam.I.1"
>  
> 🚧 Item Manuscript:
> es. "Firenze_BML_Plut.XL.1"?

> Per gli _eid_ di singole parti (ad es. Events, Hands, Edits, etc.), consultare le linee guida delle relative _parts_.  

⚠️ È fondamentale che l'_eid_ sia univoco e non abbia doppioni.  
Il compilatore deve perciò in primo luogo verificare nel [repository](repository.md) se all'_item_ da descrivere è già stato attribuito un _eid_, e ricorrere a quello in caso positivo.  
Diversamente, deve procedere ad attribuire un _eid_ all'_item_ facendo attenzione a che non corrisponda ad _eid_ già presenti, ricorrendo sia ai [repository](repository.md) sia alla funzione di [lookup](lookup.md).   

Per **richiamare un _item_** è necessario richiamarne l'_eid_: anche in questo caso è possibile ricorrere alla funzione di [lookup](lookup.md).  
Per **richiamare una _part_** è necessario richiamarne l'_eid_, cui deve essere premesso, separato da "/", l'identificativo dell'_item_ (la voce _item ID_ nella finestra di [lookup](lookup.md).  

In alcuni casi, all'_eid_ può essere associata una [Assertion](Asserted_Ids_Brick.md).   


## External Ids
Per attribuire un identificativo esterno, consultare la sezione relativa in [AssertedId](Asserted_Ids_Brick.md).
