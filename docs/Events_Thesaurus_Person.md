# Thesaurus eventi Person 
# 🚧 Controllare voci perché thesaurus ristrutturato; spostare le due ultime voci in text e duplicare in text mutatis mutandis quelle ad esso relative)

Di seguito sono elencate le tipologie di evento (_type_) relativi alle persone e le tipologie di entità collegate (_related entities_).  

#### Nascita
Permette di inserire la nascita della persona schedata nell'_item_.    
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di nascita della persona.

Non è possibile aggiungere entità _related_.
    
#### Famiglia

Permette di inserire i membri della famiglia della persona schedata nell'_item_.   
🚧 Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide ...  

È obbligatorio indicare almeno un'entità _related_, scegliendo tra:
* _figlio_: il figlio della persona schedata;
* _figlia_: la figlia della persona schedata;
* _madre_: la madre della persona schedata;
* _padre_: il padre della persona schedata;
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

* _cardinale_: se la persona è nominata cardinale; 
* _vescovo_: se la persona è nominata vescovo;
* _frate_: se la persona è membro di un ordine religioso;
* _priore_: se la persona è nominata priore;
* _canonico_: se la persona è nominata canonico;
* _sovrano_: se la persona è un sovrano, a seguito di nomina, elezione o altro;
* _uomo politico_: se la persona esercita regolarmente attività politica all'interno di gerarchie laiche, quando non sia possibile precisare ulteriormente tale attività selezionando altre voci del _thesaurus_ (es. cancelliere, segretario, ecc.);
* _maestro_: se la persona esercita la professione di maestro di scuola o una generica attività didattica, anche privatamente. È possibile indicare come entità _related_ il _discepolo_, se il dato è disponibile o interessante da rilevare. Per ogni allievo si procede alla creazione di un elemento _related_;
* _lettore_: se la persona è un lettore conventuale, responsabile della formazione intellettuale del convento di appartenenza, o un docente universitario;
* _giurista_: se la persona è un giureconsulto o un dottore in legge, attivo o meno in ambito universitario;
* _diplomatico_: se la persona svolge attività diplomatica presso gerarchie laiche o ecclesiastiche, compiendo missioni e ambascerie per conto dell'istituzione per cui opera;
* _notaio_: se la persona esercita attività notarile, risultando perciò iscritto alla matricola dei notai nel luogo di formazione o di esercizio dell'attività;
* _uomo d'armi_: se la persona è un soldato, un condottiero, un mercenario, o risulta regolarmente impegnato in attività militari;
* _copista_: se la persona è un copista di professione. Non vannno considerati copisti tutti coloro che abbiano svolto attività di copia, anche per periodi prolungati, senza che fosse la loro attività principale;
* _artista_: se la persona è un artista, un decoratore, un miniatore, ecc.;
* _musico_: se la persona è un musico;
* _apprendista_: nel caso in cui la persona abbia completato un periodo di apprendistato professionale prima di esercitare autonomamente la professione;
* _consigliere_: se la persona è un consigliere, formalmente o informalmente incaricato, a servizio delle gerarchie presso cui opera, ed è dunque un membro stabile delle élites che amministrano la politica, l'economica e così via. Nel caso in cui la persona sia un consigliere personale, occorre creare un secondo evento professione _a servizio di_ per specificare nei _related_ la persona o le persone presso cui è svolta l'attività;
* _cancelliere_: se la persona svolge le funzioni di cancelliere di un'istituzione a seguito di un incarico formale;
* _segretario_: se la persona svolge le funzioni di segretario personale, oppure di segretario in un'istituzione, in questo caso a seguito di un incarico formale. Nel caso in cui la persona sia un segretario personale, occorre creare un secondo evento professione _a servizio di_ per specificare nei _related_ la persona o le persone presso cui è svolta l'attività;
* _mercante_: se la persona è un mercante o svolge attività legate alla mercatura;
* _artigiano_: se la persona è un artigiano;
* _servo_: se la persona è servitore di una o più persone;
* _imperatore_: se la persona è un imperatore, a seguito di nomina, elezione o altro.
* _medico_: se la persona è un medico;
* _duca_: se la persona è un duca, a seguito di nomina, elezione o altro;
* _conte_: se la persona è un conte, a seguito di nomina, elezione o altro;
* _principe_: se la persona è un principe;
* _a servizio di_: se la persona presta i propri servizi, per un periodo breve o lungo, ad un'altra persona - da non confondere con _servo_. In questo caso è obbligatorio indicare come entità _related_ la _persona_ che riceve il servizio.
* _protettore_: se la persona ha il ruolo di protettore e/o mecenate di una o più persone. In questo caso è obbligatorio indicare almeno nell'entità _related_ il _protetto_.


