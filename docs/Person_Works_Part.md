# Person Works Part

**Person Work Part** permette di inserire le opere di un autore, siano esse letterie o non letterarie, autentiche, dubbie o attribuite.   

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#personworkspart).

Per aggiungere la parte, selezionare **works** dal menu a tendina, quindi cliccare su **add part**.  

##  Work
Per ogni opera è creato un elemento _work_ mediante un [editor](Editor_Brick.md).

###  Title
Inserire il titolo completo dell'opera **nella forma d'autore**. In caso di dubbio si preferisce il **titolo usato più frequentemente** nelle edizioni moderne.
> [Francesco Petrarca] _Rerum vulgarium fragmenta_ 📷 se no uno pensa di dover mettere anche nome d'autore e corsivo 📷   
> [Francesco Petrarca] _Res Seniles_   
> [Giovanni Boccaccio] _Decamerone_      

Nel caso di **raccolte d'autore**, si inserisce soltanto il **titolo della raccolta**, **mai** il titolo dei singoli testi.  
> Nell'item Francesco Petrarca non si inserisce mai _Rvf 1_, ma soltanto _Rerum vulgarium fragmenta_.  
> Allo stesso modo, si inserisce _Res Seniles_ e mai _Sen. V 1_.      

Nel caso di **testi poetici** sciolti e senza titolo, inserire il **primo verso**.  
> [Giacomo Colonna] _Se le parti del corpo mio destrutte_       

Nel caso di **lettere** non raccolte, inserire **l'intestazione** o, in sua assenza, **le prime parole del testo**.   
> [Barbato da Sulmona] _Frater carissime_  
> [Francesco Nelli] _Amor et dolor impellunt_      

🚧 NICOLA DOMANDA PER NOI: COME CI COMPORTIAMO RISPETTO A LETTERE E RIME DISPERSE? LE INSERIAMO UNA PER UNA OPPURE COME CORPUS NON D'AUTORE? E PER I CASI COME BOCCACCIO, AUTORE DI LETTERE E RIME NON RACCOLTE MA PUBBLICATE IN EDIZIONI DI CUI E' INVALSA LA NUMERAZIONE? 

La compilazione del campo è obbligatoria.  

### Eid
L'_eid_ è l'identificativo dell'opera quando questa si trovi descritta all'interno della banca dati Itinera.  
L'_eid_ permette di collegare il testo inserito nella **Person Work Part** con l'item autonomo eventualmente già esistente che descrive quel testo.


DOBBIAMO DECIDERE SE INSERIRE SOLO OPERE EXTRA-DB o ANCHE OPERE IN DB.

🚧 NICOLA DOMANDA PER NOI: SE INVECE IL TESTO O L'OPERA NON E' DESCRITTO IN ITINERA NON COMPILIAMO L'EID? O NE METTIAMO COMUNQUE UNO D'UFFICIO? IN QUESTO SECONDO CASO FORSE POTREMMO PENSARE AD UN REPOSITORY DI TITOLI, PER TENERE TRACCIA DI TUTTI 'GLI OGGETTI' INSERITI, COSI' DA POTERLI COLLEGARE ANCHE IN FUTURO QUALORA I CORPORA DESCRITTI DOVESSERO ALLARGARSI.

🚧 NB. Rivedere questione possibili doppioni risolti con indicizzazione automatica. Altrimenti ricorrere alla soluzione del repository e della creazione preventiva di tutti gli item text.
🚧 Rivedere legame con AUTHOR 🚧


###  Assertion  
Se il testo o l'opera da inserire è **dubbia** o **attribuita**, spuntare e compilare l'[assertion](Assertion_Brick).

L'_assertion_ si riferisce sempre ad una singola attribuzione: descrive cioè l'attribuzione di un singolo testo dubbio o presunto ad un autore.  
Nel caso di più testi dubbi o attribuiti, l'_assertion_ va ripetuta: si inseriscono tante _assertion_ quanti sono i testi dubbi o attribuiti.  

Il campo _note_ dell'_assertion_ può essere compilato quando il rimando alle voci bibliografiche e alle fonti non sia sufficiente o nei casi che, risultando complessi, richiedano un supplemento di spiegazione.

## Save ⚠️ 

Per ogni elemento _work_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
