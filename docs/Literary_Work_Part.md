# Literary Work Info Part

**Literary Work Info Part** raccoglie le informazioni generali sui testi.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#literaryworkinfopart).
 
La parte si articola in tre sezioni, visibili e navigabili attraverso il menu orizzontale in alto:
* generale [general]
* lingua e genere [lang./note]
* metrica [poetry], riservata ai testi poetici.

Per aggiungere la parte, selezionare **_info_** dal menu a tendina, quindi cliccare su **_add part_**.  


## Generale [General]

### 🚧 Author 🚧 ora su modello AssertedId

Permette di indicare l'autore del testo. 
🚧 NON PIU COSì 🚧 Questo campo deve essere utilizzato *soltanto nei casi in cui la paternità del testo risulti certa*. Questi casi comprendono anche quelli in cui l'autore del testo non sia identificato storicamente.    
    
🚧 NON PIU COSì 🚧 Se uno di questi autori è un nome di piuma, avrà un suo item dove si compila la PersonWorksPart; se per questo autore esistono proposte di identificazione, l'Item Person dell'autore di cui si propone l'identificazione con il nome di piuma  è collegato all'Item di quest'ultimo attraverso una tripla (o attraverso un External Id con scope=Itinera, che funzioni come un predicato "è identificabile con", con relativo rank. Nell’item dedicato al personaggio ipoteticamente identificato con il nome di piuma la PersonWorksPart non è compilata con il testo attribuito al nome di piuma. 
[AGGIUNGERE ESEMPIO NICOLA PARIGI] 

🚧 NON PIU COSì 🚧 Nei casi di autorialità dubbia o contesa, il compilatore dovrà aprire la [[Person Works Part|Person_Works_Part]] dell'autore o degli autori cui il testo è dubitosamente attribuito e inserire l'id dell'opera con un rank uguale o superiore a 2.   
 
[AGGIUNGERE ESEMPIO NICOLA PARIGI]    

PER NOMI DI PIUMA FARE RIFERIMENTO A EXTERNAL IDS PART

La compilazione del campo è 🚧 obbligatoria.

### Title
Permette di indicare il titolo del testo.  
Il titolo del testo inserito deve coincidere con il nome dell'item, ovvero con quello riportato nel **repository dei corpora**. Consultare le indicazioni riportate per il **title** dei testi in [Metadata](Item_Work_Metadata.md).

È possibile comunque indicare più titolazioni, quando ne esistessero più di una, d'autore o meno. 

⚠️ Per le lettere di Petrarca, oltre al titolo redazionale (coincidente con il nome dell'item, ovvero con quello riportato nel **repository dei corpora**: es. Fam. I 1), creare un secondo elemento _title_ corrispondente all’incipit della lettera.  

I titoli sono inseriti attraverso un [[visual editor|Editor_Brick]]. Per ciascun titolo è possibile indicare:  
* la lingua in cui il titolo è espresso (obbligatorio);
* il titolo (obbligatorio);
* una [[Assertion|Assertion_Brick]] (facoltativa) per precisare il grado di attendibilità e le fonti del titolo.

Per salvare i dati inseriti *per ogni titolo*, cliccare il tasto di spunta blu. I dati inseriti saranno così visualizzati nella parte superiore in una tabella di riepilogo.

La compilazione del campo è obbligatoria.  

### Is Lost
Spuntare **is Lost** quando il testo schedato è un testo perduto.

### Note
Il campo note permette di inserire una breve stringa di testo esplicativo. Compilare il campo solo se strettamente necessario. 


## Lingua e genere [lang./note]

### Language 
Permette di indicare, attraverso selezione multipla, la lingua o le lingue in cui il testo è stato scritto.  

La compilazione del campo è obbligatoria.

### Genre. 

Permette di indicare il genere letterario del testo attraverso un thesaurus gerarchico, suddiviso in:
* prosa
* poesia
* prosimetro

Le voci _prosa_ e _poesia_ comprendono al loro interno vari sottogeneri, tra i quali è possibile selezionare quello specifico cui appartiene il testo schedato.  

È possibile cercare il sottogenere:
* aprendo direttamente il menu a tendina desiderato (genre > poesia / prosa / prosimetro > [...]);
* ricorrendo al campo di ricerca _find_.

La voce selezionata apparirà in grassetto in testa al box, accanto alla parola _genre_, come nell'immagine:
<img width="578" alt="Schermata 2022-09-23 alle 16 33 15" src="https://user-images.githubusercontent.com/102725489/191985449-e651db61-1dd3-415d-b858-877debad1106.png">

La compilazione del campo è obbligatoria.

## Metrica [Poetry]

La compilazione di questo sottoparte è facoltativa ed è riservata ai testi poetici.

### Metre
Permette di indicare, attraverso selezione multipla, il metro o i metri utilizzati nel testo.

### Strophe
Permette di inserire lo schema rimico del testo, secondo la prassi tradizionale (per quanto riguarda i testi italiani lettere capitali per endecasillabi, minuscole per settenari).

## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
