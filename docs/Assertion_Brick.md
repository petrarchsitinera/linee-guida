# Assertion 

**Assertion** permette di qualificare i dati inseriti con un indice numerico di affidabilità e/o di associare ad essi fonti e voci bibliografiche.  

Ogni _Assertion_ si riferisce ad un singolo dato inserito.  

![](https://github.com/petrarchsitinera/linee-guida/blob/9a3544c46e6ea09d6092d436a630821b00eb5fef/docs/assets/images/assertion.png?raw=true)

Si compila un'_Assertion_ per indicare l'affidabilità di un dato e/o inserire voci bibliografiche, senza che le due possibilità si escludano. È cioè possibile inserire un'_Assertion_ perché si ha bisogno di aggiungere un rank, una voce bibliografica, o entrambe le cose contemporaneamente.

## Tag
Lasciare il campo vuoto, se non altrimenti indicato nelle linee guida della _part_ relativa.

## Rank 
Il rank è un indice numerico di affidabilità associato al dato inserito. Va da un massimo (1) ad un minimo (3) di certezza:
* il rank è pari a **1** quando il dato inserito è certo.  
* il rank è pari a **2** quando il dato inserito non è certo, ma è il più sicuro, probabile o verosimile tra quelli a disposizione.  
* il rank è pari a **3** quando il dato inserito non è certo ed è il meno sicuro, probabile o verosimile tra quelli a disposizione, oppure quando il dato è sicuramente erroneo.

In caso di più ipotesi equivalenti, è possibile inserire più _Assertions_ con rank=2 o rank=3.

**Se non compilato**, il rank è sempre uguale a 0 (ed equiparato al valore di 1: dato certo).

##  Note  
Il campo _note_ permette di inserire una breve stringa di testo esplicativo. Compilare il campo solo se strettamente necessario.  


## Assertion references  
Permette di inserire fonti e voci bibliografiche a sostegno del dato inserito, secondo il modello [DocReference](Docref_Brick.md).  
È possibile aggiungere più _references_, una per fonte o voce bibliografica.  
Per aggiungere una _reference_ aprire la finestra a scomparsa cliccando su _assertion references_ e premere il comando _+ add reference_.  

![](https://github.com/petrarchsitinera/linee-guida/blob/bb413d602f3fb56c819fb52e99645bfc0b6104d6/docs/assets/images/add_reference.png?raw=true)
