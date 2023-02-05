# Thesaurus eventi 🚧


Il **thesaurus eventi**, unico per tutte le tipologie di _item_, è strutturato come un _thesaurus_ gerarchico.   
Le relazioni che le entità collegate intrattengono con l'_item_ in cui l'evento è inserito dipendono dalla tipologia dell'evento. 
Una volta selezionata la tipologia di un evento in _general_, in altre parole, per le entità _related_ sarà possibile selezionare soltanto le relazioni previste per quella tipologia di evento.  

> Ad esempio, dopo aver selezionato _matrimonio_, non sarà possibile selezionare _persona incontrata_ come relazione per il _related_. _matrimonio_ ha infatti come relazioni possibili soltanto _marito_ e _moglie_.

La/e persona/e inserita/e tra i _related_ può/possono non essere schedata nel database Itinera.

Di seguito è fornita la lista commentata delle voci.

***

#### Nascita
Permette di inserire la nascita della persona schedata nell'_item_. Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con la data di nascita della persona.

Non è possibile aggiungere entità _related_.
    
#### Famiglia

Permette di inserire i membri della famiglia della persona schedata nell'_item_. 🚧 Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide ...  
Selezionando l'evento _famiglia_, è possibile indicare come entità _related_:
* _figlio_: il figlio della persona schedata;
* _figlia_: la figlia della persona schedata;
* _madre_: la madre della persona schedata;
* _padre_: il padre della persona schedata;
* _sorella_: la sorella della persona schedata;
* _fratello_: il marito della persona schedata.

Per ogni figlio, figlia, fratello o sorella, si procede alla creazione di un singolo elemento _related_.

#### Morte 

Permette di inserire la _morte_ della persona schedata nell'item. Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con la data di morte della persona.

Non è possibile aggiungere entità _related_.

#### Matrimonio  

Permette di inserire il matrimonio della persona schedata nell'_item_. Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con la data del matrimonio inserito.  
Selezionando l'evento _matrimonio_, è possibile indicare come entità _related_:
* _moglie_: la moglie della persona schedata a seguito del matrimonio;
* _marito_: il marito della persona schedata a seguito del matrimonio.

Per ogni allievo si procede alla creazione di un elemento _related_.

#### Professione   
Permette di inserire la professione della persona schedata nell'_item_. Con 'professione' ci si riferisce ad ogni tipo di attività. Possono essere inseriti profili professionali generici oppure specifici, di durata lunga e breve, nomine e cariche, servizi prestati presso gerarchie laiche o ecclesiastiche, e così via.  
Il [Chronotope] (Asserted_Chronotope_Brick.md) dell'evento coincide con la durata dell'attività, della carica o della nomina, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo (come nel caso delle nomine), si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.

Per ogni evento 'professione', il compilatore deve selezionare una voce tra quelle riportate di seguito. A più professioni o attività corrisponderanno più elementi 'professione'.

* _cardinale_: se la persona è nominata cardinale; 
* _vescovo_: se la persona è nominata vescovo;
* _frate_: se la persona è membro di un ordine religioso;
* _priore_: se la persona è nominata priore;
* _canonico_: se la persona è nominata canonico;
* _sovrano_: se la persona è un sovrano, a seguito di nomina, elezione o altro.
* _uomo politico_: se la persona esercita regolarmente attività politica all'interno di gerarchie laiche; [🚧PRECISARE MEGLIO]
* _maestro_: se la persona esercita la professione di maestro di scuola o una generica attività didattica, anche privatamente. È possibile indicare come entità _related_ il _discepolo_, se il dato è disponibile o interessante da rilevare. Per ogni allievo si procede alla creazione di un elemento _related_.
* _lettore_: se la persona è un lettore conventuale, responsabile della formazione intellettuale del convento di appartenenza;
* _giurista_: se la persona è un giureconsulto o un dottore in legge, attivo o meno in ambito universitario;
* _diplomatico_: se la persona svolge attività diplomatica presso gerarchie laiche o ecclesiastiche, compiendo missioni e ambascerie per conto dell'istituzione per cui opera;
* _notaio_: se la persona esercita attività notarile, risultando perciò iscritto alla matricola dei notai nel luogo di formazione o di esercizio dell'attività;
* _uomo d'armi_: se la persona è un soldato, un condottiero, un mercenario, o risulta regolarmente impegnato in attività militari;
* _copista_: se la persona è un copista, di professione o meno;
* _artista_: se la persona è un artista, un decoratore, un miniatore, ecc.;
* _musico_: se la persona è un musico;
* _apprendista_: nel caso in cui la persona abbia trascorso un apprendistato professionale prima di esercitare autonomamente la professione;
* _consigliere_: se la persona è un consigliere, formalmente o informalmente incaricato, a servizio delle gerarchie presso cui opera, ed è dunque un membro stabile delle élites che amministrano la politica, l'economica e così via;
* _cancelliere_: se la persona svolge le funzioni di cancelliere di un'istituzione a seguito di un incarico formale;
* _segretario_: se la persona svolge le funzioni di segretario personale, oppure di segretario in un'istituzione, in questo caso a seguito di un incarico formale; 
* _mercante_: se la persona è un mercante o svolge attività legate alla mercatura;
* _artigiano_: se la persona è un artigiano;
* _servo_: se la persona è servitore di una o più persone;
* _imperatore_: se la persona è un imperatore, a seguito di nomina, elezione o altro.
* _medico_: se la persona è un medico;
* _duca_: se la persona è un duca, a seguito di nomina, elezione o altro;
* _conte_: se la persona è un conte, a seguito di nomina, elezione o altro;
* _principe_: se la persona è un principe;
* _a servizio di_: se la persona presta i propri servizi, per un periodo breve o lungo, ad un'altra persona - da non confondere con _servo_. In questo caso è obbligatorio indicare come entità _related_ il _protettore_.
* _protettore_: se la persona ha il ruolo di protettore e/o mecenate di una o più persone. In questo caso è obbligatorio indicare almeno nell'entità _related_ il _protettore_.


#### Titolo  

#### Nomina   

#### Gruppo 

#### Incontro  

#### Viaggio 

#### Partecipazione  

#### Attestazione

#### Invio 

#### Ricezione   

#### Consegna  

#### Scambio 

#### Trascrizione

#### Postilla 

#### Raccolta

#### Stesura 

#### Risposta   
 
#### Testimone manoscritto 

#### Redazione

#### Edit

#### Commissione

#### Dedica

#### Possesso

#### Prestito

#### Restituzione

#### Acquisto

#### Restauro

#### Smembramento      
