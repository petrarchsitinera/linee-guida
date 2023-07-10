# Asserted Composite Id

**Asserted Composite Ids** permette di richiamare uno o più identificativi, interni ([_eid_](identifiers.md)) o esterni a Itinera qualificando il richiamo con evenutali indici di affidabilità e fonti a sostegno attraverso l'[Assertion](Assertion_Brick.md);  

È possibile creare tanti _Asserted Composite Ids_ quante sono le identificazioni da inserire.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-bricks-shell/blob/master/projects/myrmidon/cadmus-refs-asserted-ids/README.md#asserted-composite-id).  

L'editor della parte appare come nella figura:  

![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/818301a7-f4a2-446b-bd06-78b2a681a283)

La parte si compone delle seguenti sezioni e appare come nell'immagine:  
* _tag_;
* _scope_;  
* _target_;
* _assertion_.

## Tag
Lasciare vuoto.

## Scope
Permette di indicare di indicare il nome della banca dati utilizzata (es. VIAF o ISNI), **quando l'identificativo è esterno a Itinera**.    
⚠️ Non compilare quando si inseriscono identificativi Itinera.

## Target
Nella finestra _target_ è possibile selezionare o inserire l'identificativo di interesse.  
La compilazione varia a seconda che l'identificativo sia esterno o interno ad Itinera.  
L'editor è impostato di default su "external".  

### Identificativi di _item_ già presenti in Itinera
Per inserire un identificativo interno, il _flag_ "external" deve essere deselezionato.
Con questa modalità è possibile ricercare l'identificativo di un'entità già presente all'interno del database.

#### Ricerca dell'_eid_ di un _item_
Per cercare e richiamare l'_eid_ di un _item_ il compilatore può seguire più strade.  
La modalità principale, presentata di seguito, è quella da preferirsi per evitare errori di identificazione e/o di selezione.

**1)** Nel campo _item_ iniziare a digitare il titolo dell'_item_ di interesse.  
Selezionare l'_item_ di interesse.  
Nel campo _part_ selezionare la parte a cui si intende restringere la ricerca - nel caso dell'_eid_ dell'_item_ Metadata Part.  
Nel campo _pin_ iniziare a digitare l'_eid_, e, una volta individuato quello di interesse, selezionarlo cliccandolo.  
Cliccare quindi il tasto target per salvare la selezione.  
A selezione avvenuta ne compariranno gli estremi (_label_ e _GID_) nella parte alta della finestra _target_.  

![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/c0c83618-b29a-4393-955a-0183e7d1573e)

**2)** Nel campo _pin_ iniziare a digitare l'_eid_, e, una volta individuato quello di interesse, selezionarlo cliccandolo.  
Cliccare quindi il tasto target per salvare la selezione.  
A selezione avvenuta ne compariranno gli estremi (_label_ e _GID_) nella parte alta della finestra _target_.  

**3)** Spuntare il _flag_ "by type".
Dal menu a tendina del campo _part type_ selezionare la parte a cui si intende restringere la ricerca - nel caso dell'_eid_ dell'_item_ Metadata Part.  
Nel campo _pin_ iniziare a digitare l'_eid_, e, una volta individuato quello di interesse, selezionarlo cliccandolo.  
Cliccare quindi il tasto target per salvare la selezione.  
A selezione avvenuta ne compariranno gli estremi (_label_ e _GID_) nella parte alta della finestra _target_.  

> Nella finestra _target_ è presente anche il riquadro a comparsa _pin data_. Cliccandolo mostra una griglia con indicati alcuni dati dell'_item_ a cui afferisce l'_eid_ selezionato in _pin_, e che dunque permette di verificare la correttezza della selezione.


#### Ricerca dell'_eid_ di un _element_
La ricerca dell'_eid_ di un _element_ si effettua con le stesse modalità descritte sopra. Diversamente dalla ricerca dell'_eid_ di un _item_ converrà selezionare dal menu a tendina le parti opportune.  

### Altri identificativi Itinera
### Identificativi esterni


Per stabilire un collegamento con un'entità presente in una database esterno a Itinera, compilare i campi come segue:  

* _id_:
  * _tag_: lasciare vuoto;
  * _scope_: indicare il nome della banca dati utilizzata;
  * _value_: compilare con l'URI dell'entità nella banca dati utilizzata (per VIAF ricercabile attraverso un _tool_ specifico; cfr. infra);  
* _assertion_: compilare secondo le modalità previste in [Assertion](Assertion_Brick.md);  

#### Tool Viaf
Per recuperare **l'identificativo VIAF** è possibile ricorrere ad un _tool_ di ricerca integrato.  
Per usare il _tool_, è necessario attivare il _toogle tools_ dal menu orizzontale che si trova nella parte alta della schermata sulla destra. Il _tool_ è attivo quando il pulsante appare colorato come nell'immagine:  

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_on.png?raw=true)   

Una volta attivato il _tool_, sul lato sinistro della schermata appare l'editor che permette la ricerca di identificativi in _VIAF_.     

![](https://github.com/petrarchsitinera/linee-guida/blob/32a21f598ab1973e807dff0be492e94d155e5c4c/docs/assets/images/tool_viaf.png?raw=true)   

Per cercare un identificativo in VIAF, il compilatore digita nella barra di ricerca il nome della persona di interesse. Un menu a tendina mostra contestualmente i nomi presenti in VIAF. Selezionando il nome della persona desiderata, il sistema ne copia in automatico l'identificativo, che può così essere direttamente incollato nel campo _value_.     

![](https://github.com/petrarchsitinera/linee-guida/blob/7de26f57ea824e0286a03b47055b362667dfcc73/docs/assets/images/tool_viaf2.png?raw=true)




## Assertion
L'_assertion_ è compilabile aprendo la finestra a comparsa e permette di attribuire un'indice di affidabilità all'identificazione proposta secondo il modello [Assertion](Assertion_Brick.md) e di precisarne le [fonti](Docref_Brick.md).  
  
