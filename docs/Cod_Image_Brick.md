🚧 

images (CodImage[]):
id* (string)
type* (string) T:cod-image-types
sourceId (string)
label (string)
copyright (string)


[Daniele] “Source ID e’ l’identificativo della fonte; non necessariamente e’ un link, [p.es](http://p.es/). potrebbe essere un ID di un database di immagini da cui avete preso una singola immagine, o per assurdo il nome di un libro da cui avete scannerizzato qualcosa, etc; insomma e’ la fonte. Invece image ID e’ una cosa arbitraria che connette quell’entita’ a una serie di immagini. se ad es l’immagine ha ID pippo, e abbiamo dei file chiamati pippo01.jpg, pippo02.jpg, pippo03.jpg etc avremo un modo automatico di linkare quell’immagine a N file di immagine o anche NON a file ma a servizi ([p.es](http://p.es/). IIIF) costruendo in tal caso un URL a partire dall’ID”. 

‘type’ è per dire da che tipo di supporto/fonte (es. articolo) si prende l’immagine; obbligatorio ma no thesaurus.

L’intero ms. ha una parte che permette il collegamento con la riproduzione digitale. In singole parti dove vogliamo inserire un collegamento con riproduzione digitale (es. Hands e Decoration) usiamo il modello ‘images’. La fonte dell’immagine potrebbe essere la stessa della riproduzione integrale, ma ripetiamo i dati perché le parti non comunicano tra loro; inoltre, potremmo riferirci a fonti diverse, ad es. un immagine tratta da un libro di Petrucci.


-La segnatura del manoscritto è la chiave del collegamento tra ref. bibliografico ed eventuale item manoscritto relativo.

