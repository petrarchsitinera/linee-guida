# Thesaurus eventi Person 
Di seguito sono elencate le tipologie di evento (_type_) relativi alle persone e le tipologie di entità collegate (_related entities_).  

#### Nascita
Permette di inserire la nascita della persona schedata nell'_item_.    
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di nascita della persona.

È possibile indicare come entità _related_:  
* _madre_: la madre della persona schedata;  
* _padre_: il padre della persona schedata.
    
#### Famiglia
Permette di inserire i membri della famiglia della persona schedata nell'_item_ (oltre al padre e alla madre, inseriti nell'evento _nascita_).   
🚧 Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide ...  

È obbligatorio indicare almeno un'entità _related_, scegliendo tra:
* _figlio_: il figlio della persona schedata;
* _figlia_: la figlia della persona schedata;
* _sorella_: la sorella della persona schedata;
* _fratello_: il fratello della persona schedata.

Per ogni figlio, figlia, fratello o sorella, si procede alla creazione di un singolo elemento _related_.

#### Morte 
Permette di inserire la morte della persona schedata nell'item.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di morte della persona.

Non è possibile aggiungere entità _related_.

#### Matrimonio  
Permette di inserire il matrimonio della persona schedata nell'_item_.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data del matrimonio inserito.  

È possibile indicare come entità _related_:
* _moglie_: la moglie della persona schedata a seguito del matrimonio;
* _marito_: il marito della persona schedata a seguito del matrimonio.


#### Professione   
Permette di inserire la professione della persona schedata nell'_item_. Con 'professione' ci si riferisce ad ogni tipo di attività. Possono essere inseriti profili professionali generici oppure specifici, di durata lunga e breve, nomine e cariche, servizi prestati presso gerarchie laiche o ecclesiastiche, e così via.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività, della carica o della nomina, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo (come nel caso delle nomine), si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.

Per ogni evento 'professione', il compilatore deve selezionare una voce tra quelle riportate di seguito. A più professioni o attività corrisponderanno più eventi 'professione'.

* _papa_: se la persona è nominata papa; 
* _cardinale_: se la persona è nominata cardinale; 
* _vescovo_: se la persona è nominata vescovo;
* _frate_: se la persona è membro di un ordine religioso;
* _priore_: se la persona è nominata priore;
* _canonico_: se la persona è nominata canonico;
* _sovrano_: se la persona è un sovrano, a seguito di nomina, elezione o altro;
* _uomo politico_: se la persona esercita regolarmente attività politica all'interno di gerarchie laiche, quando non sia possibile precisare ulteriormente tale attività selezionando altre voci del _thesaurus_ (es. cancelliere, segretario, ecc.);
* _maestro_: se la persona esercita la professione di maestro di scuola o una generica attività didattica, anche privatamente.  
  ⚠️ Nel caso in cui la persona abbia esercitato la funzione di maestro nei confronti di un'altra persona, occorre procedere, inoltre, alla creazione di un evento _maestro di_.   
* _lettore_: se la persona è un lettore conventuale, responsabile della formazione intellettuale del convento di appartenenza, o un docente universitario;
* _giurista_: se la persona è un giureconsulto o un dottore in legge, attivo o meno in ambito universitario;
* _diplomatico_: se la persona svolge attività diplomatica presso gerarchie laiche o ecclesiastiche, compiendo missioni e ambascerie per conto dell'istituzione per cui opera;
* _notaio_: se la persona esercita attività notarile, risultando perciò iscritto alla matricola dei notai nel luogo di formazione o di esercizio dell'attività;
* _uomo d'armi_: se la persona è un soldato, un condottiero, un mercenario, o risulta regolarmente impegnato in attività militari;
* _copista_: se la persona è un copista di professione. Non vannno considerati copisti tutti coloro che abbiano svolto attività di copia, anche per periodi prolungati, senza che fosse la loro attività principale;
* _artista_: se la persona è un artista, un decoratore, un miniatore, ecc.;
* _musico_: se la persona è un musico;
* _apprendista_: nel caso in cui la persona abbia completato un periodo di apprendistato professionale prima di esercitare autonomamente la professione;
* _consigliere_: se la persona è un consigliere, formalmente o informalmente incaricato, a servizio delle gerarchie presso cui opera, ed è dunque un membro stabile delle élites che amministrano la politica, l'economica e così via.   
 ⚠️ Nel caso in cui la persona sia un consigliere personale, occorre procedere, inoltre, alla creazione di un evento _consigliere di_.
