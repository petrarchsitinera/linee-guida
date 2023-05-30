# Asserted Chronotopes Part

Permette di inserire data e luogo di **stesura** di un testo.  
Ulteriori dati cronotopici relativi a eventuali invii, ricezioni, etc., vanno inseriti in [Events Part](Events_Part.md).  

La parte è strutturata secondo il modello [AssertedChronotope](Asserted_Chronotope_Brick.md). Per istruzioni sulla compilazione dei _chronotopes_, cliccare [qui](Asserted_Chronotope_Brick.md).  

È possibile creare più _chronotopes_, a seconda della tipologia di datazione nota, qualificando ciascuno di essi attraverso il _tag_ dei campi _place_ e _date_.   

⚠️ I _tag_ da compilare sono quelli relativi ai campi _place_ e _date_ (cerchiati in rosso nell'immagine), da non confondere con i _tag_ presenti nel riquadro delle _assertions_.  

<img width="986" alt="Schermata 2023-04-03 alle 15 08 45" src="https://user-images.githubusercontent.com/102725489/229519331-798c2aca-c6e7-4ef9-8521-724321f6c265.png">

⚠️ I _tag_ di _place_ e _date_ **devono essere sempre scritti in minuscolo**.  

Per le lettere petrarchesche, compilare il campo _tag_ con **uno** dei seguenti valori:

* stesura dichiarata: per il luogo e/o la data dichiarati in calce alla lettera, riportati al calendario gregoriano. In caso di date dichiarate comprensive soltanto di giorno e mese, compilare il campo _value_ con l'indicazione del secolo;  
* stesura implicita: per il luogo e/o la data di cui gli elementi siano desunti, tutti o in parte, da elementi interni al testo o dalla posizione del testo all'interno della raccolta;  
* stesura ricostruita: per il luogo e/o la data ricostruiti dalla critica, anche se eventualmente divergenti da quelli dichiarati e/o impliciti. In presenza di una stesura ricostruita è **sempre** obbligatoria l'indicazione della fonte del dato: se la fonte si riferisce sia al luogo sia alla data, essa va riportata in entambe le _assertion_.
* altro: per elementi cronologici e termini _ante_ e _post quem_ desumibili dalla lettera, riferiti ad eventi o fatti storici puntuali utili alla datazione del testo stesso, anche in presenza di ipotesi di stesura più o meno certe. In questo caso, i termini cronologici da inserire **coincidono** con la data degli eventi o dei fatti puntuali riportati a testo.   

Per le lettere non petrarchesche, compilare il campo _tag_ con **uno** dei seguenti valori:

* stesura dichiarata: per il luogo e/o la data dichiarati in calce alla lettera, riportati al calendario gregoriano. In caso di date dichiarate comprensive soltanto di giorno e mese, compilare il campo _value_ con l'indicazione del secolo;   
* stesura ricostruita: per il luogo e/o la data ricostruiti dalla critica, eventualmente divergenti da quelli dichiarati. In presenza di una stesura ricostruita è **sempre** obbligatoria l'indicazione della fonte del dato: se la fonte si riferisce sia al luogo sia alla data, essa va riportata in entambe le _assertion_.  
* altro: per elementi cronologici e termini _ante_ e _post quem_ desumibili dalla lettera, riferiti ad eventi o fatti storici puntuali utili alla datazione del testo stesso, anche in presenza di ipotesi di stesura più o meno certe. In questo caso, i termini cronologici da inserire **coincidono** con la data degli eventi o dei fatti puntuali riportati a testo.

Per le lettere perdute, compilare il campo _tag_ con **uno** dei seguenti valori:   

* stesura ricostruita: per il luogo e/o la data di stesura ricostruita dalla critica. In presenza di una stesura ricostruita è **sempre** obbligatoria l'indicazione della fonte del dato: se la fonte si riferisce sia al luogo sia alla data, essa va riportata in entambe le _assertion_.  
* altro: per termini _ante_ e _post quem_. Per le lettere perdutee è **sempre obbligatorio** inserire come termine _ante quem_ la data di stesura della lettera che costituisce la fonte di informazione sul testo perduto.


⚠️⚠️⚠️ I _tag_ di _place_ e _date_ devono essere coerenti all'interno dell'elemento _chronotope_. Ciascun _chronotope_ deve cioè raccogliere:   
- **o** la stesura dichiarata 
- **o** la stesura implicita 
- **o** i dati relativi ad **una** ipotesi di datazione ricostruita  
- **o** altri elementi cronologici utili alla datazione della lettera.  

In nessun caso si potrà usare, ad esempio, il _tag_ "stesura ricostruita" per un luogo ipotizzato dalla critica come luogo di stesura di un testo accanto ad una data qualificata come "stesura dichiarata".  


<img width="1430" alt="Schermata 2023-04-03 alle 15 48 20" src="https://user-images.githubusercontent.com/102725489/229530035-645d5f2a-2366-4b61-9718-f80cc7eab0a0.png">



⚠️ In presenza di più elementi _chronotope_, il compilatore deve specificare quale di essi sia da considerare quello di riferimento: deve quindi aggiungere ai _tag_ di _place_ e _date_ del _chronotope_ di riferimento la dicitura _principale_, separata da punto e virgola.  

> Es. stesura ricostruita; principale

È **obbligatoria** la creazione di un _chronotope_ per la _stesura dichiarata_ e la _stesura implicita_ in presenza dei rispettivi dati. Essendo la fonte di tali dati il testo schedato, non è prevista la compilazione dell'_assertion_.   
È possibile creare un _chronotope_ per ogni _stesura ricostruita_, cioè per ogni ipotesi critica avanzata nella letteratura. In questi casi, la cmpilazione delle relative _asssertion_ è **sempre obbligatoria**.
