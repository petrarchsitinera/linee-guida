# Database bibliografico 

Il database bibliografico raccoglie tutta la bibliografia impiegata nella descrizione degli _item_ ed è accessibile:

* da [_Bibliography_](https://itinera.unisi.it/#/biblio) nel menu orizzontale nella parte alta della schermata, come nell'immagine:

<img width="624" alt="Schermata 2023-04-04 alle 15 50 33" src="https://user-images.githubusercontent.com/102725489/229814240-b6ed1a8d-4f43-4d05-b3ab-0cc0e6846132.png">


* dalla [_Bibliography Part_](External_Bibliography_Part.md) di un singolo _item_.

## Voci bibliografiche

Ogni voce bibliografica inserita costituisce una singola _entry_. Le _entries_ si distinguono in:
- _works_: singole voci bibliografiche;
- _containers_: voci bibliografiche che ne contengono altre (ad es. periodici, atti di convegno, cataloghi, ecc.). 

## Bibliografia ITINERA

La schermata iniziale del database bibliografico mostra la lista di tutte le voci bibliografiche semplici già inserite (_works_).

<img width="1438" alt="Schermata 2023-04-06 alle 12 37 26" src="https://user-images.githubusercontent.com/102725489/230355344-ab20ad59-3087-44b6-976f-07e38effd044.png">

Per visualizzare la lista dei _containers_, spuntare il flag relativo.  

<img width="1336" alt="Schermata 2023-04-06 alle 13 31 44" src="https://user-images.githubusercontent.com/102725489/230364816-fae74ce9-d1ac-415a-97c3-62caded0ef3d.png">


### Cercare voci bibliografiche

Per cercare una voce bibliografica già inserita, è possibile ricorrere alla maschera di ricerca nella parte sinistra dello schermo compilando almeno uno dei campi.

<img width="1438" alt="Schermata 2023-04-06 alle 13 26 18" src="https://user-images.githubusercontent.com/102725489/230363800-0862790d-77d5-4a63-9375-f52a9e37ef84.png">


### Visualizzare, modificare o eliminare voci bibliografiche

Usando i pulsanti a sinistra di ogni voce, è possibile visualizzare, modificare o eliminare le _entries_ relative.

<img width="799" alt="Schermata 2023-04-06 alle 12 54 22" src="https://user-images.githubusercontent.com/102725489/230357314-a9ef4bb7-7bce-4954-81e0-87ebc8f90a37.png">

⚠️⚠️⚠️ **ATTENZIONE**: Il compilatore deve prestare la massima attenzione in fase di immissione e salvataggio dei dati. Modificare o eliminare una _entry_ nel database bibliografico ha infatti ricadute su **tutti gli _item_** che fanno riferimento alla relativa voce bibliografica - si veda, in particolare, le istruzioni relative alla [_key_](bibliodb.md#key). 

#### Visualizzare voci bibliografiche

Selezionando il pulsante _view_ di una _entry_, è possibile visualizzare nella parte bassa della schermata la voce bibliografica per esteso.

<img width="1158" alt="Schermata 2023-04-06 alle 12 58 52" src="https://user-images.githubusercontent.com/102725489/230358611-a7ca6324-ed62-46f7-9c32-389d908ac5de.png">


#### Modificare voci bibliografiche

Selezionando il pulsante _edit_ di una _entry_, è possibile modificare la voce bibliografica intervenendo nei campi della finestra che si apre nella parte bassa della schermata (vedi più oltre).

⚠️⚠️⚠️ **ATTENZIONE**: Il compilatore deve prestare la massima attenzione in fase di immissione e salvataggio dei dati. Modificare o eliminare una _entry_ nel database bibliografico ha infatti ricadute su **tutti gli _item_** che fanno riferimento alla relativa voce bibliografica - si veda, in particolare, le istruzioni relative alla [_key_](bibliodb.md#key). 

<img width="1440" alt="Schermata 2023-04-06 alle 13 03 57" src="https://user-images.githubusercontent.com/102725489/230359620-b3e4b87c-63c8-4124-8d51-23def0434a4c.png">


#### Eliminare voci bibliografiche

Selezionando il pulsante _delete_ di una _entry_, è possibile eliminare la voce bibliografica relativa. Un pop-up chiede conferma dell'azione.

⚠️⚠️⚠️ **ATTENZIONE**: Eliminare una _entry_ nel database bibliografico ha ricadute su **tutti gli _item_** che fanno riferimento alla relativa voce bibliografica. 
 

### Aggungere voci bibliografiche

Per creare una nuova voce bibliografica cliccare sul pulsante _+new_.

<img width="1436" alt="Schermata 2023-04-06 alle 13 35 04" src="https://user-images.githubusercontent.com/102725489/230365400-d245be08-66df-4a28-8989-520dbdeff806.png">

Nella parte bassa della schermata si aprirà una finestra in cui sarà possibile editare i campi relativi alla voce da aggiungere.

<img width="1431" alt="Schermata 2023-04-06 alle 13 39 58" src="https://user-images.githubusercontent.com/102725489/230366351-3a267fc1-eccd-48b8-8742-db65b0d6d172.png">

È possibile aggiungere voci bibliografiche semplici (_work_) e contenitori bibliografici (_container_).


#### Aggiungere voci bibliografiche semplici (_work_)

Per aggiungere un _work_ semplice compilare i campi come segue: 

* _container_: **non spuntare** la casella;
* _typeId_: selezionare la tipologia tra _article_; _book_; _journal_; _proceedings_; 
* _key_: per la compilazione vedi il [paragrafo dedicato](bibliodb.md#key). 
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/b6f38e89e2d111d405164114fd26681777fd4b03/docs/assets/images/bibl5.png?raw=true)   
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: **non compilare**;
    * roleId: nel caso di un autore, non selezionare alcuna opzione; in tutti gli altri casi, scegliere tra: _curatore_, _traduttore_, _collaboratore_, _direttore_, _organizzatore_, _con_;
   Dopo aver compilato i campi cliccare _accept authors_.
* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;
* _year2_: se l'anno di edizione corrisponde a un intervallo. Inserire qui l'estremo più basso dell'intervallo.
* _publisher_: editore;
* _container_: contenitore, nel caso di articoli su rivista o in volumi miscellanei. Il contenitore può essere cercato digitando le prime lettere del titolo; deve essere già presente nel database nell'elenco dei _container_; in caso contrario, andrà creato prima della compilazione della _entry_ 
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/4cdc916490f77390f06ed821a68f27d7dd39b224/docs/assets/images/bibl6.png?raw=true)   
* _from-to_: pagine, nel caso di articoli su rivista o in volumi miscellanei;
* _number_: numero della rivista o della collana, se pertinente;
* _note_: note di vario tipo, ove necessarie;
* _location_: per indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: per indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca;  

⚠️ Una volta compilati i campi salvare la _entry_ cliccando sul tasto di spunta blu.

#### Aggiungere un contenitore bibliografico (_container_)

Per aggiungere un _container_ compilare i campi come segue:  
* _container_: **spuntare** la casella;
> ![](https://github.com/petrarchsitinera/linee-guida/blob/38a8a79aa3f74a4443f314f9d08e2dcd996032c7/docs/assets/images/bibl4.png?raw=true)  
* _typeId_: selezionare la tipologia tra _article_; _book_; _journal_; _proceedings_; 
* _key_: per la compilazione vedi il [paragrafo dedicato](bibliodb.md#key).   
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/b6f38e89e2d111d405164114fd26681777fd4b03/docs/assets/images/bibl5.png?raw=true)   
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: **non compilare**;
    * roleId: nel caso di un autore, non selezionare alcuna opzione; in tutti gli altri casi, scegliere tra: _curatore_, _traduttore_, _collaboratore_, _direttore_, _organizzatore_, _con_;
   Dopo aver compilato i campi cliccare _accept authors_. 
* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;  
* _year2_: se l'anno di edizione corrisponde a un intervallo. Inserire qui l'estremo più basso dell'intervallo.
* _publisher_: editore;
* _number_: numero, nel caso di collane;
* _note_: note di vario tipo, ove necessarie;
* _location_: per indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: per indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca.

⚠️ Una volta compilati i campi salvare la _entry_ cliccando sul tasto di spunta blu.

## Key

La chiave (_key_) è una chiave identificativa della voce bibliografica. Permette il collegamento tra la voce del database bibliografico e il database ITINERA, dove essa è richiamata al bisogno attraverso la compilazione di [DocReferences](Docref_Brick.md).

La (_key_) è creata automaticamente a partire dal cognome dell'autore o degli autori e dalla data della pubblicazione. Per pubblicazioni di uno stesso autore uscite nello stesso anno, la chiave è disambiguata automaticamente attraverso l'apposizione di una lettera.

In linea generale non si deve **mai** modificare la _key_ di una voce bibliografica già inserita e in uso, perché si comprometterebbe il collegamento tra quella voce e gli _item_ di Itinera che la richiamano.

Se dovesse rendersi necessario modificare una voce bibliografica in uso (p. es. in caso di errore), occorre tenere presente che la modifica di uno o più autori e/o dell’anno di pubblicazione comporta **automaticamente** la modifica della _key_. Per salvaguardare i collegamenti precedentemente istituiti tra la voce e gli _item_, si **deve perciò procedere manualmente** cliccando la casella _user key_ e ripristinando la _key_ precedente.

## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'_item_.

***

## Norme redazionali per l'inserimento di voci bibliografiche

Nel caso di articoli in rivista, atti di convegno e simili, **fare attenzione** a creare **prima** il _container_ (se non presente nel database bibliografico), quindi la voce bibliografica (_work).

Per indicare il numero di una rivista o di una collana, si usano **sempre** i numeri arabi, indipendentemente dalla prassi adottata dalla rivista.

### Casi particolari

* Nel caso di edizioni di testi di un autore, l'autore del testo va **sempre** inserito come primo autore, seguito dal curatore o dai curatori

> Esempio.   
> Nella voce bibliografica "Francesco Petrarca, _Canzoniere_, a cura di M. Santagata, Milano, Mondadori, 1996", si inserirà prima "Francesco Petrarca", quindi "Marco Santagata" (con ruolo = curatore).  

> <img width="1423" alt="Schermata 2023-04-06 alle 16 59 23" src="https://user-images.githubusercontent.com/102725489/230419042-18301315-0b91-4315-8d1a-0d0eafb75850.png">

* Nel caso di pubblicazioni per le quali i ruoli a disposizione (curatore, traduttore, collaboratore, direttore, organizzatore_) non fossero sufficienti, ricorrere **sempre** alla voce _con_

> Esempio.   
> Nella voce bibliografica "Arnaldo Foresti, _Aneddoti della vita di Francesco Petrarca_, a cura di Antonietta Tissoni Benvenuti, con una premessa di Giuseppe Billanovich, Padova, Antenore, 1977", "Arnaldo Foresti" sarà inserito come autore; Antonietta Tissoni Benvenuti con ruolo "curatore"; Giuseppe Billanovich con ruolo "con".

* Nel caso di opere collettive in più volumi o tomi con titolo particolare di ciascuno, si creano tanti _container_ quanti sono i volumi o i tomi. In questo caso si inserisce come titolo del _container_ il titolo dell'opera collettiva seguito 1. dal numero del volume o del tomo e 2. dal titolo specifico, ove presente. 

> Esempio.    
> Nel caso del volume 10 della _Storia della letteratura italiana_ diretta da Enrico Malato, andrà inserito come titolo: _Storia della letteratura italiana. Vol. 10. La tradizione dei testi_.

* Nel caso di articoli usciti più volte (p. es. prima in rivista e poi in libro), è preferibile registrare la pubblicazione più recente, ricorrendo ad essa anche per la compilazione degli _item_, avendo cura di registrare in nota la sede di prima pubblicazione secondo le norme descritte sopra.  
Nel richiamare voci bibliografiche di questo tipo durante la compilazione degli _item_, occorre però **prestare la massima attenzione** per non inserire numeri di pagina che facciano riferimento a versioni diverse della stessa pubblicazione. Nel caso in cui il compilatore abbia a disposizione una versione  diversa di una pubblicazione presente nel database bibliografico e fosse impossibilitato a consultare quest'ultima, procederà a registare la verrsione che ha a disposizione.  

