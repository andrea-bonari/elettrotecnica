>[!note]
>Lo stato di una rete elettrica è dato da tutte le variabili di stato

### Soluzione di circuiti RC e RL del primo ordine
>[!note]
>Un circuito RC o RL è un circuito con una sola variabile di stato:
>![[Pasted image 20240902180853.png]]
>Supponendo che la rete elettrica contiene solo componenti adinamici, lineari, tempo-invarianti e generatori indipendenti.

Nel caso dei circuiti RC sostituisco la rete elettrica con equivalente di Norton, viceversa nel circuito RL uso l'equivalente di Thevenin.
![[Pasted image 20240902181115.png]]

Utilizziamo questi equivalenti affinché l'equivalente ammetta soluzione anche nel caso in cui l'equazione sia degenere. Risolvendo l'equivalente, esplicitando la solo la variabile di stato, otterremo delle equazioni di stato, cioè equazioni differenziali ordinarie lineari del primo ordine a coefficienti costanti. È possibile scrivere le equazioni di stato delle seguenti forme: $$\frac{\text{d}}{\text{d}t} x(t)= \lambda x+\mu u(t) $$
Dove $x(t)$ è la variabile di stato, $\lambda$ è la frequenza libera, $u(t)$ sono gli ingressi.
Conoscendo la condizione iniziale $x_{0}=x(t_{0})$ è possibile risolvere le equazioni.

>[!tip] Soluzione di ODE
>La soluzione di una ODE (Equazione Differenziale Ordinaria) di questo tipo è composta da due parti:
> ##### Soluzione dell'equazione omogenea associata
>$$\frac{\text{d}x_{OA}}{\text{d}t}=\lambda x_{OA}$$
>La sua soluzione è nella forma: $$x_{OA}(t)= ke^{\lambda(t-t_{0})}$$
>Per $\lambda<0$, $x_{OA}(t)$ decade esponenzialmente nel tempo, quindi la risposta libera si esaurisce, e quindi il circuito è stabile. Viceversa per $\lambda>0$ il circuito è instabile.
>
>Definiamo come $\tau= \frac{1}{|\lambda|}$ la costante di tempo del circuito, e da indicazioni della scala temporale su cui evolve un circuito. In generale per $t_{0}+ [5/10]\tau$ la risposta libera può considerarsi esaurita.
> ##### Soluzione dell'integrale particolare
> Questa parte consiste nel trovare una funzione che soddisfi l'equazione di stato. In base all'ingresso troviamo un integrale particolare:
>
>| $$u(t)$$                                      | $$x_{IP}(t)$$                                |
>| --------------------------------------------- | -------------------------------------------- |
>| $$\alpha e^{\beta(t-t_{0})}$$                 | $$\gamma e^{\beta(t-t_{0})}$$                |
>| $$\sum\limits_{k=0}^{n} \alpha_{k}(t-t_0)^k$$ | $$\sum\limits_{k=0}^{n} \gamma_k(t-t_0)^k$$  |
>| $$\alpha\cos(\omega t+\beta)$$                | $$\beta\sin(\omega t)+\gamma\cos(\omega t)$$ |
>
>
>---
>La soluzione complessiva dell'equazione di stato è data dalla somma $$x_{OA}(t)+X_{IP}(t)$$


