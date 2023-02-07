# Person Works Part

**Person Work Part** permette di inserire le opere di un autore. Si inseriscono anche i testi non letterari e le opere dubbie e/o attribuite. In quest'ultimo caso, è prevista la compilazione dell'[assertion](Assertion_Brick).

⚠️ In linea generale, e salvo specifiche eccezioni, il compilatore deve inserire nella _Person work part_ di un autore soltanto i testi per i quali non sia prevista la creazione di un _item_ dedicato. 
> Lo scopo della norma è quello di evitare ridondanza nelle immissioni, stante la possibilità di collegare i testi e i rispettivi autori già negli _item text_. Ad esempio, poiché le lettere cosiddette _Disperse_ di Petrarca risultano schedate singolarmente nei rispettivi _item text_ (Disp. 1, Disp. 2, ecc.), e poiché le _Disperse_ non costituiscono un _corpus_ d'autore (cfr. _infra_), le _Disperse_ non saranno inserite nella _Person work part_ dell'_item_ relativo a Francesco Petrarca. Per verificare per quali testi è prevista la creazione di _item_ specifici, consultare i [repository dei corpora](repository.md).

⚠️ Per ogni opera o testo inserito nella _Work Part_, e qualora l'opera o il testo *non* risultino descritti in _item_ appositi, deve essere compilato un evento [_stesura_](https://github.com/petrarchsitinera/linee-guida/blob/main/docs/Events_Thesaurus.md#stesura), in cui sarà riportato l'[_eid_](identifiers.md) dell'opera indicato nella _Work Part_. Nel caso di più testi, si procede all'inserimento di un unico evento _stesura_ soltanto se i testi sono state composte in un medesimo arco cronologico. Se i testi sono stati composti in momenti diversi, si procede alla ceazione di più eventi _stesura_.   

La descrizione del modello è disponibile su [Github](https://github.com/vedph/cadmus-itinera#personworkspart).

Per aggiungere la parte, selezionare **works** dal menu a tendina, quindi cliccare su **add part**.  

##  Work
Ciascuna opera è inserita come elemento singolo (_work_) - cfr. la sezione [Creare, modificare, eliminare e salvare elementi](Editor_Brick.md).

###  Title
Inserire il titolo completo dell'opera **nella forma d'autore**. In caso di dubbio, si inserisce il titolo più usato o nella forma più comune. 

> [item Francesco Petrarca] _Triumphi_    
> [item Giovanni Boccaccio] _Decamerone_  

Nel caso di **testi poetici** sciolti, si inserisce come titolo il **primo verso**. La regola vale per tutti i testi che non costituiscano un _corpus_ d'autore, compresi quelli pubblicati in edizioni moderne di cui siano eventualmente invalsi titolo e numerazione.

> All'interno della _Person work Part_ dell'_item_ relativo a Giovanni Boccaccio, ad esempio, le _Rime_ non saranno inserite come elemento _Rime_: il compilatore procederà ad inserire singolarmente ciascun testo (un testo = un elemento), indicandone di volta in volta l'_incipit_ come _title_.
 
Nel caso di **lettere** non raccolte dall'autore, si inserisce **l'intestazione** o, in sua assenza, **le prime parole del testo**. La regola vale per tutte le lettere che non costituiscano un _corpus_ d'autore, comprese quelle pubblicate in edizioni moderne di cui siano eventualmente invalsi titolo e numerazione.

> All'interno della _Person work Part_ dell'_item_ relativo a Giovanni Boccaccio, ad esempio, le _Lettere_ non saranno inserite come elemento _Lettere_: il compilatore procederà ad inserire singolarmente ciascun testo (un testo = un elemento), indicandone di volta in volta l'intestazione o l'_incipit_ come _title_.


La compilazione del campo è obbligatoria.  

### Eid

In linea generale, le opere e i testi inseriti nella _Person Work Part_ di un autore non sono descritti in _item_ autonomi (cfr. supra).  
Tuttavia, per garantire un eventuale allargamento dei _corpora_ del progetto - che nella sua prosecuzione potrebbe arrivare a descrivere più testi di quelli inizialmente previsti - si è deciso di associare comunque ad ogni elemento inserito un _eid_.

Compilare il campo attribuendo un _eid_ al testo secondo le norme indicate [qui](identifiers.md#attribuire-un-eid).  


###  Assertion  
Se il testo o l'opera da inserire è **dubbia** o **attribuita**, spuntare e compilare l'[assertion](Assertion_Brick).

L'_assertion_ si riferisce sempre ad una singola attribuzione: descrive cioè l'attribuzione di un singolo testo dubbio o presunto ad un autore.  
Nel caso di più testi dubbi o attribuiti, l'_assertion_ va ripetuta: si inseriscono tante _assertion_ quanti sono i testi dubbi o attribuiti.  

Il campo _note_ dell'_assertion_ può essere compilato quando il rimando alle voci bibliografiche e alle fonti non sia sufficiente o nei casi che, risultando complessi, richiedano un supplemento di spiegazione.

## Save ⚠️ 

Per ogni elemento _work_ inserito è necessario salvare cliccando sul tasto di spunta blu.

Cliccare sul tasto **_save_** per salvare la parte.  
La parte è correttamente salvata quando in fondo allo schermo compare la notifica **_Part saved_**.  
Completato il salvataggio, cliccare sul tasto **_Close_** per tornare alla schermata di riepilogo dell'item.