* _cancelliere_: se la persona svolge le funzioni di cancelliere di un'istituzione a seguito di un incarico formale;
* _segretario_: se la persona svolge le funzioni di segretario personale, oppure di segretario in un'istituzione, in questo caso a seguito di un incarico formale.   
 ⚠️ Nel caso in cui la persona sia un segretario personale, occorre procedere, inoltre, alla creazione di un evento _segretario di_.  
* _mercante_: se la persona è un mercante o svolge attività legate alla mercatura;
* _banchiere_: se la persona è un banchiere o svolge attività legate al prestito di denaro;
* _artigiano_: se la persona è un artigiano;
* _servo_: se la persona è servitore di una o più persone;
* _imperatore_: se la persona è un imperatore, a seguito di nomina, elezione o altro.
* _medico_: se la persona è un medico;
* _duca_: se la persona è un duca, a seguito di nomina, elezione o altro;
* _conte_: se la persona è un conte, a seguito di nomina, elezione o altro;
* _principe_: se la persona è un principe;

#### Maestro di
Permette di indicare se la persona schedata ha esercitato la funzione di maestro nei confronti di un'altra persona.   
⚠️ 🚧 In presenza di un evento _maestro di_ occorre compilare sempre anche un evento _maestro_.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività.  

È obbligatorio indicare l'entità _related_:
* _allievo_: l'allievo della persona schedata.  

🚧 Per ogni _allievo_ si procede alla creazione di un elemento _related_. Se tuttavia i dati cronologici relativi al rapporto di discepolato differiscono, occorre procedere alla creazione di eventi _maestro di_ distinti.  

#### Allievo di
Permette di indicare se la persona schedata è stata allieva di un'altra persona.     
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività.  

È obbligatorio indicare l'entità _related_:
* _maestro_: il maestro della persona schedata.  

🚧 Per ogni rapporto di discepolato occorre creare eventi _allievo di_ distinti.  

#### Consigliere di
Permette di indicare se la persona schedata è stata consigliere personale, formalmente o informalmente incaricato, di qualcuno.  
⚠️ 🚧 In presenza di un evento _consigliere di_ occorre compilare sempre anche un evento _consigliere_.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.  

È obbligatorio indicare l'entità _related_:
* _persona_: la persona o le persone presso cui è svolta l'attività.  

🚧 Per ogni _persona_ si procede alla creazione di un elemento _related_. Se tuttavia i dati cronologici relativi al rapporto differiscono, occorre procedere alla creazione di eventi _consigliere di_ distinti. 

#### Segretario di
Permette di indicare se la persona schedata ha svolto le funzioni di segretario personale di qualcuno a seguito di un incarico formale.   
⚠️ 🚧 In presenza di un evento _segretario di_ occorre compilare sempre anche un evento _segretario_.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.  

È obbligatorio indicare l'entità _related_:
* _persona_: la persona o le persone presso cui è svolta l'attività.   

🚧 Per ogni _persona_ si procede alla creazione di un elemento _related_. Se tuttavia i dati cronologici relativi al rapporto differiscono, occorre procedere alla creazione di eventi _segretario di_ distinti. 

#### Servo di
Permette di indicare se la persona schedata ha svolto l'attività di servo presso qualcuno.     
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.  

È obbligatorio indicare l'entità _related_:
* _persona_: la persona o le persone presso cui è svolta l'attività.   

🚧 Per ogni _persona_ si procede alla creazione di un elemento _related_. Se tuttavia i dati cronologici relativi al rapporto differiscono, occorre procedere alla creazione di eventi _servo di_ distinti. 

#### A servizio di
Permette di indicare se la persona schedata ha pretato i propri servizi, per un periodo breve o lungo, ad un'altra persona - da non confondere con _servo_.  
⚠️ 🚧 Si ricorre a questo evento solo nel caso il rapporto non sia configurabile sotto le voci _consigliere di_ e _segretario di_.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.  

