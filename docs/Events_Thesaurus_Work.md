# Thesaurus eventi Work 
Di seguito sono elencate le tipologie di evento (_type_) relativi ai testi e le tipologie di entità collegate (_related entities_).  


#### Invio 
Permette di registrare l'invio del testo schedato da parte di una persona, anche diversa dall'autore.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'invio.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_;
* _allegato_.

Nel caso di più mittenti, destinatari, latori o allegati afferenti ad un medesimo invio (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

⚠️⚠️⚠️ Si inseriscono _allegati_ **soltanto** quando occorre registrare oggetti diversi da testi, per esempio manoscritti, monete, manufatti di qualsiasi tipo. Nel caso in cui siano inviati soltanto testi, questi ultimi vanno tutti inseriti come **_oggetto inviato_**. 

⚠️⚠️⚠️ **Quando i testi inviati siano più d'uno**, l'evento va **sempre inserito** a partire da un _item person_, dove è possibile aggiungere più _oggetti inviati_ - nella _Events Part_ di un _item work_ è possibile inserire soltanto l'invio del testo descritto dall'_item_, aggiungendovi eventuali allegati, ma non è possibile aggiungere più testi inviati contestualmente a quello.

⚠️⚠️⚠️ Nel caso in cui l'invio inserito sia seguito da una ricezione accertata, occcorre inserire e descrivere ciascun evento singolarmente, assegnando ad ognuno di essi da un EID univoco. L'invio e la ricezione risulteranno collegati attraverso l'inserimento di un medesimo _tag_. Vedi [qui](Events_Part.md#-tag) per la compilazione del _tag_. 

#### Ricezione  
Permette di registrare la ricezione del testo schedato da parte di una persona, anche diversa dal destinatario.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della ricezione.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_;  
* _allegato_.

Nel caso di più mittenti, destinatari, latori o allegati afferenti ad un medesima ricezione (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  

⚠️⚠️⚠️ Si inseriscono _allegati_ **soltanto** quando occorre registrare oggetti diversi da testi, per esempio manoscritti, monete, manufatti di qualsiasi tipo. Nel caso in cui siano ricevuti soltanto testi, questi ultimi vanno tutti inseriti come **_oggetto ricevuto_**. 

⚠️⚠️⚠️ **Quando i testi ricevuti siano più d'uno**, l'evento va **sempre inserito** a partire da un _item person_, dove è possibile aggiungere più _oggetti ricevuti_ - nella _Events Part_ di un _item work_ è possibile inserire soltanto la ricezione del testo descritto dall'_item_, aggiungendovi eventuali allegati, ma non è possibile aggiungere più testi ricevuti da una persona insieme a quello descritto dall'_item_.

⚠️⚠️⚠️ La ricezione séguita sempre da un invio. Ad ogni ricezione corrisponderà dunque **sempre** un invio - mentre non si darà sempre necessariamente il contrario. Se l'invio non è precisamente circostanziabile rispetto a luogo e data, si aggiungerà **almeno** come _termine ante quem_ la data in cui la lettera è stata ricevuta. I due eventi di _invio_ e _ricezione_ vanno inseriti e descritti singolarmente, e ad ognuno sarà attribuito un EID univoco: risulteranno però collegati attraverso l'inserimento, **obbligatorio**, di un medesimo _tag_. Vedi [qui](Events_Part.md#-tag) per la compilazione del _tag_. 
 

#### Scambio diretto  
Permette di inserire lo scambio diretto del testo schedato tra due persone.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dello scambio.   

È possibile indicare come entità _related_:  
* _consegna_: la persona che cede l'oggetto scambiato;  
* _destinatario_: la persona che riceve l'oggetto scambiato. 

⚠️⚠️⚠️ NON USARE MAI IL RELATED _ALLEGATO_: LA PRESENZA DI QUESTA VOCE È UN ERRORE CHE SARÀ RISOLTO AL PIÙ PRESTO. ⚠️⚠️⚠️ 

⚠️⚠️⚠️ **Quando gli oggetti scambiati siano più d'uno**, l'evento va **sempre inserito** a partire da un _item person_, dove è possibile aggiungere più _oggetti scambiati_ - nella _Events Part_ di un _item work_ è possibile inserire soltanto lo scambio di persona del testo descritto dall'_item_, aggiungendovi eventuali allegati, ma non è possibile aggiungere a questo altri testi scambiati.

⚠⚠️⚠️⚠️ Nel caso di scambi reciproci, cioè quando in un'unica occasione sono scambiati più oggetti da parte dei partecipanti allo scambio (p. es.: A dà un manoscritto a B e B dà un manoscritto ad A), **occorre creare più eventi _scambio diretto_** all'interno della _Events Part_ della persona da cui muove lo scambio. Alternativamente, **è possibile creare più eventi _scambio diretto_** all'interno della _Events Part_ dei diversi oggetti scambiati, specificando i ruoli dei partecipanti. In questi casi occorrerà compilare il campo _tag_ di ogni evento con un medesimo _tag_, così da permettere di ricondurre tutti gli scambi alla medesima occasione.

#### Lettura
Permette di inserire la lettura del testo schedato da una o più persone. 

⚠️⚠️⚠️ Si registrano eventi _lettura_ soltano per i testi, petrarcheschi o non, che rientrano nell'arco cronologico di interesse di Itinera, e dunque: testi di Petrarca, testi di corrispondenti, testi di corrispondenti di corrispondenti, etc. Non si inseriscono eventi di lettura per gli altri testi, per esempio i classici.

⚠️⚠️⚠️ Si registrano eventi _lettura_ **soltanto** per i testi di cui il lettore **non sia anche destinatario**, ovvero per i testi destinati ad altri di cui la persona sia entrata in possesso. Gli eventi _lettura_ **devono** seguitare da fatti accertati o accertabili, ad esempio dall'apposizione di postille o commenti su codici, oppure per esplicita dichiarazione della persona schedata nei suoi testi. **Non vanno registrati** come eventi _lettura_ quelli inferibili da rimandi intertestuali non circostanziabili, ma **si inseriscono eventi lettura** che facciano seguito a **citazioni esplicite di testi**, anche quando non siano note le modalità con cui la persona sia entrata in possesso del testo.

> Es. Nella lettera _Amor et dolor_ Francesco Nelli cita un verso dell'_Epyst. II 14_ di Petrarca. Si può dunque procedere all'inserimento di un evento lettura, che abbia Nelli per lettore e l'_Epyst. II 14_ come testo letto, avendo cura di inserire _Amor et dolor_ come fonte, e di indicare un rank adeguato (in questo caso 1, essendo la lettura probabile ma non certo).

⚠️⚠️⚠️ **Quando i testi letti siano più d'uno**, l'evento va **sempre inserito** a partire da un _item person_, dove è possibile aggiungere più _testi letti_ - nella _Events Part_ di un _item work_ è possibile inserire soltanto la lettura del testo descritto dall'_item_ da parte di una persona, ma non è possibile aggiungere a questo altri testi letti.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della lettura, ove nota.   

È obbligatorio indicare tra le entità _related_ la persona che ha letto il testo (_letto da_) e, ove noto, il mediatore della lettura (_mediata da_), vale a dire colui che ha materialmente fornito il testo alla persona che lo ha letto.

Nel caso in cui il testo sia letto da più persone **in uno stesso momento e/o occasione** (dunque con medesimo [Chronotope](Asserted_Chronotope_Brick.md)) si procede alla creazione di più elementi _related_ _letto da_.

Nel caso in cui la lettura del testo sia mediata da più persone **in uno stesso momento e/o occasione** (dunque con medesimo [Chronotope](Asserted_Chronotope_Brick.md)) si procede alla creazione di più elementi _related_ _mediato da_.

Nel caso in cui il testo sia letto da più persone **in momenti e/o occasioni diversi** (dunque con [Chronotope](Asserted_Chronotope_Brick.md) diverso) si procede alla creazione di più events _lettura_.

#### Trascrizione
Permette di registrare una trascrizione del testo.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della trascrizione.   

È possibile indicare come entità _related_:  
* la _copia_: il manoscritto che conserva la trascrizione, ove noto;
* il _trascrittore_: l'esecutore della copia, ove noto;

⚠️ Nel caso in cui la trascrizione proceda da una ricezione accertata, occcorre inserire e descrivere ciascun evento singolarmente, assegnando ad ognuno di essi da un EID univoco. La trascrizione e la ricezione (insieme eventulmente all'invio collegato a quest'ultima) risulteranno collegati attraverso l'inserimento di un medesimo _tag_. Vedi [qui](Events_Part.md#-tag) per la compilazione del _tag_. 

#### Raccolta
Permette di fornire informazioni sull'ingresso di un testo in una raccolta.    

La compilazione della **description** e dei **Chronotopes** è limitata a casi in cui sia nota, più o meno certamente, la data dell'ingresso e/o dell'uscita del testo in/da una raccolta, o a casi di particolare interesse o complessità come, per esempio, di lettere transitate da una raccolta all'altra, o di testi inizialmente inclusi e poi rifiutati nelle stesse. 

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento va compilato **solo** nel caso in cui sia nota, più o meno certamente, la data dell'ingresso e/o dell'uscita del testo in/da una raccolta.  

È obbligatorio indicare come entità _related_:  
* _raccolta_: la raccolta d'autore in cui è inserito il testo.    

#### Redazione
Permette di indicare quando il testo è la redazione precedente di un altro testo (ad es. _Sen_. XIII 11 gamma è redazione precedente di _Sen_. XIII 11 beta).  

La compilazione della **description** e dei **Chronotopes** è riservata a casi di particolare interesse o complessità, come per esempio lettere notevolmente rimaneggiate e/o smembrate a formare nuovi testi. In tutti gli altri casi, la _description_ e i _Chronotopes_ non vanno compilati.    

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della stesura del testo, quando nota, ovvero con il cronotopo inserito nella _Chronotope Part_.

È obbligatorio indicare tra le entità _related_:  
* _precedente di_: la redazione successiva del testo schedato.

Si inserisce tra i _related_ soltanto la redazione immediatamente successiva. Per esempio, nel caso di una lettera di cui siano attestate una redazione gamma, una redazione beta e una redazione alfa, l'_item_ relativo alla redazione gamma riporterà tra i _related_ **soltanto** la redazione beta; l'_item_ relativo alla redazione beta riporterà tra i _related_ **soltanto** la redazione alfa.  
Si aggiungono più _related_ **soltanto** nel caso in cui una redazione originaria abbia dato luogo, a seguito di smembramento, a due testi diversi.  
