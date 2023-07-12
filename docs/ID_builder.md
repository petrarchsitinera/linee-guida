Permette di indicare l'autore del testo, secondo il modello [Asserted Id](Asserted_Ids_Brick.md).  
Per individuare [l'_eid_](identifiers.md) di un autore schedato in Itinera, controllare sempre il [repository delle persone](repository.md).  
Se l'autore è schedato come Item Person all'interno della banca dati, esso è conseguentemente provvisto di un [_eid_](identifiers.md). È possibile dunque cercare e richiamare l'_eid_ attraverso lo strumento di ricerca integrato in [Asserted Id](Asserted_Ids_Brick.md#target).  
Nel caso in cui alla persona da inserire non sia già attribuito un _eid_, il compilatore dovrà selezionare il [flag _external_](Asserted_Ids_Brick.md#altri-identificativi-itinera), procedere all'assegnazione di un nuovo _eid_ seguendo le istruzioni indicate [qui](identifiers.md) e segnalarla su [Clickup](https://clickup.com/) per permettere l'aggiornamento del [repository](repository.md).  

> Tutti gli autori dispongono, di norma, di un Item Person dedicato. In caso contrario, e dopo aver verificato sui [repository](repository.md) è opportuno creare un Item Person dedicato e richiamarne l'_eid_ nel campo _author_.   
> Se l'autore non è di interesse specifico di Itinera, è possibile evitare la creazione di un Item Person dedicato e inserire un [identificativo esterno](Asserted_Ids_Brick.md#altri-identificativi-itinera) secondo le regole definite per gli [_eid_](identifiers.md). 



Item Ms
-MatDescr > eid: regole
-Watermarks > Asserted id (Briquet)
-HandsPart > eid: regole
-HandsPart > signs > eid: regole
-DecorationPart > eid: regole
-DecorationPart > Artist > sia eid sia Asserted id
-ContentsPart > id + lookup esterno
-EditsPart > eid: regole
