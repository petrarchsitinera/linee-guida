# Codicological Location (ranges)

Il campo permette di esprimere un riferimento a determinate carte del manoscritto.  
È possibile inserire riferimenti a singole carte (es. 1r), serie di carte discontinue (es. 1r 10v), intervalli di carte (es. 1r-10v), o combinazioni di tali elementi (es. 1r 4r-8v 11r 20r-30v).  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-bricks-shell/blob/master/projects/myrmidon/cadmus-cod-location/README.md)  

## Sintassi
Ogni singola _location_ può contenere i seguenti elementi:
* carta: unico elemento obbligatorio, da indicare secondo queste possibilità:
  * se la carta è numerata con cifre arabiche, riportarle;
  > es. **4**
  * se la carta è numerata con un qualsiasi valore diverso da cifra arabica (numeri romani, segni alfabetici, etc.), riportare l'indicazione tra apici doppi (" ");
  > es. **"IV"**
  * se la carta è numerata con una cifra arabica seguita da valore diverso, riportare la cifra arabica seguita dall'altro valore tra apici doppi (" ");
  > es. **3"bis"**
* facciata: in caso di cartulazione, è possibile indicare il recto della carta con _r_, il verso con _v_;
  > es. 4**r**  
  > es. "IV"**v**  
  > es. 3"bis"**r**  
* colonna: in caso di impaginazione a più colonne, è possibile indicare la colonna con lettera alfabetica minuscola (a, b, ...);
  > es. 4r**a**  
* linea: è possibile, se necessario, registrare la linea di testo: inserire il numero preceduto da punto (.); 
  > es. 4ra.**15**  
* parola: è possibile, se necessario, registrare la parola: inserire la parola preceduta da chiocciola (@).  
  > es. 4ra.15@**pace**  

Singole _location_ possono essere combinate secondo queste regole:
* per esprimere intervalli di carte successive, separare le _location_ con trattino semplice (-) senza spazi né prima né dopo;  
  > es. 1r-10v
  > es. 1ra-"XII"vb
* per esprimere serie di carte discontinue, separare le _location_ o gli intervalli con uno spazio singolo; 
  > es. 1r 4r-8v 11r 20r-30v





## Note importanti
* richiamo a numerazioni con system
* numerazione n
* reminder etichetta guardie e cover