È obbligatorio indicare l'entità _related_:
* _protettore_: la persona o le persone presso cui è svolta l'attività.   

🚧 Per ogni _protettore_ si procede alla creazione di un elemento _related_. Se tuttavia i dati cronologici relativi al rapporto differiscono, occorre procedere alla creazione di eventi _a servizio di_ distinti. 

#### Protettore di
Permette di indicare se la persona schedata ha avuto il ruolo di protettore e/o mecenate di una o più persone   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.  

È obbligatorio indicare l'entità _related_:
* _persona_: la persona o le persone che hanno goduto della protezione.   

🚧 Per ogni _persona_ si procede alla creazione di un elemento _related_. Se tuttavia i dati cronologici relativi al rapporto differiscono, occorre procedere alla creazione di eventi _protettore di_ distinti.  

#### Nomina   
Permette di inserire eventuali nomine ricevute dalla persona schedata nell'_item_ - nomine a cariche pubbliche, universitarie, ecclesiastiche, ecc.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di nomina della persona.   
Nel caso in cui la nomina dia luogo ad una posizione o ad un'attività descritta in un evento _professione_, la data d'inizio di quest'ultima dovrà coincidere con il Chronotope della _nomina_, che è sempre una data puntuale.  
⚠️ 🚧 In questo caso, all'evento _professione_ e all'evento _nomina_ deve essere attribuito un identico _tag_.   

Non è possibile aggiungere entità _related_.   

#### Nomina ad un ufficio
Permette di inserire eventuali nomine ricevute dalla persona schedata nell'_item_, specificando l'ufficio 🚧.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata dell'attività, eventualmente coincidente con la morte della persona. Quando sia possibile individuare un preciso momento di inizio dell'attività nel tempo, si indicherà quel momento come inizio dell'attività. Se non si possiede nessun elemento cronologico, ma si presume che l'attività sia proseguita per l'intera vita della persona, si inserisce almeno la data di fine, che coincide con la data di morte della persona.  

È obbligatorio indicare l'entità _related_:
* _ufficio_: l'ufficio ricevuto in seguito alla nomina.

#### Titolo  
Permette di inserire eventuali titoli ricevuti dalla persona schedata nell'_item_ - titoli nobiliari, titoli di studio o altro.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della ricezione del titolo da parte della persona.   
Nel caso in cui il titolo dia luogo ad una posizione o ad un'attività descritta in un evento _professione_, la data d'inizio di quest'ultima dovrà coincidere con il Chronotope del _titolo_, che è sempre una data puntuale.  
⚠️ 🚧 In questo caso, all'evento _professione_ e all'evento _nomina_ deve essere attribuito un identico _tag_.   

Non è possibile aggiungere entità _related_.   

#### Gruppo 
Permette di indicare se la persona è membro di un gruppo storicamente identificabile, afferente a istituzioni laiche o ecclesiastiche.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e l'intervallo di permanenza della persona nel gruppo, ove nota.   

È possibile indicare come entità _related_:
* _membro di_: il gruppo di cui la persona è membro.

#### Incontro
Permette di inserire gli incontri della persona schedata.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo in cui si è verificato l'incontro.   

È obbligatorio indicare come entità _related_ la _persona incontrata_. Per ogni  _persona incontrata_, si procede alla creazione di un singolo elemento _related_.

È possibile inoltre inserire uno o più _spettatori_, nel caso di incontri istituzionali o formali che prevedono una cerimonia della quale si vogliano indicare i presenti. Per ogni _spettatore_, si procede alla creazione di un singolo elemento _related_.

#### Viaggio 
Permette di inserire i viaggi della persona schedata.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con la meta e la data o l'intervallo di tempo del viaggio.   

È possibile indicare come entità _related_ i _partecipanti_, quando al viaggio prendano parte altre persone. Per ogni _partecipante_, si procede alla creazione di un singolo elemento _related_.

⚠️ 🚧 _tag_ per tappe   

#### Partecipazione  
Permette di inserire la partecipazione della persona schedata ad eventi non altrimenti descritti dal thesaurus, come ad esempio un'ambasceria.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo dell'attività cui la persona prende parte.   

