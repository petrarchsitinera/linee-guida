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
* _eid mano_: richiamare attraverso [lookup](lookup.md) l'_eid_ assegnato alla mano di interesse, avendo cura di premettervi, separato da "/", l'_eid_ del manoscritto; 
* _copista_: se il copista coincide con un Item Person, richiamare attraverso [lookup](lookup.md) l'_eid_ ad esso assegnato; se il copista è sprovvisto di un Item Person, è consigliabile procedere alla sua creazione e richiamarne l'_eid_, avendo cura di aggiungerlo all'elenco dei copisti nel [repository](repositories.md).  

⚠️ Si registrano: copisti storicamente identificati; copisti anonimi noti agli studi per la loro produzione (es. "copista principale del Dante dei Cento"); qualsiasi copista la cui mano sia riconosciuta su almeno due manoscritti; tutti i copisti per cui sia possibile fornire qualche informazione biografica (es. notaio, copista di professione, etc.).  

#### Editing
Permette di attribuire ad un personaggio noto gli interventi scrittori successivi alla copia del codice registrati in [Edits Part](Edits_Part.md).  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'intervento scrittorio.  

Indicare come entità _related_:  
* _eid edit_: richiamare attraverso [lookup](lookup.md) l'_eid_ assegnato all'_edit_, avendo cura di premettervi, separato da "/", l'_eid_ del manoscritto;  
* _eseguito da_: l'autore dell'intervento scrittorio.   

#### Commissione
Permette di inserire informazioni sulla commissione del manoscritto.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento non deve essere compilato, a meno che non siano note ulteriori informazioni sulla commissione, diverse dalla data di esecuzione del manoscritto registrata in [Material Description Part](Material_Description_Part.md).  

È possibile indicare come entità _related_:  
* _committente_: la persona che ha commissionato il manoscritto;  
* _esecutore_: la persona (o bottega, etc.) che riceve la commissione, ed eventualmente allestisce o contribuisce ad allestire il codice.  

#### Dedica
Permette di inserire informazioni sulla dedica del manoscritto.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento non deve essere compilato, a meno che non siano note ulteriori informazioni sulla dedica, diverse dalla data di esecuzione del manoscritto registrata in [Material Description Part](Material_Description_Part.md).  

È possibile indicare come entità _related_: 
* _dedicante_: la persona che dedica il manoscritto;
* _dedicatario_: la persona cui è dedicato il manoscritto.  

#### Possesso
Permette di indicare il possesso stabile del manoscritto da parte di una persona o di un ente.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del possesso.

Indicare come entità _related_: 
* _possessore_: la persona o ente che possiede il manoscritto;  
* _attestato da_: se presente una nota di possesso, richiamare attraverso [lookup](lookup.md) l'_eid_ assegnato all'_edit_ relativo, avendo cura di premettervi, separato da "/", l'_eid_ del manoscritto.


#### Prestito
Permette di registrare il prestito del manoscritto.  

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la durata del prestito.

Indicare come entità _related_: 
* _prende in prestito_: la persona o ente a cui il manoscritto è dato in prestito;
* _presta_: la persona o ente da cui il manoscritto è preso in prestito.

#### Restituzione
Permette di registrare la restituzione del manoscritto dopo prestito, furto, etc.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data di restituzione.

Indicare come entità _related_: 
* _restituisce_: la persona o ente che restituisce il manoscritto;  
* _ottiene restituzione_: la persona o ente a cui il manoscritto è restituito.  

#### Acquisto
Permette di registrare l'acquisto o la vendita del manoscritto.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'acquisto.

Indicare come entità _related_: 
* _acquirente_: la persona o ente che acquista il manoscritto;  
* _venditore_: la persona o ente che vende il manoscritto.  

#### Restauro
Permette di registrare gli interventi di restauro del manoscritto.

Il [Chronotope](Asserted_Chronotope_Brick.md) dell'evento coincide con il luogo e la data dell'intervento di restauro.

Indicare come entità _related_: 
* _restauratore_: la persona o ente responsabile del restauro.   
