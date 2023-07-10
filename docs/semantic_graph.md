# Grafo semantico  

Il grafo semantico è costruito automaticamente a partire dai dati inseriti all'interno degli _item_.  

Per il compilatore il grafo semantico serve in primo luogo a verificare l'esistenza di eventi e relazioni tra due o più entità.  
Dal momento che in alcuni casi uno stesso evento può essere inserito a partire da diversi punti di accesso, è fondamentale verificare che l'evento non sia già stato inserito da un altro compilatore.

⚠️ Il grafo va usato per verificare che un evento da inserire che coinvolga due o più entità non sia già stato inserito, o che, inserito, riporti dati corretti. È dunque uno strumento fondamentale per evitare ridondanze ed errori. La sua consultazione è **obbligatoria** prima dell'inserimento di un qualsiasi evento.  

## Ricerca sul grafo: esempio
Prendiamo il caso della Fam. XXII 4, datata 20 aprile 1363.
Non sappiamo quando Petrarca la invii concretamente al destinatario, Barbato da Sulmona, ma sappiamo dalla risposta di quest'ultimo, _In die nativitatis_, che Barbato la ricevette il 25 dicembre 1363 e che dunque, prima di quella data, Petrarca la inviò al destinatario.  
Lo schedatore di _In die nativitatis_, di fronte all'accusa di ricezione di Fam. XXII 4, dovrà verificare che esista all'interno della banca dati un evento _invio_ che colleghi Petrarca in qualità di mittente, Fam. XXII 4 in qualità di oggetto inviato, Barbato in qualità di destinatario.  
Anziché verificare all'interno della _Events Part_ di ogni singolo _item_, il compilatore può ricorrrere alla _query_ del grafo, dove gli eventi e le entità ad essi collegate risultano appunto proiettati.

Per accedere al grafo selezionare _Graph_ dal menu orizzontale in alto.  
![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/b71a29a3-90ed-4f3f-8d6f-2d293cb10dde)

Si accederà così ad una schermata, divisa in tre sezioni navigabili, dedicate rispettivamente a:
* nodi: la lista delle entità mappate a partire dai dati degli _item_;
* triple: la lista delle relazioni tra entità create a partire da eventi e altre parti degli _item_;
* walker: un sistema di visualizzazione di nodi e triple.  

![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/59819308-52cb-47d5-9123-ebc3b33b4c39)

A sinistra della sezione dedicata ai nodi è disponibile un'interfaccia di ricerca. Digitando le prime lettere dell'_eid_ dell'entità di interesse nel campo _label_, è possibile filtrare i risultati compatibili per individuare rapidamente l'_item_ di interesse.

![image](https://github.com/petrarchsitinera/linee-guida/assets/123007762/66c399fe-e082-4fcc-9b10-4ddb45c0963c)

Nella colonna dedicata all'_item_ di interesse cliccare il primo comando a sinistra "walk node".  

🚧 IMMAGINE 🚧

Cliccando _walk node_ si accede alla sezione del walker, che mostra il nodo in questione e le relazioni che lo coinvolgono.  
Il grafo è navigabile cliccando sui riquadri colorati, che riportano al loro interno il numero di entità ulteriormente collegate.  
Per individuare la relazione di interesse tra quelle registrate sul grafo, il compilatore deve cliccare i riquadri colorati.   

**Se l'evento risulta già inserito**, questo comparirà tra i nodi collegati alla entità. Selezionando il riquadro relativo e cliccando (🚧 + _shift_) sul tasto di spunta blu nella sezione a sinistra dello schermo ("pick selected node") è possibile accedere alla _Events Part_ dell'_item_ in cui l'evento è stato inserito. In questo caso il compilatore **deve** verificare la correttezza dei dati inseriti.  
⚠️ La revisione di dati già inseriti da un altro compilatore, va segnalata al responsabile della scheda e ai revisori, che provvederanno ad aggiornarla e correggerla ove necessaria.  

**Se l'evento non risulta già inserito**, il compilatore può procedere alla creazione dell'evento relativo.
