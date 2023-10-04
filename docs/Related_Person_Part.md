# Related Persons Part

**Related Persons Part** permette di inserire le persone collegate al testo a vario titolo (citato, pseudonimo, destinatario, dedicatario, richiesta di recapito).  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#relatedpersonspart).  

Per aggiungere la parte, selezionare **_rel-persons_** dal menu a tendina, quindi cliccare su **_add part_**. 

## Person
Per ogni persona collegata si crea un elemento _person_ mediante [editor](Editor_Brick.md).  

⚠️ Il destinatario del testo va inserito **solo** come _destinatario_ (_type_=_destinatario_) anche quando si trovi citato in altri luoghi del testo. **Non** va dunque inserito anche come _citato_ (_type_=_citato_).  

⚠️ In presenza di più citazioni riferite ad un sola persona, si crea un unico elemento _person_, compilando il campo _name_ con la forma più esplicita, possibilmente il nome, normalizzata al **nominativo** se presente a testo in altri casi.  

⚠️ Il destinatario del testo che sia citato, nella rubrica o a testo, anche attraverso pseudonimo va inserito **sia** come _destinatario_ (_type_=_destinatario_) **sia** come pseudonimo (_type_=_pseudonimo_). In questi casi esisteranno dunque un elemento _person_ che indica la persona come destinatario e un elemento _person_ che lo indica come _pseudonimo_. Nel caso in cui il destinatario risulti ulteriormente citato a testo **non** si procede alla creazione di un ulteriore elemento _person_ con _type_=_citato_, come già indicato.

⚠️ Se una persona è citata sia attraverso uno pseudonimo sia con il nome proprio, registrare un'unica _person_ sotto _pseudonimo_. Sono da includere nei citati anche eventuali latori menzionati a testo, sia che si tratti di latori del testo schedato sia che si tratti di latori di altri testi.   

⚠️ Nel caso in cui a testo sia presente un nome collettivo, aggiungere tanti elementi _person_ quante sono le persone a cui ci si riferisce.  

> Esempio. La lettera _Multa expectaram_ di Francesco Nelli a Francesco Petrarca fa riferimento ad un "coetus tuus", ovvero al cosiddetto cenacolo fiorentino di amici e ammiratori di Petrarca, composto, oltre che da Nelli stesso, da Giovanni Boccaccio, Lapo da Castiglionchio e Francesco Bruni. In questo caso, andrebbero aggiunti tre elementi _person_ (ognuno con _name_ "coetus tuus"), ma poiché Francesco Bruni e Giovanni Boccaccio sono citati a testo in forma esplicita, per questi ultimi si preferisce il nominativo.  

<img width="743" alt="Screenshot 2023-10-03 alle 17 31 43" src="https://github.com/petrarchsitinera/linee-guida/assets/102725489/ba2fccd1-cfac-43ff-b19f-a4066df3e448">   



⚠️⚠️⚠️ Nel caso in cui il testo schedato **dia notizia di un invio o di una ricezione**, occorre creare un evento apposito nella [EventsPart](Events_Part.md) del **testo inviato o ricevuto**, dove è possibile esplicitare i ruoli di mittente, destinatario e latore, a seconda dei casi. 

⚠️⚠️⚠️ Nel caso in cui il testo schedato **dia notizia di un qualsiasi altro evento**, occorre creare un evento apposito nella [EventsPart](Events_Part.md) della **persona** o del **testo** implicato, indicando il testo come fonte d'infomazione.


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

In presenza di più citazioni riferite ad una medesima persona, si privilegia la forma più esplicita, possibilmente il nome, normalizzata al **nominativo** se presente a testo in altri casi.    

Nel caso di lettere di cui si debba indicare il destinatarioin in cui manchi l'intestazione, si inserisce il nome della persona nella forma indicata nel [repository dei nomi di persona](repository.md) **tra parentesi quadre**.

Nel caso di lettere perdute di cui si debba indicare il destinatario, essendo impossibile ricorrere alla forma del nome citato a testo, si inserisce il nome della persona nella forma indicata nel [repository dei nomi di persona](repository.md) **tra parentesi quadre**.

> Es. [Francesco Petrarca]

Nel caso in cui il testo schedato sia diretto o citi istituzioni o gruppi istituzionali, si adotta il nome italianizzato presente  nella rubrica del testo o a testo. Qualora fosse utile indicare uno o più membri di tali istituzioni o gruppi, è possibile inserirne gli identificativi nel campo _Ids_.

> Es. La _Related person part_ di Fam. XI 5 avrà un elemento _related person_ in cui il _name_ con _type=destinatario_ coinciderà con "Fiorentini". Poiché in questo caso non è utile indicare la lista dei fiorentini ai quali Petrarca scrive, non occorre compilare il campo _Ids_.

La compilazione del campo è **obbligatoria**.

### Ids 
Permette di collegare il nome inserito ad una o più persone storicamente individuate, secondo il modello [Asserted Id](Asserted_Ids_Brick.md).  
Per individuare [l'_eid_](identifiers.md) di una persona schedata in Itinera, controllare sempre il [repository delle persone](repository.md).  
Se la persona è schedata come Item Person all'interno della banca dati, essa è conseguentemente provvista di un [_eid_](identifiers.md). È possibile dunque cercare e richiamare l'_eid_ attraverso lo strumento di ricerca integrato in [Asserted Id](Asserted_Ids_Brick.md#target).  
Nel caso in cui alla persona da inserire non sia già attribuito un _eid_, il compilatore dovrà selezionare il [flag _external_](Asserted_Ids_Brick.md#altri-identificativi-itinera), procedere all'assegnazione di un nuovo _eid_ seguendo le istruzioni indicate [qui](identifiers.md) e segnalarla su [Clickup](https://clickup.com/) per permettere l'aggiornamento del [repository](repository.md).  
   
⚠️ Ogni _id_ inserito in un singolo elemento _person_ costituisce una proposta di identificazione del _name_ relativo.   

⚠️ Più _id_ all'interno di un singolo elemento _person_ sono proposte di identificazione alternative del _name_ inserito, ciascuna eventualmente corredata di indice di affidabilità e fonti, secondo il modello [Asserted Id](Asserted_Ids_Brick.md).    

La compilazione del campo è **obbligatoria** in presenza dei dati relativi.  

## Save ⚠️ 

Per ogni elemento _person_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