È obbligatorio indicare come entità _related_ i _partecipanti_, quando al viaggio prendano parte altre persone. Per ogni _partecipante_, si procede alla creazione di un singolo elemento _related_.

#### Attestazione
Permette di inserire l'elenco delle attestazioni documentarie della persona schedata.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data del documento che dà luogo all'attestazione.   
Per ogni Chronotope sono inserite nell'_assertion_ relativa al campo _date_ le segnature archivistiche dei documenti che danno luogo all'attestazione.  
> es. AsBo, Notarile, San Giovanni in Monte, VI 5

#### Invio 
Permette di inserire l'invio di un oggetto (testo, manoscritto, altro) da parte della persona schedata.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'invio.   

È obbligatorio indicare come _related_ almeno un'entità tra _destinatario_ e _oggetto inviato_.  
Nel caso di più destinatari o di più oggetti inviati afferenti ad un medesimo invio (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

È possibile indicare inoltre come entità _related_ l'eventuale _latore_, ove noto, ovvero la persona cui è affidata la trasmissione dell'oggetto. 

⚠️ 🚧 _tag_ per invio+ricezione+consegna  

#### Ricezione   
Permette di inserire la ricezione di un oggetto (testo, manoscritto, altro) da parte della persona schedata.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della ricezione.   

È obbligatorio indicare come _related_ almeno un'entità tra _mittente_ e _oggetto ricevuto_ .   
Nel caso di più mittenti o di più oggetti ricevuti afferenti ad un medesima ricezione (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

È possibile indicare inoltre come entità _related_ l'eventuale _latore_, ove noto, ovvero la persona cui è affidata la trasmissione dell'oggetto.

#### Consegna  
Permette di inserire la consegna di un oggetto (testo, manoscritto, altro) da parte della persona schedata. Rientra nella consegna anche lo scambio diretto di oggetti.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della consegna.   

È obbligatorio indicare almeno una entità _related_ tra _oggetto consegnato_, _mittente_ e _destinatario_.   
Nel caso più oggetti consegnati, di più destinatari o di più mittenti, afferenti ad una medesima consegna (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

#### Trascrizione
Permette di inserire la puntuale attività di trascrizione di un testo da parte di una persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della trascrizione.   

In linea generale, è sempre obbligatorio indicare tra le entità _related_:
* la _copia_: il manoscritto che conserva la trascrizione materialmente eseguita dalla persona, ove noto;
* il _testo trascritto_: il titolo del testo oggetto della copia, ovvero il titolo dell'antigrafo;

#### Raccolta di testi petrarcheschi
Permette di inserire eventuali attività di collezione di testi petrarcheschi da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della raccolta dei testi da parte della persona.   

È obbligatorio indicare tra le entità _related_:
* il _manoscritto_: il manoscritto che conserva la collezione raccolta dalla persona schedata, ove noto;
* il _testo raccolto_: il titolo del testo petrarchesco che la persona ha raccolto;

Nel caso di più testi petrarcheschi raccolti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti, si procede alla creazione di più eventi _raccolta di testi petrarcheschi_.

#### Postilla
Permette di inserire eventuali attività di postillatura di testi da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo dell'attività di postillatura da parte della persona.

È obbligatorio indicare tra le entità _related_:
* il _manoscritto postillato_: il manoscritto che conserva le postille apposte dalla persona;
* il _testo postillato_: il titolo del testo postillato dalla persona;

Nel caso di più testi postillati, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti postillati, si procede alla creazione di più eventi _postilla_.
 
#### Scrittura
Permette di stabilire una corrispondenza tra la persona schedata e una mano registrata in un Item Manuscript (in [Hands Part](Hands_Part.md)).  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento non deve essere compilato.   

È obbligatorio indicare come entità _related_:
* _mano_: richiamare attraverso [lookup](lookup.md) l'_eid_ assegnato alla mano di interesse, avendo cura di premettervi, separato da "/", l'_eid_ del manoscritto.  
 
#### Stesura
Permette di inserire la stesura di testi da parte della persona.

⚠️ L'evento stesura va inserito nella _Events Part_ di una persona soltanto quando risultino rispettate queste condizioni:
* il testo non è descritto in un _item_ autonomo;
* il titolo del testo è inserito *anche* nella _Work Part_ della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della stesura.

È obbligatorio indicare tra le entità _related_ il _testo_ composto dalla stesura, richiamandolo attraverso l'[_eid_](identifiers.md)

Nel caso di più testi, qualora il _Chronotope_ non coincida, si procede alla creazione di più eventi _stesura_

#### Commissione
Permette di inserire eventuali commissioni di codici da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della commissione.

È obbligatorio indicare tra le entità _related_:
* il _manoscritto_: il manoscritto commmissionato;
* l'_esecutore_: la persona che materialmente allestisce o contribuisce ad allestire il codice, ove nota;

Nel caso di più esecutori, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti commissionati, si procede alla creazione di più eventi _commissione_.

#### Esecuzione su commissione
Permette di inserire eventuali commissioni di codici ricevute dalla persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della commissione.

È obbligatorio indicare tra le entità _related_:
* il _manoscritto_: il manoscritto commmissionato;
* il _committente_: la persona che ha commissionato il manoscritto;

Nel caso di più committenti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti commissionati, si procede alla creazione di più eventi _esecuzione su commissione_.

#### Dedica
Permette di inserire le dediche di testi o manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della dedica.

È obbligatorio indicare tra le entità _related_ il _dedicatario_.
Nel caso di più dedicatari, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

È obbligatorio inoltre indicare tra le entità _related_ l'oggetto dedicato, da scegliere tra:
* _testo_: il testo dedicato;
* _manoscritto_: il manoscritto dedicato;
 
Nel caso di più dediche, si procede alla creazione di più eventi _dedica_.

#### Ricezione di dedica
Permette di inserire le dediche di testi o manoscritti ricevute della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della dedica.

È obbligatorio indicare tra le entità _related_ il _dedicante_.
Nel caso di più dedicanti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

È obbligatorio inoltre indicare tra le entità _related_ l'oggetto dedicato, da scegliere tra:
* _testo_: il testo dedicato;
* _manoscritto_: il manoscritto dedicato;
 
Nel caso di più dediche, si procede alla creazione di più eventi _ricezione di dedica_.

#### Possesso

Permette di inserire il possesso stabile di manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del possesso.

È obbligatorio indicare tra le entità _related_ il _manoscritto_.
Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

#### Prende in prestito
Permette di inserire il prestito di manoscritti da parte della persona (prestito da altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del prestito.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto preso in prestito, ove noto;
* _presta_: la persona da cui il manoscritto è preso in prestito, ove nota;

Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più prestatari, si procede alla creazione di più eventi _prende in prestito_.

#### Presta
Permette di inserire il prestito di manoscritti da parte della persona (prestito ad altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del prestito.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto preso in prestito, ove noto;
* _prende in prestito_: la persona a cui il manoscritto è dato in prestito, ove nota;

Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più persone cui si danno in prestito manoscritti, si procede alla creazione di più eventi _presta_.

#### Restituisce
Permette di inserire la restituzione di manoscritti da parte della persona (restituzione ad altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di restituzione.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto restituito, ove noto;
* _ottiene restituzione_: la persona a cui il manoscritto è restituito, ove nota;

Nel caso di più persone cui si restituiscono manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più manoscritti, si procede alla creazione di più eventi _restituisce_.

#### Ottiene restituzione
Permette di inserire la restituzione di manoscritti alla persona (restituzione da altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di restituzione.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto restituito, ove noto;
* _restituisce_: la persona che restituisce il manoscritto, ove nota;

Nel caso di più persone che restituiscono manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più manoscritti, si procede alla creazione di più eventi _ottiene restituzione_.

#### Acquista
Permette di inserire l'acquisto di manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'acquisto.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto acquistato, ove noto;
* _venditore_: la persona da cui si acquista manoscritto, ove nota;

Nel caso di più venditori, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più manoscritti, si procede alla creazione di più eventi _acquista_.

#### Vende
Permette di inserire la vendita di manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della vendita.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto venduto, ove noto;
* _acquirente_: la persona cui si vende il manoscritto, ove nota;

Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più acquirenti, si procede alla creazione di più eventi _acquista_.
