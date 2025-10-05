---
title: Meta è bello
output:
  prettydoc::html_pretty:
    theme: cayman
    highlight: github
---

## Introduzione

Nel mondo esistono molti problemi strani, alcuni anche pericolosi, altri solo interessanti. Per molti dei problemi della vita ci è stata data una soluzione, vuoi dai nostri genitori o dalla scuola o da un collega. Altri invece li incontriamo da soli senza averne mai sentito parlare.

Voi avete mai pensato al problema dei meta?

## Il Problema

> "Se avessi a disposizione otto ore per abbattere un albero, ne passerei sei ad affilare l'ascia."
>
> Abramo Lincoln

Grazie Abramo, ma quante ore passeresti a scegliere la cote?

Il problema è questo.

Al corso base di gestione di processi di qualsiasi Università del mondo vi viene insegnato che per gestiere un processo è necessario progettarlo. Serve a varie cose: per capire cosa potrebbe andare storto, per fare delle stime su costi e tempi o semplicemente per farsi un'idea un pò più chiara di cosa si vuole fare. Ci interessa poco comunque.

Ora immeginate questo scenario in cui:  
**dobbiamo progettare [un prodotto]** *(progettazione - $p_1$)*

Progettare un prodotto è sicuramente un processo e, se è un processo, allora dobbiamo progettarlo, ci hanno insegnato questo e ci torna il senso della cosa. Qundi:  
**dobbiamo progettare [un processo di progettazione di [un prodotto]]** *(meta-progettazione - $p_2$)*  

Che è a sua volta un processo, da cui consegue che:  
**dobbiamo progettare [un processo di progettazione di [un processo di progettazione di [un prodotto]]]** *(meta-meta progettazione -  $p_3$)*  

E così via.

Il problema nasce dalla natura autoreferenziale della progettazione che può avere tra i suoi possibili output, la progettazione stessa, diventando, così, un sistema autologico, ricorsivo, infinito ecc.

Il problema è interessante e ha vari collegamenti con la matematica frattale. Io non ne so nulla, però mi affascina maledettamente. E' una di quelle cose che ci trigghera visceralmente per trovare una soluzione.

La faccenda ha, anche, risvolti terribilmente seri. Ogni volta che ci chiediamo in modo formale come svolgere un'attività dobbiamo stimare un certa quota di tempo per progettare quello che stiamo per fare e quindi anche per la progettazione della progettazione.

Ma quanto tempo?  
Ha senso chiederselo?  
E quando, invece, ha senso fermarsi e fare la prima cosa che ci passa per la testa?  

## Soluzione (wip)

### Convergenza della serie

Facciamo 3 ipotesi:

-   in un processo di durata $t$, composto da attività di progettazione ed esecuzione, è possibile stimare empiricamente, con dati di progetti reali, la percentuale ottimale di tempo di progettazione $p$ come $$p = 1 - e$$ in cui $e$ è la percentuale di tempo utilizzata in attività di esecuzione;
-   per un qualsiasi processo, la percentuale di tempo di progettazione ottimale $p$ è invariante sui diversi livelli meta (progettazione, meta-progettazione, ecc.);
-   per un qualsiasi processo le attività di esecuzione sono sempre successive a quelle di progettazione;

Date queste ipotesi sappiamo, quindi, che un qualsiasi processo è composto da:

-   $p$: percentaule del tempo di progettazione
-   $e$: percentuale del tempo di esecuzione

Questo vale per il processo progettazione $p_1$, ma anche per il processo di meta-progettazione $p_2$ e così via.

Il tempo di progettazione, per un progetto con un budget di tempo $t$, ad un qualsiasi livello meta $i$ è, quindi, uguale a : $$ P_i=p^it$$

Questo può sembrare di poca utilità pratica, ma ci permette in qualsiasi momento di **esecuzione** di un processo,di sapere in quale livello-meta dovremmo trovarci.

Supponiamo di avere un progetto di durata $10 h$ e che per questo tipo di progetti $p = 0.2$. Questo significa che dovremmo impiegare:

-   circa $2\ h$ in progettazione, di cui:

    -   circa $24\ m$ in meta-progettazione, di cui:

        -   circa $5\ m$ in meta-meta-progettazione

Per le persone come me che si perdono troppo spesso in filosofeggiamenti sulle meta-cause delle meta-domande questo tipo di approccio è estremamnte utile.

C'è solo un problema.

## Ritorno al problema (Parte I)

Il problema di questa soluzione è che la seconda ipotesi è terribile falsa.

Per esperienza, il valore ottimale del tempo di progettazione non si mantiene costante sui diversi livelli meta. Ad esempio il tempo di meta-progettazione ottimale, in alcuni contesti, è decisamente superiore a $1/p^2$.  

Ma anche se si mantenesse sempre costante avremmo comunque un problema.  

Un'enorme quantità di asset generati dalle attività di meta e meta-meta progettazione è poi riutilizzabilie cross processo e, di fatto, viene riutilizzata. Non è quindi possibile dare una stima, anche approssimata, della percentuale di tempo impiegato in attività di meta-progettazione perchè, per lo più, non sono svolte sul processo in analisi e nemmeno dallo stesso soggetto che svolge il processo.  

Sintetizzando, dato che i valori di performance che misuriamo sui processi attuali beneficiano di sforzi di meta-progettazione passata, non ci da nessuna indicazione su quanto tempo abbia senso investire in progettazione e meta-progettazione in attività nuove.  

Il problema è che i processi non sono indipendenti, e i meta-processi lo sono ancora meno.  
Per fortuna (o sfortuna) nessuno di noi parte da un foglio davvero bianco.  

Come dicevo un bel problema, interessante però.


