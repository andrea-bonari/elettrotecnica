>[!note]
>Un circuito RL o RC del primo ordine comprende un solo condensatore/induttore collegato ad una rete elettrica formata da soli componenti adinamici, lineari, tempo-invarianti e al più generatori indipendenti.

>[!abstract] Processo di risoluzione
>Nel caso del condensatore troviamo l'equivalente di Norton alla rete lineare, e ricaviamo tramite KCL l'equazione di stato del circuito: $$\frac{\text{d}V_{C}}{\text{d}t}=- \frac{1}{RC}V_{C}- \frac{1}{C}a(t)$$
>Nel caso dell'induttore troviamo l'equivalente di Thevenin alla rete lineare, e ricaviamo tramite KVL-II l'equazione di stato del circuito: $$\frac{\text{d}i_{L}}{\text{d}t}=- \frac{R}{L}i_{L}+ \frac{1}{L}e(t)$$

### Equazioni di stato
>[!note]
>Per i circuiti del primo ordine, un'equazione di stato è un equazione differenziale ordinaria del primo ordine a coefficienti costanti. La risolviamo tramite il generico problema di Cauchy: $$\begin{cases}
>\frac{\text{d}x}{\text{d}t}=-\lambda x+ u(t) \\
>x(t_{0})=x_{0}
>\end{cases}$$
>Dove $x$ è la variabile di stato, $\lambda$ è la frequenza libera ($[\lambda]=\text{Hz}$) e $u(t)$ sono gli ingressi.
>La soluzione di questa equazione sarà: $$x(t)= \left(x_{0}+ \frac{u(t)}{\lambda}\right)e^{\lambda(t-t_{0})}- \frac{u(t)}{\lambda}$$

>[!example] Dimostrazione
>La soluzione di un Problema di Cauchy di un EDO del primo ordine è una soluzione particolare $\overline{x}: J\subseteq\mathbb{R}\to\mathbb{R}$ dell'integrale generale del EDO che soddisfa le condizioni del sistema.
>
>Per trovare l'integrale generale della EDO dobbiamo trovare la soluzione dell'omogenea associata, e la soluzione dell'integrale particolare. Cerchiamo la soluzione dell'omogenea associata: $$\frac{\text{d}}{\text{d}t} x_{\text{OA}}(t)=\lambda x_{\text{OA}}$$
>Si ha che la sua soluzione è: $$x_{\text{OA}}(t)=ke^{\lambda(t-t_{0})}$$
>Affinché il circuito sia stabile ($\lambda<0$) è necessario che la risposta libera si esaurisca nel tempo $\tau= \frac{1}{|\lambda|}\qquad [\tau]=\text{S}$. Si ha quindi che per $t>t_{0}+ (5/10)t$ allora $x_{\text{OA}}(t)\simeq0$
>
>Troviamo adesso la soluzione dell'integrale particolare, che è: $$\gamma_{0}=- \frac{u}{\lambda}$$
>L'integrale generale è dato dalla somma della soluzione dell'omogenea associata all'integrale particolare: $$x(t)=ke^{\lambda(t-t_{0})}- \frac{u}{\lambda}$$
>Imponendo le condizioni iniziali $x(t_{0})=x_{0}$ otteniamo: $$k= x_{0}+ \frac{u}{\lambda}$$
>E di conseguenza: $$x(t)= \left(x_{0}+ \frac{u(t)}{\lambda}\right)e^{\lambda(t-t_{0})}- \frac{u(t)}{\lambda}$$

