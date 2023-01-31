# Assertion 

**Assertion** permette di qualificare i dati inseriti con un indice numerico di affidabilità e/o di associare ad essi fonti e voci bibliografiche.  

Ogni _Assertion_ si riferisce ad un singolo dato inserito.

Si compila un'_Assertion_ per indicare l'affidabilità di un dato e/o inserire voci bibliografiche, senza che le due possibilità si escludano. È cioè possibile inserire un'_Assertion_ per aggiungere soltanto un rank o soltanto una voce bibliografica, ma è possibile ricorrere alla parte per inserirli entrambi.

## Tag
Lasciare il campo vuoto, se non altrimenti indicato.

## Rank 
Il rank è un indice numerico di affidabilità associato al dato inserito. Va da un massimo (1) ad un minimo (3) di certezza:
* il rank è pari a **1** quando il dato inserito è certo.  
* il rank è pari a **2** quando il dato inserito non è certo, ma è il più sicuro, probabile o verosimile tra quelli a disposizione.  
* il rank è pari a **3** quando il dato inserito non è certo ed è il meno sicuro, probabile o verosimile tra quelli a disposizione.

In caso di più ipotesi equivalenti, è possibile inserire più _Assertions_ con rank=2 o rank=3.

**Se non compilato**, il rank è sempre uguale a 0 (ed equiparato al valore di 1: dato certo).

##  Note  
Il campo _note_ permette di inserire una breve stringa di testo esplicativo. Compilare il campo solo se strettamente necessario.  


## Assertion references  
Permette di inserire fonti e voci bibliografiche a sostegno del dato inserito.  
È possibile aggiungere più _References_, una per fonte o voce bibliografica.
> 🚧 Immagine

### Type
Indica la tipologia di fonte addotta. Selezionare un valore tra:  
* ---: quando la fonte del dato non è identificabile con nessuna delle opzioni seguenti;
* testo: quando la fonte del dato è un testo letterario (lettere, testi poetici, opere, ecc.);
* bibliografia: quando la fonte del dato è una voce biblografica;
* manoscritto: quando la fonte del dato è un manoscritto;
* documento arch.: quando la fonte del dato è un documento d'archivio.

### Tag
Lasciare vuoto il campo.

### Citation
Permette di indicare il titolo o il riferimento sintetico alla fonte.  
⚠️ Se la fonte è registrata nel [database bibliografico di Itinera](External_Bibliography_Part.md) è possibile riferirsi ad essa attraverso l'utilizzo della _key_ ad esso attribuita nel database.  
⚠️ Di norma, ogni fonte pertinente alle schede di Itinera deve essere registrata nel database. Per ogni _item_, le fonti pertinenti saranno elencate nella relativa [Bibliography Part](External_Bibliography_Part.md); ove sia necessario fornire un più alto grado di dettaglio o citarle a supporto di singoli dati, esse saranno richiamate sinteticamente nelle _Assertions_ relative.  

### Note
Il campo _note_ permette di inserire una breve stringa di testo esplicativo. Compilare il campo solo se strettamente necessario. 
