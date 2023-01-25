# Related Persons Part

**Related Persons Part** permette di elencare le persone collegate al testo.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#relatedpersonspart).  

Per aggiungere la parte, selezionare **_rel-persons_** dal menu a tendina, quindi cliccare su **_add part_**. 

## Person
Per ogni persona collegata è creato un elemento _person_ mediante un [editor](Editor_Brick.md).

### Type
Permette di specificare il tipo di relazione che la persona da inserire intrattiene con l'item _text_ schedato. Selezionare un valore tra:  
* citato (la persona è citata nel testo);
* pseudonimo (la persona è citata nel testo mediante uno pseudonimo);
* destinatario (la persona è il destinatario diretto ed esplicito del testo);
* dedicatario (la persona è il dedicatario primario ed esplicito del testo);
* richiesta di recapito a (la persona è indicata nel testo come ulteriore destinatario cui recapitare il testo).  

La compilazione del campo è obbligatoria.

### Name
Il nome della persona nella forma presente a testo.  
In presenza di più citazioni riferite ad un sola persona, si privilegia la forma più esplicita, possibilmente il nome, normalizzata al nominativo.  

La compilazione del campo è obbligatoria.

### Id 🚧 MA ORA VEDI CON LOOKUP
Permette di collegare il nome inserito ad una o più persone storicamente individuate.

Il collegamento avviene attraverso l'inserimento dell'ID della persona, sia essa schedata nel database di Itinera oppure in risorse esterne.
Nel primo caso, l'**external ID** corrisponde all'ID dell'item persona, cioè al **title** dell'item, e lo **scope** a **Itinera**.
Per gli altri casi consultare le indicazioni per la compilazione di [[ExternalIDs|External_IDs_Part]]

### Assertion 🚧 MA ELIMINARE PERCHè ORA è ASSERTED ID quindi tutta la spiega è nel brick corrisp.
Permette, mediante il modello [Assertion](Assertion_Brick.md) di indicare l'attendibilità dell'identificazione e le eventuali fonti a sostegno.

## Save ⚠️ 

Per ogni elemento _person_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
