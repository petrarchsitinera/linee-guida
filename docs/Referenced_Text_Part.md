# Referenced Text Part

**Referenced Text Part** permette di inserire e descrivere alcune relazioni del testo schedato con altri testi, in particolare:  
* il testo al quale il testo schedato risponde - per le tenzoni e per le corrispondenze in prosa;  
* i testi citati nel testo schedato.

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#referencedtextspart).

Per aggiungere la parte, selezionare **_ref-texts_** dal menu a tendina, quindi cliccare su **_add part_**. 


## Text
Per ogni testo collegato è creato un elemento _text_ mediante un [[editor|Editor_Brick]].

⚠️ Per quanto riguarda i testi di corrispondenza, si registrano in questa parte i soli testi collegati come antecedenti nella catena di corrispondenza rispetto al testo schedato. Non si registrano dunque eventuali risposte al testo schedato. L'intera catena di corrispondenza è ricostruita a posteriori sul grafo semantico grazie all'incrocio dei dati.

### Type
Permette di specificare il tipo di relazione che l'item schedato intrattiene con l'elemento _text_. Selezionare un valore tra:  
* risposta a (indica che l'item costituisce una risposta all'elemento _text_ indicato nel campo _target id_);
* citazione di (indica che l'item contiene una citazione dell'elemento _text_ indicato nel campo _target id_).

La compilazione del campo è obbligatoria.

### Target ID
🚧 ora con lookup??
Il testo interessato collegato all'item schedato.

La compilazione del campo è obbligatoria.

### Target citation
Il luogo del testo citato da cui è tratta la citazione, espresso secondo le convenzioni appropriate.

> es. 🚧

La compilazione del campo è facoltativa.

### Source
Il luogo del testo schedato in cui si verifica la citazione, espresso secondo le convenzioni appropriate.

> es. 🚧

La compilazione del campo è facoltativa.

### Assertion
Permette, mediante il modello [Assertion](Assertion_Brick.md) di indicare l'attendibilità del collegamento intertestuale e le eventuali fonti a sostegno.

## Save ⚠️ 
Per ogni elemento _text_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