#### Titolo  
Permette di inserire eventuali titoli ricevuti dalla persona schedata nell'_item_ - titoli nobiliari, titoli di studio o altro.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della ricezione del titolo da parte della persona.   
Nel caso in cui il titolo dia luogo ad una posizione o ad un'attività descritta in un evento _Professione_, la data d'inizio di quest'ultima dovrà coincidere con il Chronotope del _Titolo_, che è sempre una data puntuale.

#### Nomina   

Permette di inserire eventuali nomine ricevute dalla persona schedata nell'_item_ - nomine a cariche pubbliche, universitarie, ecclesiastiche, ecc.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di nomina della persona.   
Nel caso in cui la nomina dia luogo ad una posizione o ad un'attività descritta in un evento _Professione_, la data d'inizio di quest'ultima dovrà coincidere con il Chronotope della _Nomina_, che è sempre una data puntuale.

#### Gruppo 

Permette di indicare se la persona è membro di un gruppo storicamente identificabile, afferente a istituzioni laiche o ecclesiastiche.   
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e l'intervallo di permanenza della persona nel gruppo, ove nota.   

#### Incontro

Permette di inserire gli incontri della persona schedata.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo in cui si è verificato l'incontro.   

È obbligatorio indicare come entità _related_ la _persona incontrata_. Per ogni  _persona incontrata_, si procede alla creazione di un singolo elemento _related_.

È possibile inoltre inserire uno o più _spettatori_, nel caso di incontri istituzionali o formali che prevedono una cerimonia della quale si vogliano indicare i presenti. Per ogni _spettatore_, si procede alla creazione di un singolo elemento _related_.

#### Viaggio 

Permette di inserire i viaggi della persona schedata.  
Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con la meta e la data o l'intervallo di tempo del viaggio.   

È possibile indicare come entità _related_ i _partecipanti_, quando al viaggio prendano parte altre persone. Per ogni _partecipante_, si procede alla creazione di un singolo elemento _related_.

#### Partecipazione  

Permette di inserire la partecipazione della persona schedata ad eventi non altrimenti descritti dal thesaurus, come ad esempio un'ambasceria.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo dell'attività cui la persona prende parte.   

È obbligatorio indicare come entità _related_ i _partecipanti_, quando al viaggio prendano parte altre persone. Per ogni _partecipante_, si procede alla creazione di un singolo elemento _related_.

#### Attestazione

Permette di inserire le attestazioni documentarie della persona schedata.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data del documento che dà luogo all'attestazione.   

È obbligatorio indicare come entità _related_ il _documento_ che dà luogo all'attestazione, indicato attraverso la segnatura archivistica dello stesso 
> es. AsBo, Notarile, San Giovanni in Monte, VI 5

#### Invio 

Permette di inserire l'invio di un oggetto (testo, manoscritto, altro) da parte della persona schedata.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'invio.   

È obbligatorio indicare come _related_ almeno un'entità tra _destinatario_ e _oggetto inviato_.  
Nel caso di più destinatari o di più oggetti inviati afferenti ad un medesimo invio (con un medesimo con _Chronotope_), si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

È possibile indicare inoltre come entità _related_ l'eventuale _latore_, ove noto, ovvero la persona cui è affidata la trasmissione dell'oggetto. 

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
* il _testo copiato_: il titolo del testo oggetto della copia, ovvero il titolo dell'antigrafo;


#### Raccolta di testi petrarcheschi

Permette di inserire eventuali attività di collezione di testi petrarcheschi da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della raccolta dei testi da parte della persona.   

È obbligatorio indicare tra le entità _related_:
* il _manoscritto_: il manoscritto che conserva la collezione raccolta dalla persona schedata, ove noto;
* il _testo raccolto_: il titolo del testo petrarchesco che la persona ha raccolto;

Nel caso di più testi petrarcheschi raccolti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti, si procede alla creazione di più eventi _Raccolta di testi petrarcheschi_.

#### Postilla

Permette di inserire eventuali attività di postillatura di testi da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo dell'attività di postillatura da parte della persona.

È obbligatorio indicare tra le entità _related_:
* il _manoscritto postillato_: il manoscritto che conserva le postille apposte dalla persona;
* il _testo postillato_: il titolo del testo postillato dalla persona;

Nel caso di più testi postillati, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti postillati, si procede alla creazione di più eventi _Postilla_.
 
#### Stesura
Permette di inserire la stesura di testi da parte della persona.

⚠️ L'evento stesura va inserito nella _Events Part_ di una persona soltanto quando risultino rispettate queste condizioni:
* il testo non è descritto in un _item_ autonomo;
* il titolo del testo è inserito *anche* nella _Work Part_ della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della stesura.

È obbligatorio indicare tra le entità _related_ il _testo_ composto dalla stesura, richiamandolo attraverso l'[_eid_](identifiers.md)

