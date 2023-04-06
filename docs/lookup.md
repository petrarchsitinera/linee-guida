# Strumento di lookup e ricerca _eid_
  
Gli [_eid_](identifiers.md) servono a identificare _item_, parti o singole componenti di Itinera, permettendo il successivo collegamento tra di essi.  

Per individuare _eid_ di _item_ o parti già presenti in Itinera è possibile ricorrere ad uno strumento di ricerca interno al database (_lookup_).  L'_eid_ così individuato può essere successivamente **copiato e incollato** nel campo che si intende compilare. 
 
⚠️ Gli _eid_ degli _item_ compresi nei _corpora_ di Itinera sono consultabili anche nei rispettivi [_repositories_](repository.md). Per ulteriori informazioni sugli _eid_ consultare [questa pagina](identifiers.md).   

La documentazione sul _lookup_ è disponibile [qui](https://myrmex.github.io/overview/cadmus/dev/concepts/lookup).  


## _Lookup_ integrato e tool di _lookup_

Poiché all'interno di alcune _parts_ si rende necessario più frequentemente richiamare entità, in alcuni casi lo strumento di _lookup_ appare, per comodità, affiancato al campo che ospita l'_eid_. È il caso di [_AssertedId_](Asserted_Ids_Brick.md): 

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/lookup_shape_2.png?raw=true)  

Lo strumento strumento di _lookup_ è integrato anche nella [Referenced Text Part](Referenced_Text_Part.md) e nella sezione [RelatedEntities di Events Part](Events_Part.md#related-entities).

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/lookup_shape_1.png?raw=true)  

Quando lo strumento non è integrato alla parte, è sempre possibile ricorrere ad esso attivandolo attraverso pulsante _toogle tools_ nella parte alta della schermata.

![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_off.png?raw=true)  

Cliccandolo, il pulsante si illumina.   
![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_on.png?raw=true)  

Contestualmente, sul lato sinistro della pagina si apre una barra laterale che dà accesso alla funzionalità di ricerca.   
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

In alternativa, è possibile copiare l'_eid_ ricorrendo all'[_ID builder_](ID_builder.md).

⚠️⚠️⚠️ L'_eid_ e il _pin_ riportati nella tabella **corrispondono soltanto** nella ricerca di _eid_ di _item_. **ATTENZIONE a non confonderli** in tutti gli altri casi.

### Ricercare _eid_ di _parts_ ed _elements_

Lo strumento di _lookup_ permette di ricercare anche _eid_ di singole _parts_ ed _elements_ selezionando altre voci di _type_.
Consultare [_ID builder_](ID_builder.md).


