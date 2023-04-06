# Regole per identificativi e authority file

Per ogni _item_ e per alcune _parts_ e _elements_, Itinera si serve di:
* un identificativo interno _human readable_ (**EID**), che permette di identificare e, ove necessario, richiamare le entità di interesse all'interno del database;  
* eventuali identificativi esterni (**External Ids**), che permettono di collegare gli _item_ a risorse esterne al database Itinera.  

## EID
Gli _eid_ sono identificativo interni _human readable_ univoci che permettono di identificare ed eventualmente richiamare _item_, _parts_ ed _elements_ all'interno del database.   

La documentazione relativa all'_eid_ è disponibile [qui](https://myrmex.github.io/overview/cadmus/dev/concepts/lookup).    

Ad ogni _item_ è **obbligatoriamente** associato un _eid_, da registrare in [Metadata Part](Metadata_Part.md).  

⚠️⚠️⚠️ Il compilatore non deve confondere _eid_ e _title_ dell'_item_, che sono due proprietà diverse e con diverse funzioni.   

### EID di _item_ inclusi nei _corpora_ Itinera
Gli identificativi degli _item_ che fanno parte dei _corpora_ di Itinera sono già assegnati e consultabili nel [repository](repository.md).  

Gli _eid_ delle persone sono consultabili nel [repository dei nomi persona](https://shortest.link/m1EA).  
Gli _eid_ dei testi sono consultabili nel [repository dei testi](https://shortest.link/m1EQ).  
Gli _eid_ dei manoscritti sono consultabili nel repository 🚧. Nel caso degli Item Manuscript si ricorre ad ulteriori identificativi per singole _parts_ o _elements_. 

### Regole di composizione di nuovi EID 
Nel caso di nuove immissioni, gli _eid_ si attribuiscono secondo le regole specifiche.  
Ogni volta che si crea un nuovo _eid_ è **obbligatorio** segnalare l'aggiunta in clickup per permettere l'aggiornamento del [repository](repository.md).  

Quando si renda necessario **creare** un nuovo _eid_, occorre attenersi alle seguenti regole generali:  
* l'_eid_ si compone di caratteri a-z, 0-9; 
* l'_eid_ non può contenere lettere maiuscole;  
* l'_eid_ non può contenere spazi;
* l'_eid_ non può contenere trattino semplice (-), sostituito eventualmente dall'underscore (\_); 
* il primo carattere dell'_eid_ non può mai essere un numero.  

Per l'_eid_ degli _item person_, si ricorre al nome della persona ponendo tutte le lettere in minuscolo e sostituendo eventuali spazi e segni di interpunzione con underscore (\_):  
> es.  Giovanni dell’Incisa > giovanni_dell_incisa   

Per gli anonimi non esistono regole specifiche per l'attribuzione dell'_eid_. In linea generale, il compilatore assegna un _eid_ arbitrario componendolo nel modo più esplicito e parlante possibile. Il compilatore presterà la massima attenzione a verificare che l'anonimo inserito non corrisponda ad altro anonimo già presente nel database.  

> es. Il sonetto _Vo' mi negate la virtù che nunca_, proposta di _Rvf_ 166 è anonimo. Il suo autore sarà schedato in Itinera avendo come _eid_: anonimo_vo_mi_negate.  

Per l'_eid_ degli _item text_, si ricorre al _title_ dell'_item_, sostituendo spazi e segni di interpunzione con underscore (\_). Nel caso dei testi citati attraverso l'_incipit_, il titolo va abbreviato in modo opportuno:  
>  es. Fam. I 1 > fam_i_1    
>  es. Rvf 84 > rvf_84    
>  es. I’provai già quanto la soma è grave > i_provai   

Per l'_eid_ dei testi perduti si riccorre alla sigla "tp" seguita da underscore (\_) e dall'_eid_ del testo da cui si deduce l'esistenza del testo perduto.  
> es. La lettera di Petrarca cui Francesco Nelli risponde con la lettera _Multa expectaram_ è perduta. Tale lettera sarà schedata in Itinera avendo come _eid_ : tp_multa_expectaram.  

Per l'_eid_ degli _item manuscript_, si indica sinteticamente la sigla della biblioteca e/o del fondo come riportata nel [🚧 repository dei manoscritti](repository.md), seguita da underscore (\_) e dalla segnatura. Nel caso in cui la segnatura del codice comprenda punti, questi sono sostituiti da underscore (\_):  
> es. plut_xl_1 🚧  
> es. bodl_can_it_66 🚧  

Per gli _eid_ di singole parti (ad es. Events, Hands, Edits, etc.), consultare le linee guida delle relative _parts_.  


## External Ids
Per attribuire un identificativo esterno, consultare la sezione relativa in [AssertedId](Asserted_Ids_Brick.md).
