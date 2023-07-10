# External IDs Part
**External IDs Part** raccoglie gli identificativi dell'item in risorse esterne, permettendo così di incrociare, in fase di pubblicazione, i dati inseriti nel database di Itinera con quelli presenti altrove.   

La descrizione del modello, basato su [_Asserted Id_](Asserted_Ids_Brick.md), è disponibile su [Github](https://github.com/vedph/cadmus-general#externalidspart).  

Per stabilire un collegamento con un'entità presente in una database esterno a Itinera, compilare i campi come segue:  

* _id_:
  * _tag_: lasciare vuoto;
  * _scope_: indicare il nome della banca dati utilizzata;
  * _value_: compilare con l'URI dell'entità nella banca dati utilizzata (per VIAF ricercabile attraverso un _tool_ specifico; cfr. infra);  
* _assertion_: compilare secondo le modalità previste in [Assertion](Assertion_Brick.md);  

⚠️ Nello _scope_ la risorsa è indicata con i nomi nella forma specificata nei paragrafi successivi.

## External IDs obbligatori

Per gli Item Person relativi a soggetti storicamente esistiti ed individuabili si inseriscono **obbligatoriamente** gli identificativi presenti in:

- **VIAF**
- **ISNI** 

Per recuperare **l'identificativo VIAF** è possibile ricorrere al tool di ricerca (vedi sotto) presente in Cadmus.  

Per **l'identificativo ISNI**, consultare il database disponibile a questo [link](https://isni.org/page/search-database/).  
Individuato il record ISNI relativo alla persona, copiarne l'identificativo nel campo _value_.

### Tool Viaf
Per recuperare **l'identificativo VIAF** è possibile ricorrere ad un _tool_ di ricerca integrato.  
Per usare il _tool_, è necessario attivare il _toogle tools_ dal menu orizzontale che si trova nella parte alta della schermata sulla destra. Il _tool_ è attivo quando il pulsante appare colorato come nell'immagine:  

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_on.png?raw=true)   

Una volta attivato il _tool_, sul lato sinistro della schermata appare l'editor che permette la ricerca di identificativi in _VIAF_.     

![](https://github.com/petrarchsitinera/linee-guida/blob/32a21f598ab1973e807dff0be492e94d155e5c4c/docs/assets/images/tool_viaf.png?raw=true)   

Per cercare un identificativo in VIAF, il compilatore digita nella barra di ricerca il nome della persona di interesse. Un menu a tendina mostra contestualmente i nomi presenti in VIAF. Selezionando il nome della persona desiderata, il sistema ne copia in automatico l'identificativo, che può così essere direttamente incollato nel campo _value_.     

![](https://github.com/petrarchsitinera/linee-guida/blob/7de26f57ea824e0286a03b47055b362667dfcc73/docs/assets/images/tool_viaf2.png?raw=true)



## External IDs facoltativi

È possibile aggiungere ulteriori identificativi, se opportuno o utile. Si segnalano, in particolare:
* Dbpedia
* WorldCat Identities
* Wikidata
* Library of Congress Authority ID
* MOL – Manus online (indici)
* E-codices (person index)
* Dizionario Biografico degli Italiani
* Référentiel d&#39;autorités &quot;personnes&quot; IRHT
* ULAN ID (artisti: copisti e decoratori)


## Soggetti non identificati storicamente
In presenza di soggetti non individuati storicamente è possibile utilizzare questa parte per proporre ipotesi di identificazione.  

Se per un soggetto non individuato storicamente è possibile proporre una o più ipotesi di identificazione con una persona schedata in Itinera come Item Person, è necessario creare un Item Person relativo al soggetto non individuato; nella relativa _External Ids Part_ è creato un [AssertedId](Asserted_Ids_Brick.md#identificativi-interni-a-itinera-eid) che ha come _value_ l'_eid_ del personaggio noto. Naturalmente, è possibile, grazie all'_Assertion_ esprimere l'attendibilità e le fonti di tale proposta di identificazione.  

> Una simile procedura si osserva, ad esempio, nel caso di nomi d'autore attestati dalla tradizione di cui non è possibile stabilire l'identità storica; per cui si veda il campo [Author](Literary_Work_Part.md#authors) dell'Item Text).  


## Save ⚠️ 

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.

