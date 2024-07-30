# Asserted Chronotopes Brick 

**Asserted Chronotopes** permette l'inserimento dei dati relativi a date e luoghi, con relative fonti.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-general#chronotopespart).  

Per aggiungere un cronotopo cliccare su **add chronotope**.  
La parte è ripetibile per ogni tipologia di data e luogo da inserire e per ogni ipotesi, qualora ve ne siano più di una.  
È possibile modificare, spostare, eliminare i singoli _chronotopes_ attraverso un [editor](Editor_Brick.md).  

## Place
Permette di inserire le informazioni relative al luogo.  

* _tag_: può ospitare un'etichetta, variabile a seconda dell'item.
* _place_: permette di indicare il luogo.  
* _place assertion_: permette di indicare l'attendibilità e le fonti della data topica, secondo il modello [Assertion](Assertion_Brick.md).

Il campo _place_ deve essere compilato con un unico valore, corrispondente all'indicazione geografica più precisa tra città/regione/area/stato.  
Solo nel caso in cui sia possibile fornire un'indicazione topografica più precisa rispetto alla città (ad es. un edificio, una via, un quartiere, etc.), si indica il nome della città seguito da tale indicazione, separate da virgola.

> place= "Venezia"  
> place= "Lazio"  
> place= "Italia meridionale"  
> place= "Firenze, carcere delle Stinche"  

⚠️ I nomi di città o località vanno espressi di regola in italiano (es. Avignone). Qualora non esista o non sia in uso una forma italiana della città o della località da inserire, si ricorre alla lingua della medesima città o località (es. Clermont-Ferrand).   

## Date
Permette di inserire le informazioni relative alla data. Per inserire una datazione occorre spuntare la casella **has date**.

* _tag_: può ospitare un'etichetta, variabile a seconda dell'item e della parte in cui viene inserito il _Chronotope_.
* _datation_: permette di indicare la data.
* _date assertion_: permette di indicare l'attendibilità e le fonti della data, secondo il modello [Assertion](Assertion_Brick.md).

### _datation_
Permette di inserire date complete di anno-mese-giorno, date con solo anno e mese, date con solo anno, date al secolo, intervalli da-a, date ante quem e post quem.
È possibile inserire la data attraverso il visual editor che si apre cliccando sulla freccia blu a destra del campo.
* _value_: permette di inserire in forma numerica l'anno o il secolo (sempre in cifre arabiche, spuntando il flag _century_).
* _month_: permette di inserire in forma numerica il mese.
* _day_: permette di inserire in forma numerica il giorno.
* _century_: il flag trasforma il _value_ inserito in una datazione al secolo.
* _span_: il flag permette di indicare se la datazione corrisponde a un intervallo approssimativo che include l'anno espresso in _value_ e il successivo.
* _about_: il flag permette di indicare se si stratta di una datazione approssimativa.
* _dubious_: il flag permette di indicare se si stratta di una datazione dubbia.
* _hint_: permette di aggiungere una breve nota a giustificazione del valore inserito.
* _A-B_: permette di inserire un intervallo. Cliccandolo si apre un secondo elemento di datazione in cui sono ripetuti tutti i campi. Per inserire un termine ante quem compilare la data B e inserire 0 come value in A. Per inserire un termine post quem compilare la data A e inserire 0 come value in B. 
se si stratta di una datazione approssimativa (flag about), dubbia (flag dubious), o di una datazione al secolo (flag century). 

I flag non solo esclusivi: è possibile sceglierne più di uno. L’inserimento di *value* è obbligatorio: se non è conosciuto, inserire il secolo di riferimento (per esempio XIV sec per la datazione di una lettera di Petrarca) o un intervallo di secoli.

Dopo aver inserito una datazione attraverso il visual editor **è necessario salvare** cliccando sul **bottone di spunta blu** nel box dell'editor.


***
Per i manoscritti:  
⚠️ In tutti i casi in cui sia prassi indicare i dati cronologici con formulazioni di massima tipo "moderna", "recente", è opportuno indicare l'intervallo cronologico facendo riferimento alla seguente tavola di corrispondenza:
* coeva: il secolo di datazione dell'oggetto;  
* antica: entro il sec. XV;  
* moderna: entro il sec. XIX;   
* recente: secc. XX-XXI;
* Altri casi: esempi:
  * sec. XV primo quarto: ca. 1401 - ca. 1425 (spuntare il flag _about_);  
  * sec. XV metà: ca. 1450 (spuntare il flag _about_);  
  * sec. XV ex. - sec. XVI in.: ca. 1490 - ca. 1510 (spuntare il flag _about_).

