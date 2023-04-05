# Related Persons Part

**Related Persons Part** permette di elencare le persone collegate al testo a vario titolo (citato, pseudonimo, destinatario, dedicatario, richiesta di recapito).  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#relatedpersonspart).  

Per aggiungere la parte, selezionare **_rel-persons_** dal menu a tendina, quindi cliccare su **_add part_**. 

## Person
Per ogni persona collegata si crea un elemento _person_ mediante [editor](Editor_Brick.md).  

⚠️ In presenza di più citazioni riferite ad un sola persona, si crea un unico elemento _person_, compilando il campo _name_ con la forma più esplicita, possibilmente il nome, normalizzata al **nominativo** se presente a testo in altri casi.  

⚠️ Se una persona è citata sia attraverso uno pseudonimo sia con il nome proprio, registrare un'unica _person_ sotto _pseudonimo_. Sono da includere nei citati anche eventuali latori menzionati a testo, sia che si tratti di latori del testo schedato sia che si tratti di latori di altri testi.   

⚠️ Nel caso in cui a testo sia presente un nome collettivo, aggiungere tanti elementi _person_ quante sono le persone a cui ci si riferisce.  

> Esempio. La lettera _Multa expectaram_ di Francesco Nelli a Francesco Petrarca fa riferimento ad un "coetus tuus", ovvero al cosiddetto cenacolo fiorentino di amici e ammiratori di Petrarca, composto, oltre che da Nelli stesso, da Giovanni Boccaccio, Lapo da Castiglionchio e Francesco Bruni. In questo caso, andrebbero aggiunti tre elementi _person_ (ognuno con _name_ "coetus tuus"), ma poiché Francesco Bruni è citato a testo in forma esplicita, per quest'ultimo si preferisce il nominativo.  

<img width="362" alt="Schermata 2023-04-05 alle 11 29 15" src="https://user-images.githubusercontent.com/102725489/230040977-9494fe4f-cafe-42d1-87de-9b56199ff2d8.png">


⚠️ Nel caso in cui il testo schedato dia notizia di un invio o di una ricezione, occorre creare un evento apposito nella [EventsPart](Events_Part.md) del **testo inviato o ricevuto**, dove è possibile esplicitare i ruoli di mittente, destinatario e latore, a seconda dei casi.  



### Type
Permette di specificare il tipo di relazione che la persona da inserire intrattiene con il testo schedato:  
* citato: quando la persona è citata nel testo;
* pseudonimo: quando la persona è citata nel testo mediante uno pseudonimo;
* destinatario: quando la persona è il destinatario diretto ed esplicito del testo;
* dedicatario: quando la persona è il dedicatario primario ed esplicito del testo;
* richiesta di recapito a: quando la persona è indicata nel testo come ulteriore destinatario cui recapitare il testo.  

La compilazione del campo è **obbligatoria** in presenza dei dati relativi.  

### Name
Il nome della persona nella forma presente a testo.  
In presenza di più citazioni riferite ad un sola persona, si privilegia la forma più esplicita, possibilmente il nome, normalizzata al nominativo.  

La compilazione del campo è **obbligatoria**.

### Ids 
Permette di collegare il nome inserito ad una o più persone storicamente individuate, secondo il modello [Asserted Id](Asserted_Ids_Brick.md).   
Se la persona è schedata come Item Person in Itinera, cercare l'item relativo e copiarne [l'_eid_](identifiers.md), servendosi eventualmente dei [repository](repository.md) e della funzione di [lookup](lookup.md). 
⚠️ L'_eid_ deve essere copiate nel campo _value_.   
Per gli altri casi consultare le indicazioni per la compilazione degli [identificativi](identifiers.md).  


## Save ⚠️ 

Per ogni elemento _person_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
