#ID builder

NON VI SERVE ANCORA - In corso


- per cercare eid di testi
- per cercare eid di persone
- cercare cercare eid eventi
- cercare eid mss

referenced text solo referenced text

1. se l'item è nei corpora deve esistere e quindi: ha un meta _eid_ e lo stesso _eid_ è usato nelle altre parti
2. alcuni testi e persone non esistono ma possono esistere come puri nomi in altre parti, quindi bisogn verificare che l'_eid_ che non trovo in meta non sia in ref. events




Lo strumento è composto dai seguenti campi:  
* **_type_**: permette di indicare a quale tipologia di entità appartiene l'_eid_ ricercato. A seconda del valore selezionato, è possibile effettuare la ricerca tra:
🚧 capire come fare questa lista: spiegando così, o con rinvio a parti/elementi, o citare esplicitamente solo meta\_eid e accennare genericamente a 'tutti gli altri'🚧
  * meta\_eid: gli identificativi degli _item_, quali sono stati registrati in [Metadata Part](Metadata_Part.md);
  * event\_eid: gli identificativi degli eventi 🚧 precisare bene norme di richiamo in base a norme decise per eid eventi 🚧;

 
* **_pin_**: permette la ricerca e la selezione dell' 🚧 _eid_ 🚧: digitando alcune lettere compaiono gli _eid_ che corrispondono alla ricerca; selezionare tra questi il valore desiderato;  
* **_ID builder_**: permette di importare 🚧 l'_eid_ 🚧 che si desidera copiare nel campo.  
 È costituito da un **campo testuale** libero e da una **tabella** di valori. La tabella offre alcune informazioni sull'_eid_ come l'_item_ o la _part_ di appartenenza, in modo da favorire l'identificazione. Cliccando sul segno _+_ nella tabella è possibile importare uno o più 🚧 identificativi 🚧 nel campo soprastante. 
 Se il _pin_ è univoco (ad es. l'_eid_ di un _item_) è importato il solo _pin_; se non è univoco (ad es. l'_eid_ di alcune _parts_), è necessario premettere all'_eid_ l'identificativo dell'_item_ o della _part_, separato da "/".  
 
  > Ad es. l'_eid_ ricercato corrisponde a un Item Person, deve essere importato soltanto il _pin_.  
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/e4dd1632b6f24b831811da7cc88950d6ea0cdf3f/docs/assets/images/lookup_builder1.png?raw=true)  
  > Ad es. se l'_eid_ ricercato corrisponde a una sottoparte, come un elemento _Hand_, si deve premettere all'_eid_ l'identificativo del Manuscript Item, perché l'etichetta convenzionale assegnata alle mani è univoca soltanto relativamente ad esso.   
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/e4dd1632b6f24b831811da7cc88950d6ea0cdf3f/docs/assets/images/lookup_builder2.png?raw=true)    
 
Una volta inserito l'_eid_ desiderato nel campo testuale cliccare il segno di spunta blu; apparirà il messaggio **"ID copied"** e sarà possibile copiare l'_eid_ nel campo _EID_ desiderato.







************************************++

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
