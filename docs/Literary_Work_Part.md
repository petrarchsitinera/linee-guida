# Literary Work Info Part

**Literary Work Info Part** raccoglie le informazioni generali sui testi.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#literaryworkinfopart).
 
La parte si articola in tre sezioni, navigabili attraverso il menu orizzontale in alto:
* generale [general]
* lingua e genere [lang./note]
* metrica [poetry], riservata ai testi poetici.

Per aggiungere la parte, selezionare **_info_** dal menu a tendina, quindi cliccare su **_add part_**.  


## Generale [General]

### Authors
Permette di indicare l'autore del testo, secondo il modello [Asserted Id](Asserted_Ids_Brick.md).  
Per individuare [l'_eid_](identifiers.md) di un autore schedato in Itinera, consultare il [repository delle persone](repository.md) o ricorrere alla funzione di [lookup](lookup.md).   
Nel caso in cui alla persona da inserire non sia attribuito un _eid_, il compilatore procede ad assegnarne uno seguendo le istruzioni indicate [qui](identifiers.md). 

⚠️ L'_eid_ deve essere copiate nel campo _value_.   

> Tutti gli autori dispongono, di norma, di un Item Person dedicato. In caso contrario, e dopo aver verificato sui [repository](repository.md) è opportuno creare un Item Person dedicato e richiamarne l'_eid_ nel campo _author_.   
> Se l'autore non è di interesse specifico di Itinera, è possibile evitare la creazione di un Item Person dedicato e inserire un identificativo convenzionale secondo le regole definite per gli [_eid_](identifiers.md).  
> Anche autori non identificati storicamente dispongono, di norma, di un Item Person dedicato. Se sussistono ipotesi di identificazione, queste sono registrate nella [_External Ids Part_ di tali _items_](External_Ids_Part_Person.md#soggetti-non-identificati-storicamente). Di conseguenza, occorre compilare il campo _author_ con l'identificativo dell'Item Person dedicato all'autore non storicamente identificato cui è attribuito il testo e NON con l'identificativo dell'Item Person con cui l'ignoto è identificato.  

La sezione _assertion_ permette di precisare il grado di attendibilità dell'attribuzione, e di indicarne eventualmente le fonti.  

Il campo _author_ è replicabile: permette infatti di dare conto di casi di autorialità multipla o contesa.  
In questi casi creare più elementi _Asserted Id_, con i relativi _rank_ e fonti.

La compilazione del campo è obbligatoria.

### Title
Permette di indicare il titolo del testo.  
Il titolo del testo inserito deve coincidere con il nome dell'item, ovvero con quello riportato nel [**repository dei testi**](repository.md). Consultare le indicazioni riportate per il **title** dei testi in [Metadata](Item_Work_Metadata.md).

È possibile comunque indicare più titolazioni, se del caso, siano esse d'autore o meno. 

⚠️ Per le lettere di Petrarca è **sempre obbligatorio** creare un secondo elemento _title_ corrispondente all’incipit della lettera, oltre al titolo redazionale (coincidente con il nome dell'item, ovvero con quello riportato nel [**repository dei testi**](repository.md): es. Fam. I 1).  

I titoli sono inseriti attraverso un [editor](Editor_Brick.md). Per ciascun titolo è possibile indicare:  
* la lingua in cui il titolo è espresso (obbligatorio);
* il titolo (obbligatorio);
* una [Assertion](Assertion_Brick.md) per precisare il grado di attendibilità e le fonti del titolo.

Per salvare i dati inseriti *per ogni titolo*, cliccare il tasto di spunta blu. I dati inseriti saranno così visualizzati nella parte superiore in una tabella di riepilogo.

La compilazione del campo è obbligatoria.  

### Is Lost
Spuntare **is Lost** quando il testo schedato è un testo perduto.

### Note
Il campo note permette di inserire una breve stringa di testo esplicativo. Compilare il campo solo se strettamente necessario.   
⚠️ Ogni frase deve essere chiusa da punto fermo.  

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
Inserire l'intero schema rimico senza spazi.  
> es. ABBAABBACDECDE  

## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
