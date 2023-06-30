# Thesaurus eventi


Il **thesaurus eventi**, unico per tutte le tipologie di _item_, è strutturato come un _thesaurus_ gerarchico.   
Le relazioni che le entità collegate possono intrattenere con l'_item_ in cui l'evento è inserito dipendono dalla tipologia dell'evento.  
Una volta selezionata la tipologia di un evento in _general_, per le entità _related_ sarà possibile selezionare soltanto le relazioni previste per quella tipologia di evento.  

> Ad esempio, dopo aver selezionato _matrimonio_, non sarà possibile selezionare _persona incontrata_ come relazione per il _related_: _matrimonio_ ha infatti come relazioni possibili soltanto _marito_ e _moglie_.

È possibile, se necessario, inserire più elementi _related_ della stessa tipologia.

> Ad esempio, nel caso di più destinatari o di più oggetti inviati afferenti ad un medesimo invio (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

⚠️ Le entità inserite tra i _related_, se presenti in Itinera (in qualità di _item_, _parts_ o _elements_), devono essere richiamate attraverso l'_eid_, secondo le regole stabilite in [_lookup_](lookup.md).  
Le entità inserite tra i _related_ non devono necessariamente esistere come _item_ in Itinera: in questo caso hanno un valore solo 'letterale', perché non possono essere collegate a _item_, _part_ o _element_ esterni all'evento dentro cui sono inserite. Tali entità sono comunque immesse secondo le norme definite per gli [identificativi](identifiers.md) di persone, testi e manoscritti. Se necessario, è sempre possibile, in ogni caso, creare a posteriori un _item_ per le entità inserite in related.  


⚠️⚠️⚠️ Il compilatore deve prestare la massima attenzione alla formalizzazione degli eventi secondo la tassonomia elaborata per Itinera, individuando la corretta tipologia di evento  dal _thesaurus_ (cfr. _infra_). Deve assicurarsi soprattutto che eventi **puntuali**, circoscritti nello spazio e nel tempo, siano descritti in modo altrettanto puntuale all'interno di eventi singoli, anche quando si tratti di eventi logicamente collegati tra loro. Due eventi logicamente e fattualmente collegati come un invio e una ricezione, sono infatti inseriti e descritti come eventi singoli, e collegati attraverso l'uso del _tag_.

Di seguito è fornita la lista degli eventi disponibili, suddivisa per tipologia di _item_.


* [Person](Events_Thesaurus_Person.md)  
* [Work](Events_Thesaurus_Work.md)  
* [Manuscript](Events_Thesaurus_Manuscript.md)  
