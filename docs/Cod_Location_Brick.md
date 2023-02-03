# Codicological Location (ranges)

Il modello permette di esprimere un riferimento a determinate carte del manoscritto nei campi **range(s)** e **sample**.  
È possibile inserire riferimenti a singole carte (es. 1r), serie di carte discontinue (es. 1r 10v), intervalli di carte (es. 1r-10v), o combinazioni di tali elementi (es. 1r 4r-8v 11r 20r-30v).  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-bricks-shell/blob/master/projects/myrmidon/cadmus-cod-location/README.md)  

Per la compilazione del campo è possibile scegliere tra due modalità:
* utilizzare la numerazione di riferimento _n_ creata in [Sheet Labels Part](Sheet_Labels_Part.md);
* utilizzare le carte fisiche, rappresentate dalla colonna grigia in [Sheet Labels Part](Sheet_Labels_Part.md).  

## Numerazione di riferimento

Per utilizzare la numerazione di riferimento (colonna _n_ di [Sheet Labels Part](Sheet_Labels_Part.md)) occorre osservare la seguente sintassi:
* **numerazione di riferimento**: inserire sempre come primo elemento l'indicazione della colonna _n_, seguita da due punti (:);
 > n:
* **carta**: inserire sempre l'indicazione della carta, riportando tra apici doppi ("") l'intera etichetta presente sulla cella relativa alla carta desiderata, comprensiva di _r_/_v_.
 > n:"4r" 
 > n:"IVr" 
 > n:"13bisv" 
 > n:"[v]" (controguardia anteriore)
* **colonna**: in caso di impaginazione a più colonne, è possibile indicare la colonna con lettera alfabetica minuscola (a, b, ...);
  > n:"4r"a   
* **linea**: è possibile, se necessario, registrare la linea di testo: inserire il numero preceduto da punto (.); 
  > n:"4r"a.15  
* **parola**: è possibile, se necessario, registrare la parola: inserire la parola preceduta da chiocciola (@).  
  > n:"4r"a.15@pace  

Singole _location_ possono essere combinate secondo queste regole:
* per esprimere **intervalli di carte successive**, separare le _location_ con trattino semplice (-) senza spazi né prima né dopo; 
  > n:"1r"-n:"10v"
⚠️ Ricordarsi di premette ad ogni singola _location_ il prefisso _n:_.
* per esprimere **serie di carte discontinue**, separare le _location_ o gli intervalli con uno spazio singolo; 
  > n:"1r" n:"4r"-n:"8v" n:"11r" n:"20r"-n:"30v"
⚠️ Ricordarsi di premette ad ogni singola _location_ il prefisso _n:_.

## Riferimento alle carte fisiche
Per utilizzare il riferimento alle carte fisiche (colonna grigia di [Sheet Labels Part](Sheet_Labels_Part.md)) occorre osservare la seguente sintassi:  

* **carta**: inserire sempre il numero di carta in cifre arabiche, indicando _r_/_v_:
  > 4r
  * per le carte di guardia anteriori o posteriori riportare i valori presenti nella colonna grigia;
  > (1r)
  > (/1r)
  * per piatto o al contropiatto anteriori o posteriori riportare i valori presenti nella colonna grigia;
  > [r]
  > [/v]
* **colonna**: in caso di impaginazione a più colonne, è possibile indicare la colonna con lettera alfabetica minuscola (a, b, ...);
  > 4ra  
* **linea**: è possibile, se necessario, registrare la linea di testo: inserire il numero preceduto da punto (.); 
  > 4ra.15  
* **parola**: è possibile, se necessario, registrare la parola: inserire la parola preceduta da chiocciola (@).  
  > 4ra.15@pace  

Singole _location_ possono essere combinate secondo queste regole:
* per esprimere **intervalli di carte successive**, separare le _location_ con trattino semplice (-) senza spazi né prima né dopo;  
  > 1r-10v  
* per esprimere **serie di carte discontinue**, separare le _location_ o gli intervalli con uno spazio singolo; 
  > 1r 4r-8v 11r 20r-30v  

## CodLocation Converter
Per rendere più agevole la corrispondenza tra carte fisiche e numerazioni del manoscritto (registrate in [Sheet Labels Part](Sheet_Labels_Part.md)), è disponibile uno strumento di conversione.  

Per attivare la funzionalità, nella barra di testa, sulla destra, attivare il pulsante _toogle tools_.  
![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_off.png?raw=true)  
Cliccandolo, si illumina di rosso.   
![](https://github.com/petrarchsitinera/linee-guida/blob/e4de2f4f2dca13dcba7beae653a386470c141348/docs/assets/images/tools_on.png?raw=true)  
Contestualmente, sul lato sinistro della pagina si apre una barra laterale che dà accesso a una funzionalità denominata _Cod Location_.   
![](?raw=true)   
Nel campo _item_ cercare e selezionare l'identificativo del manoscritto in fase di descrizione.  
Nel campo _system_ selezionare il nome della numerazione interessata.  
Digitando nel campo _label_ l'etichetta assegnata a una carta, comprensiva di _r_/_v_, nel campo _location_ compare il numero della carta fisica corrispondente.  
È possibile effettuare la conversione anche in senso contrario.  

