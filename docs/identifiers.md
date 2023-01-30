# Regole per identificativi e authority file

## Creare e attribuire un identificativo univoco interno a Itinera (EID)   

Nei casi in cui sia necessario creare ed attribuire un _eid_, è necessario attenersi alle seguenti regole generali:  
* l'_eid_ deve essere composto esclusivamente con i caratteri A-Z, 0-9; 
* utilizzare sempre underscore (\_) e mai trattino semplice (-); 
* il primo carattere dell'_eid_ non può mai essere un numero.
* 🚧🚧🚧 ALTRE REGOLE? Spazi, virgole, etc. 🚧🚧🚧  

In alcuni casi è necessario osservare particolari regole di composizione: consultare le linee guida delle relative _parts_.  

🚧 SPECIFICARE AD LOCA REGOLE PER: Referenced Text Part. target id  (se non in DB, incipit testo), Witness (se non in DB, segnatura), PersonWorksPart (se non in DB titolo invalso, facoltativo); MatDescr (u1, etc.); HandsPart (mano a etc); HandsPart.signs (rimando a repository o libero); DecorationPart (dec1 etc.); DecorationPart.Artist(se non in db, facoltativo e libero); ContentsPart (se non in DB titolo invalso, facoltativo); EditsPart (edit 1 etc.); EventsPart (boh?)

## Creare e attribuire un identificativo esterno 

Asserted Id


## Cercare e richiamare un identificativo univoco (EID) all'interno del database

un Asserted ID punta sempre a eid già esistente e ha sempre lookup quindi da Asserted id link a questa pagina 



### RIASSUNTO

Eid: regole di composizione degli eid
Come cercare gli eid: lookup
 sia con eid semplice + lookup
 sia con Asserted Id
Come puntare fuori: 
 con Asserted Id



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




Potranno essere cercati in lookup: metti link a spiegazione, che sia in IDS o forse meglio in pagina autonoma

Descrivi funzionamento EID builder
