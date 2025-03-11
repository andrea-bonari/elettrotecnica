>[!note]
>Il teorema di esistenza e unicità della soluzione afferma che la soluzione di un circuito esiste ed è unica se e solo se: $$\det(T(t))\neq0\qquad \forall t$$

>[!example] Dimostrazione
>Si consideri una rete elettrica di $l$ lati e $n$ nodi, si hanno quindi $2l+n-1$ incognite nel circuito. E si considerino le equazioni di Tableau: $$\begin{cases}
>A\overrightarrow{i}=\overrightarrow{0}&n-1 \\
>A^{T}\space\overrightarrow{u}-\overrightarrow{V}=\overrightarrow{0}&l
>\end{cases}$$
>
>Scriviamo le $l$ equazioni costitutive dei componenti $j$ nella seguente forma: $$M_{j}\overrightarrow{V}_{j}+N_{j}\overrightarrow{i}_{j}=\overrightarrow{z}_{j}$$
>Dove $\overrightarrow{v}_{j}$ sono le tensioni descrittive del $j$-esimo componente, $\overrightarrow{i}_{j}$ sono le correnti descrittive, e $\overrightarrow{z}_{j}$ sono i termini noti.
>Scriviamo quindi tutte le $l$ equazioni costitutive accorpando tutte le sottomatrici $M_{j}, N_{j}$ e i vettori $z_{j}$: $$M(t)\overrightarrow{V}+N(t)\overrightarrow{i}=\overrightarrow{z}(t)$$
>Aggiungiamo questa equazione alle equazioni di Tableau: $$\begin{cases}
>A\overrightarrow{i}=\overrightarrow{0}&n-1 \\
>A^{T}\space\overrightarrow{u}-\overrightarrow{V}=\overrightarrow{0}&l \\
>M(t)\overrightarrow{V}+N(t)\overrightarrow{i}=\overrightarrow{z}&l
>\end{cases}$$
>Raccogliamo le incognite nel vettore $\overrightarrow{w}=(\overrightarrow{u}\space^{T}, \overrightarrow{V}\space^{T}, \overrightarrow{i}\space^{T})^{T}$: $$\underbrace{\begin{pmatrix}\mathbb{0}&\mathbb{0}&A\\-A^{T}&\mathbb{1}&\mathbb{0}\\\mathbb{0}&M&N\end{pmatrix}}_{T(t)}\underbrace{\begin{pmatrix}\overrightarrow{u}\\\overrightarrow{V}\\\overrightarrow{i}\end{pmatrix}}_{\overrightarrow{w}}=\underbrace{\begin{pmatrix}\overrightarrow{0}\\\overrightarrow{0}\\\overrightarrow{z}\end{pmatrix}}_{\overrightarrow{y}(t)}$$
>Dove $\mathbb{0}$ è una matrice di zeri, e $\mathbb{1}$ è la matrice identità di opportune dimensioni. Questo è il sistema risolutivo del circuito. La cui soluzione è: $$\overrightarrow{w}= T^{-1}(t)\cdot\overrightarrow{y}(t)$$
>
