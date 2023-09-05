# Thesaurus eventi Work 
Di seguito sono elencate le tipologie di evento (_type_) relativi ai testi e le tipologie di entità collegate (_related entities_).  


#### Invio 
Permette di registrare l'invio del testo.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'invio.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_;
* _allegato_.

Nel caso di più mittenti, destinatari, latori o allegati afferenti ad un medesimo invio (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  

⚠️ Nel caso in cui l'invio inserito sia seguito da una ricezione accertata, occcorre inserire e descrivere ciascun evento singolarmente, assegnando ad ognuno di essi da un EID univoco. L'invio e la ricezione risulteranno collegati attraverso l'inserimento di un medesimo _tag_. Vedi [qui](Events_Part.md#-tag) per la compilazione del _tag_. 

#### Ricezione  
Permette di registrare la ricezione del testo da parte di una persona.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della ricezione.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_;  
* _allegato_.

Nel caso di più mittenti, destinatari, latori o allegati afferenti ad un medesima ricezione (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  

⚠️ Nel caso in cui l'invio inserito sia seguito da una ricezione accertata, occcorre inserire e descrivere ciascun evento singolarmente, assegnando ad ognuno di essi da un EID univoco. L'invio e la ricezione risulteranno collegati attraverso l'inserimento di un medesimo _tag_. Vedi [qui](Events_Part.md#-tag) per la compilazione del _tag_.   

#### Scambio diretto  
Permette di inserire lo scambio diretto di un testo tra due persone.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dello scambio.   

È possibile indicare come entità _related_:  
* _consegna_: la persona che cede l'oggetto scambiato;  
* _destinatario_: la persona che riceve l'oggetto scambiato. 
* _allegato_: eventuali altri oggetti scambiati.

⚠️ Nel caso di scambi reciproci, cioè quando in un'unica occasione sono scambiati più oggetti da parte dei partecipanti allo scambio, occorre creare più eventi _scambio diretto_ all'interno della _Events Part_ della persona da cui muove lo scambio o all'interno della _Events Part_ degli oggetti scambiati (specificando i ruoli dei partecipanti). In questi casi occorrerà compilare il campo _tag_ di ogni evento con un identificativo unico, così da permettere di ricondurre tutti gli scambi alla medesima occasione.

> es. 

#### Trascrizione
Permette di registrare una trascrizione del testo.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della trascrizione.   

È possibile indicare come entità _related_:  
* la _copia_: il manoscritto che conserva la trascrizione, ove noto;
* il _trascrittore_: l'esecutore della copia, ove noto;

⚠️ Nel caso in cui la trascrizione proceda da una ricezione accertata, occcorre inserire e descrivere ciascun evento singolarmente, assegnando ad ognuno di essi da un EID univoco. La trascrizione e la ricezione (insieme eventulmente all'invio collegato a quest'ultima) risulteranno collegati attraverso l'inserimento di un medesimo _tag_. Vedi [qui](Events_Part.md#-tag) per la compilazione del _tag_. 

#### Raccolta
Permette di fornire informazioni sull'ingresso di un testo in una raccolta.   
La compilazione è limitata a casi in cui sia nota, più o meno certamente, la data dell'ingresso del testo in una raccolta e/o dell'uscita, o a casi di particolare interesse o complessità (come, per esempio, di lettere transitate da una raccolta all'altra, o di testi inizialmente inclusi e poi rifiutati nelle stesse).  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento va compilato **solo** nel caso in cui sia nota, più o meno certamente, la data dell'ingresso del testo in una raccolta e/o dell'uscita.  

È obbligatorio indicare come entità _related_:  
* _raccolta_: la raccolta d'autore in cui è inserito il testo.  

#### Redazione
Permette di indicare quando il testo è la redazione precedente di un altro testo (ad es. _Sen_. XIII 11 gamma è redazione precedente di _Sen_. XIII 11).  

La compilazione della _description_ è riservata a casi di particolare interesse o complessità, come per esempio lettere notevolmente rimaneggiate e/o smembrate a formare nuovi testi.  In tutti gli altri casi, la _description_ non va compilata.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della stesura del testo.

È obbligatorio indicare tra le entità _related_:  
* _precedente di_: la redazione successiva del testo schedato.

Si inserisce tra i _related_ soltanto la redazione immediatamente successiva. Per esempio, nel caso di una lettera di cui siano attestate una redazione gamma, una redazione beta e una redazione alfa, l'_item_ relativo alla redazione gamma riporterà tra i _related_ **soltanto** la redazione beta; l'_item_ relativo alla redazione beta riporterà tra i _related_ **soltanto** la redazione alfa.  
Si aggiungono più _related_ **soltanto** nel caso in cui una redazione originaria abbia dato luogo, a seguito di smembramento, a due testi diversi.  
