# Thesaurus eventi Work 
Di seguito sono elencate le tipologie di evento (_type_) relativi ai testi e le tipologie di entità collegate (_related entities_).  


#### Invio 
Permette di registrare l'invio del testo.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'invio.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_.  

Nel caso di più mittenti, destinatari o latori afferenti ad un medesimo invio (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
⚠️ 🚧 _tag_ per invio+ricezione+consegna  

#### Ricezione  
Permette di registrare la ricezione del manoscritto da parte di una persona.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della ricezione.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_.  

Nel caso di più mittenti, destinatari o latori afferenti ad un medesima ricezione (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
⚠️ 🚧 _tag_ per invio+ricezione+consegna  

#### Consegna  
Permette di registrare la consegna del manoscritto da parte di una persona ad un'altra.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della consegna.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_.  

Nel caso di più mittenti, destinatari o latori afferenti ad una medesima consegna (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

#### Trascrizione
Permette di registrare una trascrizione del testo.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della trascrizione.   

È possibile indicare come entità _related_:  
* la _copia_: il manoscritto che conserva la trascrizione, ove noto;
* il _trascrittore_: l'esecutore della copia, ove noto;

#### Stesura 🚧 ELIMINARE
Permette di indicare autore e data di stesura del testo schedato

⚠️ L'evento stesura va inserito nella _Events Part_ di un testo soltanto quando risultino rispettate queste condizioni:
* il testo non è descritto in un _item_ autonomo;
* il titolo del testo è inserito *anche* nella _Work Part_ della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della stesura.


#### Raccolta
Permette di indicare quando il testo è parte di una raccolta d'autore.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'ingresso del testo in raccolta, ove noto.

È obbligatorio indicare come entità _related_:  
* _raccolta_: la raccolta d'autore in cui è inserito il testo.  

#### Redazione
Permette di indicare quando il testo è la redazione precedente o successiva di un altro testo.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della stesura del testo.

È obbligatorio indicare tra le entità _related_ una tra:
* _precedente_: la redazione precedente del testo schedato;
* _successiva_: la redazione successiva del testo schedato.
