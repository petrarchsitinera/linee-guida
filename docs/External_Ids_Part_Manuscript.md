# External IDs Part
**External IDs Part** raccoglie gli identificativi dell'item in risorse esterne, permettendo così di incrociare, in fase di pubblicazione, i dati inseriti nel database di Itinera con quelli presenti altrove.   

La descrizione del modello, basato su [_Asserted Id_](Asserted_Ids_Brick.md), è disponibile su [Github](https://github.com/vedph/cadmus-general#externalidspart).  

Per stabilire un collegamento con un'entità presente in una database esterno a Itinera, compilare i campi come segue:  

* _id_:
  * _tag_: lasciare vuoto;
  * _scope_: indicare il nome della banca dati utilizzata;
  * _value_: compilare con l'URI dell'entità nella banca dati utilizzata (per VIAF ricercabile attraverso un _tool_ specifico; cfr. infra);  
* _assertion_: compilare secondo le modalità previste in [Assertion](Assertion_Brick.md);  

⚠️ Per gli Item Mauscript è possibile creare un collegamento con RDP, Mirabile, PERI, MOL, E-codices, DigiVatlib, indicate in questa forma nello _scope_.   
È possibile inoltre inserire il link ad eventuali riproduzioni digitali disponibili online: in questo caso compilare il campo _tag_ con la voce "riproduzione".  


## Save ⚠️ 

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
