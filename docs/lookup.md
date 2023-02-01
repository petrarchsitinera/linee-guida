# Strumento di lookup

Per la ricerca di _eid_ già esistenti in Itinera è possibile ricorrere a uno strumento di ricerca interno al database (_lookup_).  
Inoltre, per alcuni _item_ e _parts_ è possibile consultare l'elenco degli _eid_ utilizzati nei [repository dedicati](repository.md).  
 
⚠️ Gli _eid_ sono identificativi che permettono di richiamare un'entità (_item_, _part_ o _element_): per ulteriori informazioni consultare [questa pagina](identifiers.md).   

## Lookup e campi 
Nella banca dati Itinera gli _eid_ sono ospitati da campi denominati _EID_ o _ID_ o, se sono accompagnati da un'asserzione, [AssertedId](Asserted_Ids_Brick.md).  


-a cosa serve
-tipo: integrato in campo (asserted id e altri casi) o attivabile con tool
-cosa fa: 
  -pin
  -EID builder (casi in cui pescare solo pin, o in cui premettere id item)
  Per **richiamare un _item_** è necessario richiamarne l'_eid_: anche in questo caso è possibile ricorrere alla funzione di [lookup](lookup.md).  

Per **richiamare una _part_** è necessario richiamarne l'_eid_, cui deve essere premesso, separato da "/", l'identificativo dell'_item_ (la voce _item ID_ nella finestra di [lookup](lookup.md)).  

  -selezionare eid e copiare/importare



### ⚠️ 🚧 RIASSUNTO FINALE DI IDENTIFICATIVI
### ⚠️ 🚧 CONTROLLA TUTTI QUESTI CAMPI E VERIFICA SE CON QUANTO DETTO IN EID, ASSERTED ID E LOOKUP le spiegazioni tornano

Item Text  
-Literary Work Part. author > Asserted id
(-External Id > non lo usiamo)
-Referenced Text Part. target id > id + lookup interno + assertion esterna
-Related Persons Part > Asserted id
-Witness > id + lookup esterno

Item Person
-External Id > Asserted id (sia per db esterni; nome di piuma)
-PersonWorksPart > id + lookup esterno

Item Ms
-MatDescr > eid: regole
-Watermarks > Asserted id (Briquet)
-HandsPart > eid: regole
-HandsPart > signs > eid: regole
-DecorationPart > eid: regole
-DecorationPart > Artist > sia eid sia Asserted id
-ContentsPart > id + lookup esterno
-EditsPart > eid: regole

EventsPart > eid regole
EventsPart > related > id + lookup interno
