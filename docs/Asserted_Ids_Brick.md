# Asserted Ids
**Asserted Ids** permette due differenti operazioni:  
* richiamare uno o più identificativi ([_eid_](identifiers.md)), qualificando i dati con una [Assertion](Assertion_Brick.md), ovvero con indice di affidabilità e fonti a sostegno;  
* collegare un _item_ o un elemento ad una o più entità schedate in database esterni.

È possibile creare tanti _Asserted Ids_ quante sono le identificazioni.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#externalidspart).  

> La struttura della parte è identica sia che venga utilizzata per richiamare un identificativo interno che per stabilire un collegamento con un database esterno.  
> Soltanto la compilazione ne risulta differenziata.  
> * _id_: sezione che permette di inserire l'identificativo e i suoi metadati;   
>    * _tag_: permette di attribuire all'identificativo un'etichetta utile ai fini della ricerca;  
>    * _scope_: permette di indicare la fonte in cui è archiviato l'identificativo (Itinera o database esterno);  
>    * _value_: permette di inserire l'identificativo (per le entità di Itinera l'_eid_, ricercabile attraverso lo strumento di [lookup integrato](lookup.md));  
> * _assertion_: sezione, attivabile con finestra a comparsa, permette di attribuire un'indice di affidabilità all'identificazione attraverso [Assertion](Assertion_Brick.md) e di precisarne le [fonti](Docref_Brick.md).  
  

![](https://github.com/petrarchsitinera/linee-guida/blob/e88adcfe6655f13f9f18f6aa7de232fe8d83907b/docs/assets/images/asserted_id.png)  


## Identificativi interni a Itinera (_eid_)

Per richiamare l'identificativo di un'entità schedata nel database Itinera, compilare i campi nel seguente modo:

* _id_:
  * _tag_: lasciare vuoto;
  * _scope_: lasciare vuoto (🚧?) 
  * _value_: compilare con l'[_eid_]((identifiers.md)) dell'entità, ricercandolo tramite [lookup](lookup.md) e nei [repositories](repository.md);  
* _assertion_: compilare secondo le modalità previste in [Assertion](Assertion_Brick.md);  

## Identificativi esterni

Per stabilire un collegamento con un'entità schedata in una database esterno a Itinera, compilare i campi nel seguente modo:  

* _id_:
  * _tag_: lasciare vuoto;
  * _scope_: indicare il nome della banca dati utilizzata.
  * _value_: compilare con l'URI dell'entità nella banca dati utilizzata (per VIAF ricercabile attraverso un _tool_ specifico; cfr. infra);  
* _assertion_: compilare secondo le modalità previste in [Assertion](Assertion_Brick.md);  

Per 


-utilizzo di external id come part autonoma negli item  
-come compilare
-come compilare value: 
  -tool viaf (magari pagina autonoma linkata)


