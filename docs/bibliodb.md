# Database bibliografico 

Il database bibliografico raccoglie tutta la bibliografia impiegata nella descrizione degli _item_ ed è accessibile:

* da [_Bibliography_](https://itinera.unisi.it/#/biblio) nel menu orizzontale nella parte alta della schermata, come nell'immagine:

<img width="624" alt="Schermata 2023-04-04 alle 15 50 33" src="https://user-images.githubusercontent.com/102725489/229814240-b6ed1a8d-4f43-4d05-b3ab-0cc0e6846132.png">


* dalla [_Bibliography Part_](External_Bibliography_Part.md) di un singolo _item_.

## Voci bibliografiche

Ogni voce bibliografica inserita costituisce una singola _entry_. Le _entries_ si distinguono in:
- _works_: singole voci bibliografiche;
- _containers_: voci bibliografiche che ne contengono altre (ad es. periodici, atti di convegno, cataloghi, ecc.). 

## Bibliografia

La schermata iniziale del database bibliografico mostra la lista delle _entries_ già inserite.

<img width="1438" alt="Schermata 2023-04-06 alle 12 37 26" src="https://user-images.githubusercontent.com/102725489/230355344-ab20ad59-3087-44b6-976f-07e38effd044.png">

Da questa schermata è possibile visualizzare, modificare ed eliminare le _entries_.

⚠️⚠️⚠️ **ATTENZIONE**: Modificare o eliminare una _entry_ nel database bibliografico ha ricadute su **tutti gli _item_** che fanno riferimento alla relativa voce bibliografica. 

Usando i pulsanti a sinistra di ogni voce, è possibile visualizzare, modificare o eliminare le _entries_ relative.

<img width="799" alt="Schermata 2023-04-06 alle 12 54 22" src="https://user-images.githubusercontent.com/102725489/230357314-a9ef4bb7-7bce-4954-81e0-87ebc8f90a37.png">

Selezionando il pulsante _view_ di una _entry_, è possibile visualizzare nella parte bassa della schermata la voce bibliografica per esteso.

<img width="1158" alt="Schermata 2023-04-06 alle 12 58 52" src="https://user-images.githubusercontent.com/102725489/230358611-a7ca6324-ed62-46f7-9c32-389d908ac5de.png">

Selezionando il pulsante _edit_ di una _entry_, è possibile modificare la voce bibliografica intervenendo nei campi della finestra che si apre nella parte bassa della schermata (vedi più oltre).

<img width="1440" alt="Schermata 2023-04-06 alle 13 03 57" src="https://user-images.githubusercontent.com/102725489/230359620-b3e4b87c-63c8-4124-8d51-23def0434a4c.png">

⚠️⚠️⚠️ **ATTENZIONE**: Non modificare **mai** la _key_ di una voce già inserita (vedi più oltre).

Selezionando il pulsante _delete_ di una _entry_, è possibile eliminare la voce bibliografica relativa. Un pop-up chiede conferma dell'azione.

⚠️⚠️⚠️ **ATTENZIONE**: Eliminare una _entry_ nel database bibliografico ha ricadute su **tutti gli _item_** che fanno riferimento alla relativa voce bibliografica. 

##FILTRI
 Per visualizzare soltanto la lista dei _containers_, spuntare la casella relativa.  

<img width="1438" alt="Schermata 2023-04-06 alle 12 37 26" src="https://user-images.githubusercontent.com/102725489/230356154-14186fd2-c218-4ca0-af00-db0c44dd7f10.png">

### Creare una voce bibliografica semplice (_work_)
Per creare un nuovo _work_ cliccare il comando _+ new_.  
> ![](https://github.com/petrarchsitinera/linee-guida/blob/38a8a79aa3f74a4443f314f9d08e2dcd996032c7/docs/assets/images/bibl2a.png?raw=true)  

⚠️ Per le norme citazionali seguire le istruzioni [in fondo alla pagina](External_Bibliography_Part.md#norme-citazionali).  

Ogni _work_ è strutturato nei seguenti campi:  
* _container_: non spuntare la casella;
* _typeId_: permette di specificare la tipologia di voce bibliografica selezionando tra: article; book; journal; proceedings;  
* _key_: chiave identificativa della voce biliografica, che può essere utilizzata per richiamare sinteticamente la voce in [DocReference](Docref_Brick.md);
  * la chiave è, di norma, creata automaticamente a partire dal cognome dell'autore o degli autori e dalla data della pubblicazione; in caso di identità (ad es. per   pubblicazioni dello stesso autore uscite nello stesso anno) la chiave è disambiguata automaticamente attraverso l'apposizione di un lettera);  
  * se si desidera attribuire una chiave diversa da quella generata automaticamente (ad es. per opere senza anno o senza autore), spuntare la casella _user key_.  
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/b6f38e89e2d111d405164114fd26681777fd4b03/docs/assets/images/bibl5.png?raw=true)   
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: non compilare;
    * roleId: selezionare, se pertinente, tra: curatore, traduttore, collaboratore, direttore, organizzatore;
   Dopo aver compilato i campi cliccare _accept authors_.

* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;
* _year2_: se l'anno di edizione corrisponde a un intervallo (in questo caso attribuire una _key_ bibliografica arbitraria, poiché quella automatica indica solo il valore inserito in _year_);   
* _publisher_: editore;
* _container_: permette di indicare il contenitore, nel caso di articoli su rivista o in volumi miscellanei. Il contenitore può essere cercato digitando le prime lettere del titolo; deve essere già presente nel database nell'elenco dei _container_; in caso contrario, andrà creato prima della compilazione della _entry_ 
  > ![](https://github.com/petrarchsitinera/linee-guida/blob/4cdc916490f77390f06ed821a68f27d7dd39b224/docs/assets/images/bibl6.png?raw=true)   
* _from-to_: permette di inserire le pagine, nel caso di articoli su rivista o in volumi miscellanei;
* _number_: permette di inserire il numero, nel caso di articoli su rivista o di collane;
* _note_: permette di aggiungere note di vario tipo;
* _location_: permette di indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: permette di indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca.  


Una volta compilati i campi salvare la _entry_ cliccando sul tasto di spunta blu.

### Creare un contenitore bibliografico (_container_)
Per creare un nuovo _container_ cliccare il comando _+ new_.  
> ![](https://github.com/petrarchsitinera/linee-guida/blob/38a8a79aa3f74a4443f314f9d08e2dcd996032c7/docs/assets/images/bibl2a.png?raw=true)  

⚠️ Per le norme citazionali seguire le istruzioni [in fondo alla pagina](External_Bibliography_Part.md#norme-citazionali).  

Ogni _container_ è strutturato nei seguenti campi: 
* _container_: spuntare la casella;
> ![](https://github.com/petrarchsitinera/linee-guida/blob/38a8a79aa3f74a4443f314f9d08e2dcd996032c7/docs/assets/images/bibl4.png?raw=true)  

* _typeId_: permette di specificare la tipologia di voce bibliografica selezionando tra: article; book; journal; proceedings;  
* _key_: chiave identificativa della voce biliografica, che può essere utilizzata per richiamare sinteticamente la voce in [DocReference](Docref_Brick.md);
  * la chiave è, di norma, creata automaticamente a partire dal cognome dell'autore o degli autori e dalla data della pubblicazione; in caso di identità (ad es. per   pubblicazioni dello stesso autore uscite nello stesso anno) la chiave è disambiguata automaticamente attraverso l'apposizione di un lettera);  
  * se si desidera attribuire una chiave diversa da quella generata automaticamente (ad es. per opere senza anno o senza autore), spuntare la casella _user key_.  
* _authors_: permette di indicare l'autore o gli autori della voce bibliografica. Cliccando il campo si apre una finestra dalla quale è possibile:
  * cercare il nome di un autore già presente nel database bibliografico: inserendo le prime lettere del nome o del cognome dell'autore nel campo _last name_ sono mostrati suggerimenti; selezionare l'autore prescelto e cliccare _accept authors_;
 > ![](https://github.com/petrarchsitinera/linee-guida/blob/b6f38e89e2d111d405164114fd26681777fd4b03/docs/assets/images/bibl5.png?raw=true)   
  * inserire il nome di un autore: cliccare _add new author_ e compilare i seguenti campi:
    * firstName: nome;
    * lastName: cognome;
    * suffix: non compilare;
    * roleId: selezionare, se pertinente, tra: curatore, traduttore, collaboratore, direttore, organizzatore;
   Dopo aver compilato i campi cliccare _accept authors_.  
* _title_: titolo dell'opera;
* _language_: lingua dell'opera, selezionando un valore nel menu a tendina;
* _place_: luogo di edizione;
* _year_: anno di edizione;  
* _year2_: se l'anno di edizione corrisponde a un intervallo (in questo caso attribuire una _key_ bibliografica arbitraria, poiché quella automatica indica solo il valore inserito in _year_);   
* _publisher_: editore;
* _number_: permette di inserire il numero, nel caso di collane;
* _note_: permette di aggiungere note di vario tipo;
* _location_: permette di indicare, nel caso di risorse online, l'indirizzo web;
* _access date_: permette di indicare, nel caso di risorse online, la data di consultazione;
* _keywords_: per aggiungere _tag_ utili ai fine della ricerca.

Una volta compilati i campi salvare il _container_ cliccando sul tasto di spunta blu.

## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'_item_.

***

## Norme citazionali