Nel caso di più testi, qualora il _Chronotope_ non coincida, si procede alla creazione di più eventi _Stesura_

#### Commissione

Permette di inserire eventuali commissioni di codici da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della commissione.

È obbligatorio indicare tra le entità _related_:
* il _manoscritto_: il manoscritto commmissionato;
* l'_esecutore_: la persona che materialmente allestisce o contribuisce ad allestire il codice, ove nota;

Nel caso di più esecutori, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti commissionati, si procede alla creazione di più eventi _Commissione_.

#### Esecuzione su commissione

Permette di inserire eventuali commissioni di codici ricevute dalla persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della commissione.

È obbligatorio indicare tra le entità _related_:
* il _manoscritto_: il manoscritto commmissionato;
* il _committente_: la persona che ha commissionato il manoscritto;

Nel caso di più committenti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.  
Nel caso di più manoscritti commissionati, si procede alla creazione di più eventi _Esecuzione su commissione_.

#### Dedica

Permette di inserire le dediche di testi o manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della dedica.

È obbligatorio indicare tra le entità _related_ il _dedicatario_.
Nel caso di più dedicatari, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

È obbligatorio inoltre indicare tra le entità _related_ l'oggetto dedicato, da scegliere tra:
* _testo_: il testo dedicato;
* _manoscritto_: il manoscritto dedicato;
 
Nel caso di più dediche, si procede alla creazione di più eventi _Dedica_.

#### Ricezione di dedica

Permette di inserire le dediche di testi o manoscritti ricevute della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data o l'intervallo di tempo della dedica.

È obbligatorio indicare tra le entità _related_ il _dedicante_.
Nel caso di più dedicanti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

È obbligatorio inoltre indicare tra le entità _related_ l'oggetto dedicato, da scegliere tra:
* _testo_: il testo dedicato;
* _manoscritto_: il manoscritto dedicato;
 
Nel caso di più dediche, si procede alla creazione di più eventi _Dedica_.

#### Possesso

Permette di inserire il possesso stabile di manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del possesso.

È obbligatorio indicare tra le entità _related_ il _manoscritto_.
Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.

#### Prestito

Permette di inserire il prestito di manoscritti da parte della persona (prestito da altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del prestito.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto preso in prestito, ove noto;
* _presta_: la persona da cui il manoscritto è preso in prestito, ove nota;

Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più prestatari, si procede alla creazione di più eventi _Prestito_.

#### Presta

Permette di inserire il prestito di manoscritti da parte della persona (prestito ad altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del prestito.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto preso in prestito, ove noto;
* _prende in prestito_: la persona a cui il manoscritto è dato in prestito, ove nota;

Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più persone cui si danno in prestito manoscritti, si procede alla creazione di più eventi _Presta_.

#### Restituisce

Permette di inserire la restituzione di manoscritti da parte della persona (restituzione ad altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di restituzione.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto restituito, ove noto;
* _ottiene restituzione_: la persona a cui il manoscritto è restituito, ove nota;

Nel caso di più persone cui si restituiscono manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più manoscritti, si procede alla creazione di più eventi _Restituzione_.

#### Ottiene restituzione

Permette di inserire la restituzione di manoscritti alla persona (restituzione da altri).

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di restituzione.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto restituito, ove noto;
* _restituisce_: la persona che restituisce il manoscritto, ove nota;

Nel caso di più persone che restituiscono manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più manoscritti, si procede alla creazione di più eventi _Ottiene restituzione_.

#### Acquista

Permette di inserire l'acquisto di manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'acquisto.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto acquistato, ove noto;
* _venditore_: la persona da cui si acquista manoscritto, ove nota;

Nel caso di più venditori, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più manoscritti, si procede alla creazione di più eventi _Acquista_.

#### Vendita

Permette di inserire la vendita di manoscritti da parte della persona.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della vendita.

È obbligatorio indicare tra le entità _related_ almeno uno tra:
* _manoscritto_: il manoscritto venduto, ove noto;
* _acquirente_: la persona cui si vende il manoscritto, ove nota;

Nel caso di più manoscritti, si procede alla creazione di un singolo elemento _related_ per ognuno di essi.
Nel caso di più acquirenti, si procede alla creazione di più eventi _Acquista_.

#### Raccolta

Permette di indicare quando il testo è parte di una raccolta d'autore.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'ingresso del testo in raccolta, ove noto.

È obbligatorio indicare tra le entità _related_ la _raccolta_, ovvero la raccolta d'autore in cui è inserito il testo.

#### Redazione

Permette di indicare quando il testo è la redazione precedente o successiva di un altro testo.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della stesura del testo.

È obbligatorio indicare tra le entità _related_ una tra:
* _precedente_: la redazione precedente del testo schedato;
* _successiva_: la redazione successiva del testo schedato;


