# EID (_Entity Identifier_)

Ad ogni _item_ e ad alcuni _elements_ è **assegnato da parte del compilatore** un **EID** (_Entity Identifier_), cioè un identificativo interno a Itinera e _human readable_, che ha la funzione di:  
* identificare univocamente l'_item_ o _element_ all'interno del database;
* richiamare l'_item_ o _element_ in un'altra parte del database;
* proiettare l'entità costituita dall'_item_ o _element_ sul [grafo semantico](semantic_graph.md).

La documentazione tecnica relativa all'_eid_ è disponibile [qui](https://myrmex.github.io/overview/cadmus/dev/concepts/lookup).    

## Modalità di inserimento

### Item
Ogni _item_ schedato in Itinera deve essere **obbligatoriamente** associato ad un _eid_.  
Questo è registrato dal compilatore in [Metadata Part](Metadata_Part.md) sotto la voce _identifiers_.  
⚠️ Il compilatore non deve confondere _eid_ e _title_ dell'_item_, che sono due proprietà diverse e con diverse funzioni.  

![Compilazione dell'_eid_ di un _item_](https://github.com/petrarchsitinera/linee-guida/assets/123007762/114ab780-539a-4d8b-a806-b4ea7c304e42)  
> Nell'immagine la compilazione dell'_eid_ di un _item_, redatto secondo le norme precisate oltre e inserito secondo le regole stabilite in [Metadata Part](Metadata_Part.md).

Gli identificativi degli _item_ che fanno parte dei _corpora_ di Itinera sono già assegnati e consultabili nei [repository](repository.md).  

Gli _eid_ delle persone sono consultabili nel [repository dei nomi persona](https://shortest.link/m1EA).  
Gli _eid_ dei testi sono consultabili nel [repository dei testi](https://shortest.link/m1EQ).  
Gli _eid_ dei manoscritti sono consultabili nel repository 🚧. 

### Elements
Ad alcuni _elements_ presenti in singole _parts_ può essere associato un _eid_, quando pertinente.  
L'_eid_ è inserito come testo libero nel campo omonimo.  

![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/f59bf8db-985a-42cc-a205-81fc8d9e1287)
> Nell'immagine la compilazione dell'_eid_ di un _element_ _work_ della _Works Part_ di un _Item Person_: dal momento che in Itinera sono, di norma, provvisti di un _item_ i soli testi di corrispondenza con Petrarca, le altre opere di un autore schedato come _item Person_ sono elencate in questa _part_ e non dotate di un _item_ autonomo. L'assegnazione di un _eid_ garantisce la possibilità di richiamarle quando necessario.

Fatte salve le regole di composizione degli _eid_, esposte di seguito, le modalità di assegnazione di un _eid_ ad un _element_ sono precisate nelle line guida delle relative _parts_.  
Di seguito l'elenco degli _elements_ che prevedono l'assegnazione, facoltativa o obbligatoria, di un _eid_:
🚧🚧🚧
*PersonWorksPart, elemento [_works_]();
*
CodContentsPart.contents.eid
CodDecorationsPart.decorations.eid
CodDecorationsPart.decorations.artists.eid
CodEditsPart.edits.eid
CodHandsPart.hands.eid
CodHandsPart.hands.description.signs.eid
CodMaterialDscPart.units.eid
🚧🚧🚧

## Regole di composizione
Nel caso di nuove immissioni, gli _eid_ si attribuiscono secondo regole specifiche.  
⚠️ Ogni volta che si crea un nuovo _eid_ relativo a una persona, a un testo o a un manoscritto è **obbligatorio** segnalare l'aggiunta in [Clickup](https://app.clickup.com/) per permettere l'aggiornamento del [repository](repository.md).  

Quando si renda necessario **creare** un nuovo _eid_, occorre attenersi alle seguenti regole generali:  
* l'_eid_ si compone di caratteri a-z, 0-9; 
* l'_eid_ non può contenere lettere maiuscole;  
* l'_eid_ non può contenere spazi;
* l'_eid_ non può contenere trattino semplice (-), sostituito eventualmente dall'underscore (\_); 
* il primo carattere dell'_eid_ non può mai essere un numero.

### Eid di persone
Per l'_eid_ degli _item person_, si ricorre al nome della persona ponendo tutte le lettere in minuscolo e sostituendo eventuali spazi e segni di interpunzione con underscore (\_):  
> es.  Giovanni dell’Incisa > giovanni_dell_incisa   

Per gli anonimi non esistono regole specifiche per l'attribuzione dell'_eid_. In linea generale, il compilatore assegna un _eid_ arbitrario componendolo nel modo più esplicito e parlante possibile. Il compilatore presterà la massima attenzione a verificare che l'anonimo inserito non corrisponda ad altro anonimo già presente nel database.  

> es. Il sonetto _Vo' mi negate la virtù che nunca_, proposta di _Rvf_ 166, è scritto da un anonimo. Il suo autore sarà schedato in Itinera avendo come _eid_: anonimo_vo_mi_negate.

### Eid di testi
Per l'_eid_ degli _item text_, si ricorre al _title_ dell'_item_, sostituendo spazi e segni di interpunzione con underscore (\_). Nel caso dei testi citati attraverso l'_incipit_, il titolo va abbreviato in modo opportuno:  
>  es. Fam. I 1 > fam_i_1    
>  es. Rvf 84 > rvf_84    
>  es. I’provai già quanto la soma è grave > i_provai   

Anche nel caso di lettere di redazione gamma o beta, l'_eid_ corrisponde al titolo, opportunamente adattato alle regole di composizione: riporterà dunque per esteso l'indicazione della redazione, gamma o beta.  
> es. Sen. II 1 gamma > sen_ii_1_gamma  

Per l'_eid_ dei testi perduti si riccorre alla sigla "tp" seguita da underscore (\_) e dall'_eid_ del testo da cui si deduce l'esistenza del testo perduto.  
> es. La lettera di Petrarca cui Francesco Nelli risponde con la lettera _Multa expectaram_ è perduta. Tale lettera sarà schedata in Itinera avendo come _eid_ : tp_multa_expectaram.

### Eid di manoscritti
Per l'_eid_ degli _item manuscript_, si indica sinteticamente la sigla della biblioteca e/o del fondo come riportata nel [🚧 repository dei manoscritti](repository.md), seguita da underscore (\_) e dalla segnatura. Nel caso in cui la segnatura del codice comprenda punti, questi sono sostituiti da underscore (\_):  
> es. plut_xl_1 🚧  
> es. bodl_can_it_66 🚧

### Eid di singoli _elements_
Per gli _eid_ di singole parti (ad es. Events, Hands, Edits, etc.), consultare le linee guida delle relative _parts_.  
