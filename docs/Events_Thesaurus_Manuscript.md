# Thesaurus eventi Manuscript 

Di seguito sono elencate le tipologie di evento (_type_) relativi ai manoscritti e le tipologie di entità collegate (_related entities_).  


#### Invio 
Permette di registrare l'invio del manoscritto.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'invio.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_.  

#### Ricezione  
Permette di registrare la ricezione del manoscritto da parte di una persona.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della ricezione.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_.  

#### Consegna  
Permette di registrare la consegna del manoscritto da parte di una persona ad un'altra.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data della consegna.   

È possibile indicare come entità _related_:  
* _mittente_;  
* _destinatario_;  
* _latore_.  

#### Scrittura
Permette di stabilire una corrispondenza tra una delle mani presenti nel codice e un copista noto.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento non deve essere compilato.   

Indicare come entità _related_:  
* _eid mano_: richiamare attraverso [lookup](lookup.md) l'_eid_ assegnato alla mano di interesse, avendo cura di premettervi l'_eid_ del manoscritto;  
* _copista_.  

#### Editing
Permette di stabilire una corrispondenza tra una delle mani presenti nel codice e un copista noto.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento non deve essere compilato.   

Indicare come entità _related_:  
* _eid mano_: richiamare attraverso [lookup](lookup.md) l'_eid_ assegnato alla mano di interesse, avendo cura di premettervi l'_eid_ del manoscritto;  
* _copista_.  




      {
        "id": "manuscript.editing",
        "value": "manoscritto: editing"
      },
      {
        "id": "manuscript.commission",
        "value": "manoscritto: commissione"
      },
      {
        "id": "manuscript.dedication",
        "value": "manoscritto: dedica"
      },
      {
        "id": "manuscript.possession",
        "value": "manoscritto: possesso"
      },
      {
        "id": "manuscript.lend",
        "value": "manoscritto: prestito"
      },
      {
        "id": "manuscript.return",
        "value": "manoscritto: restituzione"
      },
      {
        "id": "manuscript.buy",
        "value": "manoscritto: acquisto"
      },
      {
        "id": "manuscript.restore",
        "value": "manoscritto: restauro"
      }
