# Strumento di lookup e ricerca _eid_
  
Gli [_eid_](identifiers.md) servono a identificare _item_, parti o singole componenti di Itinera, permettendo il successivo collegamento tra di essi.  

Per individuare _eid_ di _item_ o parti già presenti in Itinera è possibile ricorrere ad uno strumento di ricerca interno al database (_lookup_).  L'_eid_ così individuato può essere successivamente **copiato e incollato** nel campo che si intende compilare. 
 
⚠️ Gli _eid_ degli _item_ compresi nei _corpora_ di Itinera sono consultabili anche nei rispettivi [_repositories_](repository.md). Per ulteriori informazioni sugli _eid_ consultare [questa pagina](identifiers.md).   

La documentazione sul _lookup_ è disponibile [qui](https://myrmex.github.io/overview/cadmus/dev/concepts/lookup).  


## _lookup_ integrato e tool _lookup_

Poiché all'interno di alcune _parts_ si rende necessario più frequentemente richiamare entità, in alcuni casi lo strumento di _lookup_ appare, per comodità, affiancato al campo che ospita l'_eid_. È il caso di [_AssertedId_](Asserted_Ids_Brick.md): 

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/lookup_shape_2.png?raw=true)  

Lo strumento strumento di _lookup_ è integrato anche nella [Referenced Text Part](Referenced_Text_Part.md) e nella sezione [RelatedEntities di Events Part](Events_Part.md#related-entities).

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/lookup_shape_1.png?raw=true)  

Quando lo strumento non è integrato alla parte, è sempre possibile ricorrere ad esso attivandolo attraverso pulsante _toogle tools_ nella parte alta della schermata.

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_off.png?raw=true)  

Cliccandolo, il pulsante si illumina.   
![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_on.png?raw=true)  

Contestualmente, sul lato sinistro della pagina si apre una barra laterale che dà accesso ad una funzionalità denominata _pin lookup_.   
![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/lookup_shape_3.png?raw=true)   


## Funzionamento dello strumento di _lookup_

Lo strumento di _lookup_ ricerca gli _eid_ già presenti e attribuiti ad _item_, parti o singoli elementi all'interno del database. La ricerca si effettua all'interno dei campi in cui l'_eid_ è stato inserito.   

Per la ricerca dell'_eid_ di un _item_, ad esempio, lo strumento interrogherà **soltanto** la parte dell'_item_ deputata ad accogliere il suo _eid_, cioè la [_Metadata Part_](Metadata_Part.md), come nell'esempio:

<img width="189" alt="Schermata 2023-04-06 alle 11 46 04" src="https://user-images.githubusercontent.com/102725489/230340482-47c5eafc-e243-4504-9891-f84f444104a6.png">

Il menu _type_ dello strumento permette di selezionare la _part_ nella quale si intende effettuare la ricerca. Nel paragrafo successivo sono illustrate le modalità di ricerca per gli _eid_ degli _item_, in quello seguente tutte le altre.

### Ricercare l'_eid_ di un _item_

Tutte le entità comprese nei _corpora_ di Itinera sono provviste di un _eid_ depositato nella [_Metadata Part_](Metadata_Part.md).
Per ricercare l'_eid_ di un _item_ già presente nella banca dati attraverso lo strumento di _lookup_, occorre dunque limitare la ricerca alla _Metadata Part_ selezionando dal _type_ **_meta_eid_**.   
Selezionato il _type_, il compilatore inizia a digitare nel campo _pin_ il nome dell'entità da cercare (testo, persona o manoscritto). Lo strumento mostra contestualmente i risultati corrispondenti alla ricerca. Il compilatore può a questo punto selezionare il risultato corrispondente alla ricerca.

> Esempio. Lo strumento mostra i risultati compatibili con la ricerca di "nel", tra cui "francesco_nelli"
> <img width="385" alt="Schermata 2023-04-06 alle 11 56 54" src="https://user-images.githubusercontent.com/102725489/230343471-205c5743-d37e-4cde-b2f5-97485aeace90.png">

Selezionando il risultato desiderato, lo strumento apre la tabella con i dati dell'_item_ relativo.

> Esempio. Tabella con i dati dell'_item_ Francesco Nelli   
> <img width="335" alt="Schermata 2023-04-06 alle 12 04 59" src="https://user-images.githubusercontent.com/102725489/230345255-fe4adf92-1aac-4cc9-846c-ba01887eb955.png">

Dalla tabella il compilatore può così copiare l'_eid_ dell'_item_ e incollarlo nel campo apposito. 

<img width="347" alt="Schermata 2023-04-06 alle 12 12 09" src="https://user-images.githubusercontent.com/102725489/230347475-877fa458-1c92-4149-9105-07fd19ae8088.png">

In alternativa, è possibile copiare l'_eid_ ricorrendo all'[_Id builder_](id_builder.md).


### Ricercare _eid_ di _parts_ ed _elements_

- cercare eid testi
- cercare eid persone
- cercare eid eventi
- cercare eid mss

referenced text solo referenced text

1. se l'item è nei corpora deve esistere e quindi: ha un meta _eid_ e lo stesso _eid_ è usato nelle altre parti
2. alcuni testi e persone non esistono ma possono esistere come puri nomi in altre parti, quindi bisogn verificare che l'_eid_ che non trovo in meta non sia in ref. events

🚧 ovunque il nome _pin_: distinguere tra pin e eid 

Lo strumento è composto dai seguenti campi:  
* **_type_**: permette di indicare a quale tipologia di entità appartiene l'_eid_ ricercato. A seconda del valore selezionato, è possibile effettuare la ricerca tra:
🚧 capire come fare questa lista: spiegando così, o con rinvio a parti/elementi, o citare esplicitamente solo meta\_eid e accennare genericamente a 'tutti gli altri'🚧
  * meta\_eid: gli identificativi degli _item_, quali sono stati registrati in [Metadata Part](Metadata_Part.md);
  * event\_eid: gli identificativi degli eventi 🚧 precisare bene norme di richiamo in base a norme decise per eid eventi 🚧;
  * cod\_matdsc\_eid: gli identificativi delle unità codicologiche;
  * cod\_hand\_eid: gli identificativi delle mani;
  * cod\_decoration\_eid: gli identificativi degli apparati decorativi;
  * cod\_artist\_eid: gli identificativi dei decoratori;
  * cod\_content\_eid: gli identificativi dei testi contenuti nei manoscritti;
  * cod\_edit\_eid: gli identificativi degli interventi di ;
  * 🚧meta\_eid: gli identificativi degli eventi;
  * 🚧meta\_eid: gli identificativi degli eventi;
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
