# Asserted Composed Id

**Asserted Composed Ids** permette due differenti operazioni:  
* richiamare uno o più identificativi ([_eid_](identifiers.md)), qualificando il richiamo con evenutali indici di affidabilità e fonti a sostegno attraverso l'[Assertion](Assertion_Brick.md);  
* collegare un _item_ o un elemento a risorse esterne al database Itinera.

È possibile creare tanti _Asserted Ids_ quante sono le identificazioni da inserire.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#externalidspart).  

> La struttura della parte è la seguente:  
> * _id_: permette di inserire l'identificativo e i suoi metadati;   
>    * _tag_: permette di attribuire all'identificativo un'etichetta utile ai fini della ricerca;  
>    * _scope_: permette di indicare la fonte in cui è archiviato l'identificativo (Itinera o database esterni);  
>    * _value_: permette di inserire l'identificativo (per le entità di Itinera l'_eid_, ricercabile attraverso lo strumento di [lookup integrato](lookup.md));  
> * _assertion_: compilabile aprendo la finestra a comparsa, permette di attribuire un'indice di affidabilità all'identificazione attraverso [Assertion](Assertion_Brick.md) e di precisarne le [fonti](Docref_Brick.md).  
  

![](https://github.com/petrarchsitinera/linee-guida/blob/e88adcfe6655f13f9f18f6aa7de232fe8d83907b/docs/assets/images/asserted_id.png)  

La parte viene compilata in modo diverso a seconda che si debba richiamare un identificativo interno o stabilire un collegamento con una risorsa esterna.  

## Identificativi interni a Itinera (_eid_)

Per richiamare l'identificativo di un'entità schedata nel database Itinera, compilare i campi come segue:

* _id_:
  * _tag_: lasciare vuoto;
  * _scope_: lasciare vuoto;    
  * _value_: copiare l'[_eid_]((identifiers.md)) dell'entità, individuato consultando i [repositories](repository.md) o attraverso lo strumento di [lookup](lookup.md) ;  
* _assertion_: compilare secondo le modalità previste in [Assertion](Assertion_Brick.md);  

## Identificativi esterni

Per stabilire un collegamento con un'entità presente in una database esterno a Itinera, compilare i campi come segue:  

* _id_:
  * _tag_: lasciare vuoto;
  * _scope_: indicare il nome della banca dati utilizzata;
  * _value_: compilare con l'URI dell'entità nella banca dati utilizzata (per VIAF ricercabile attraverso un _tool_ specifico; cfr. infra);  
* _assertion_: compilare secondo le modalità previste in [Assertion](Assertion_Brick.md);  

### Tool Viaf
Per recuperare **l'identificativo VIAF** è possibile ricorrere ad un _tool_ di ricerca integrato.  
Per usare il _tool_, è necessario attivare il _toogle tools_ dal menu orizzontale che si trova nella parte alta della schermata sulla destra. Il _tool_ è attivo quando il pulsante appare colorato come nell'immagine:  

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_on.png?raw=true)   

Una volta attivato il _tool_, sul lato sinistro della schermata appare l'editor che permette la ricerca di identificativi in _VIAF_.     

![](https://github.com/petrarchsitinera/linee-guida/blob/32a21f598ab1973e807dff0be492e94d155e5c4c/docs/assets/images/tool_viaf.png?raw=true)   

Per cercare un identificativo in VIAF, il compilatore digita nella barra di ricerca il nome della persona di interesse. Un menu a tendina mostra contestualmente i nomi presenti in VIAF. Selezionando il nome della persona desiderata, il sistema ne copia in automatico l'identificativo, che può così essere direttamente incollato nel campo _value_.     

![](https://github.com/petrarchsitinera/linee-guida/blob/7de26f57ea824e0286a03b47055b362667dfcc73/docs/assets/images/tool_viaf2.png?raw=true)


