# Asserted Composite Id

**Asserted Composite Ids** permette di richiamare uno o più identificativi, siano interni ([_eid_](identifiers.md)) o esterni a Itinera, qualificando il richiamo con evenutali indici di affidabilità e fonti a sostegno attraverso la compilazione dell'[Assertion](Assertion_Brick.md);  

È possibile creare tanti _Asserted Composite Ids_ quante sono le identificazioni da inserire.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-bricks-shell/blob/master/projects/myrmidon/cadmus-refs-asserted-ids/README.md#asserted-composite-id).  

## Ids

Ogni elemento _id_ è composto dai seguenti campi:  
* _tag_;
* _scope_;  
* _target_;
* _assertion_.

![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/818301a7-f4a2-446b-bd06-78b2a681a283)

### Tag
Lasciare vuoto.

### Scope
Permette di indicare di indicare il nome della banca dati utilizzata (es. VIAF o ISNI), quando l'identificativo è **esterno a Itinera**.    

⚠️⚠️⚠️ Il campo **NON** va compilato quando si inseriscono identificativi Itinera. ⚠️⚠️⚠️


### Target
Il campo _target_ permette di selezionare o di inserire manualmente l'identificativo di interesse. La compilazione varia a seconda che l'identificativo sia esterno o interno ad Itinera. L'editor è impostato di default su _external_.  

#### Identificativi di _item_ già presenti in Itinera
Per inserire un identificativo interno a Itinera, il _flag_  _external_ **deve** essere deselezionato.
Con questa modalità è possibile ricercare l'identificativo di un'entità già presente all'interno del database.

##### Ricerca dell'_eid_ di un _item_
L'_eid_ di un _item_ può essere cercato in più modi. La modalità principale, presentata di seguito, è quella da preferirsi per evitare errori di identificazione e/o di selezione.

**1)** Nel campo _item_ iniziare a digitare il titolo dell'_item_ di interesse.  
Selezionare l'_item_ di interesse.  
Nel campo _part_ selezionare la parte a cui si intende restringere la ricerca - nel caso dell'_eid_ dell'_item_ selezionare _Metadata Part_.  
Nel campo _pin_ iniziare a digitare l'_eid_, e, una volta individuato quello di interesse, selezionarlo cliccandolo.  
Cliccare quindi il tasto _target_ per salvare la selezione.  
A selezione avvenuta ne compariranno gli estremi (_label_ e _GID_) nella parte alta della finestra _target_.  

![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/c0c83618-b29a-4393-955a-0183e7d1573e)

**2)** Nel campo _pin_ iniziare a digitare l'_eid_, e, una volta individuato quello di interesse, selezionarlo cliccandolo.  
Cliccare quindi il tasto target per salvare la selezione.  
A selezione avvenuta ne compariranno gli estremi (_label_ e _GID_) nella parte alta della finestra _target_.  

**3)** Spuntare il _flag_ "by type".
Dal menu a tendina del campo _part type_ selezionare la parte a cui si intende restringere la ricerca - nel caso dell'_eid_ dell'_item_ selezionare _Metadata Part_.    
Nel campo _pin_ iniziare a digitare l'_eid_, e, una volta individuato quello di interesse, selezionarlo cliccandolo.  
Cliccare quindi il tasto target per salvare la selezione.  
A selezione avvenuta ne compariranno gli estremi (_label_ e _GID_) nella parte alta della finestra _target_.  

> Nella finestra _target_ è presente anche il riquadro a comparsa _pin data_. Cliccandolo mostra una griglia con indicati alcuni dati dell'_item_ a cui afferisce l'_eid_ selezionato in _pin_, e che dunque permette di verificare la correttezza della selezione.

> Questa modalità di ricerca è disponibile come [tool di ricerca autonomo](lookup_tool.md), indipendente da _Asserted Composite Id_ e utile per ricerche generiche sulle entità presenti nel database.  


##### Ricerca dell'_eid_ di un _element_
La ricerca dell'_eid_ di un _element_ si effettua con le stesse modalità descritte sopra. Diversamente dalla ricerca dell'_eid_ di un _item_ converrà selezionare dal menu a tendina le parti opportune.  

#### Altri identificativi Itinera
Selezionando il _flag_ "external" è possibile richiamare entità, dotate o meno di un identificativo all'interno di Itinera, per le quali non è prevista la compilazione di un _item_.  
⚠️ Per verificare se a tali entità sia già stato attribuito un _eid_, consultare i [repository](repository.md).  
⚠️ Se l'entità non dispone di un _eid_, crearlo secondo le norme di composizione degli [eid](identifiers.md) e segnalare l'aggiunta in [Clickup](https://app.clickup.com/) per permettere l'aggiornamento del [repository](repository.md).   

Nella finestra _target_ compilare i campi:
* _label_: inserire il nome dell'entità in forma _human-friendly_, secondo le norme indicate per i metadati degli item;
* _GUID_: inserire l'_eid_ dell'entità.

Cliccare quindi il tasto target per salvare la selezione.  
A selezione avvenuta ne compariranno gli estremi (_label_ e _GID_) nella parte alta della finestra _target_.  

### Assertion
L'_assertion_ è compilabile aprendo la finestra a comparsa e permette di attribuire un'indice di affidabilità all'identificazione proposta secondo il modello [Assertion](Assertion_Brick.md) e di precisarne le [fonti](Docref_Brick.md).  
  
