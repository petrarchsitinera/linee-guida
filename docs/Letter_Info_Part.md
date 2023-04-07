# Letter Info

**Letter Info** raccoglie, in forma di testo libero, alcune informazioni relative al contenuto, all'intestazione e alla datazione dichiarata dei testi epistolari.  

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#letterinfopart).  

⚠️ Se un testo dà notizia di uno o più eventi riguardanti persone, testi o manoscritti, e se tali eventi sono compresi nel [_thesaurus_ degli eventi di Itinera](Events_Thesaurus.md), è **obbligatorio** creare uno o più eventi dedicati nella [_Events Part_](Events_Part.md) di una delle entità coinvolte. Il testo da cui si ricava l'informazione andrà **obbligatoriamente** inserito come fonte nell'[Assertion](Assertion_Brick.md) dell'evento creato.

> Esempio.   
Nella lettera _Multa expectaram_ di Francesco Nelli, si dà notizia di un incontro di alcuni amici fiorentini di Petrarca, tra cui Giovanni Boccaccio, Lapo da Castiglionchio e Francesco Bruni, che, riuniti, leggono insieme alcuni versi e lettere inviati loro da Petrarca. Dopo aver verificato sul grafo che gli eventi non siano già stati inseriti e descritti, il compilatore dell'_item_ relativo alla _Multa expectaram_ dovrà creare:  
> - un evento 'incontro' nella _Events Part_ dell'_item_ relativo ad uno dei partecipanti (p. es. Francesco Nelli), indicando gli altri partecipanti tra i _related_ (tutti gli alti, tranne Nelli). 
> - tanti eventi 'ricezione' quante sono le ricezioni testimoniate dalla _Multa expectaram_: la ricezione da parte di Nelli della proposta petrarchesca (perduta) alla _Multa expectaram_, la ricezione di _Epyst._ III 17 da parte di Boccaccio, ecc. Il compilatore può scegliere se creare gli eventi nella _Events Part_ degli _item_ relativi ai testi in questione o in quelli relativi alle persone che hanno ricevuto i testi.

Per aggiungere la parte, selezionare **_letter_** dal menu a tendina, quindi cliccare su **_add part_**.

## Subject
Permette di inserire un breve regesto del testo, chiaro e conciso. Evitare le frasi nominali e le frasi troppo lunghe. Evitare di ripetere i dati già inseriti altrove nel modello: non è necessario, per esempio, riportare il nome delle persone citate, indicate in una parte apposita.  

> Es. La lettera risponde ad un'altra perduta di Petrarca, che informava Francesco Nelli della morte di Giacomo da Carrara.

Per lettere perdute di cui si può ricostruire il contenuto a partire dalle risposte, il _subject_ è preceduto dall'indicazione della fonte tra parentesi quadre. 

⚠️ Ogni frase deve essere chiusa da punto fermo.  

La compilazione del campo è **obbligatoria**. Per le lettere perdute, è obbligatoria solo in presenza di dati sul contenuto desumibili da altre fonti. 

## Header
Permette di inserire l’intestazione della lettera, in latino, nella forma accertata dall’edizione critica o attestata nel manoscritto.

> Es. Ad eundem se tempore belli ad loca pacifica invitantem

La compilazione del campo è **obbligatoria** in presenza del dato. 

## Text date
Permette di inserire la data della lettera, in latino, nella forma accertata dall’edizione critica o attestata nel manoscritto.

> Es. Florentie penultima die Ianuarii

La compilazione del campo è **obbligatoria** in presenza di data dichiarata. 

## Save ⚠️ 
Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'_item_.
