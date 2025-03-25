>[!note]
>Il principio di sovrapposizione degli effetti afferma che l'intensità di corrente e la tensione associata a ciascun lato del grafo corrispondente al circuito sono pari, rispettivamente, alla somma delle intensità di corrente e delle tensioni che ciascuno dei generatori indipendenti produrrebbe se agisse da solo con tutti gli altri generatori spenti:
>$$\begin{align*}
V&= \sum\limits_{k=1}^{N}\alpha_{k}E_{k}+\sum\limits_{j=1}^{M}R_{j}A_{j}&\qquad[a_{k}]=\text{1},[R_{j}]=\ohm\\
i&= \sum\limits_{k=1}^{N}g_{k} E_{k}+\sum\limits_{j=1}^{M}\beta_{j}A_{j}&\qquad[\beta_{k}]=\text{1},[g_{j}]=\text{S}
\end{align*}$$
>![[Pasted image 20240829141112.png|center]]

>[!example] Dimostrazione
>Dall'equazione dei componenti si ha che: $$\overrightarrow{i}= N^{-1}(\overrightarrow{z}-M\overrightarrow{v})$$
>Usando l'equazione di Tableau $\overrightarrow{v}=A^{T}\overrightarrow{u}$: $$\overrightarrow{i}=N^{-1}(\overrightarrow{z}-MA^{T}\overrightarrow{u})$$
>Usando l'altra equazione di Tableau $A\overrightarrow{i}=0$: $$\begin{align*}
>&AN^{-1}(\overrightarrow{z}-MA^{T}\space\overrightarrow{u})=\overrightarrow{0}\\
>\Longrightarrow\space&\underbrace{AN^{-1}}_{b}\overrightarrow{z}=\underbrace{AN^{-1}MA^{T}}_{a}\space\overrightarrow{u}\\
>\Longrightarrow\space&a\overrightarrow{u}=b\overrightarrow{z}\\
>\Longrightarrow\space&\overrightarrow{u}= \underbrace{a^{-1}b}_{c}\overrightarrow{z} 
>\end{align*}$$
>Dove $\overrightarrow{u}$ è una combinazione lineare tramite la matrice $c$ degli ingressi contenuti nel vettore dei termini noti $\overrightarrow{z}$. Per ricavare la corrente: $$\begin{align*}
>&\overrightarrow{v}=A^{T}\overrightarrow{u}=\underbrace{A^{T}c}_{d}\overrightarrow{z}\\
>\Longrightarrow\space&\overrightarrow{i}=N^{-1}(\overrightarrow{z}-MA^{T}c\overrightarrow{z})=\underbrace{N^{-1}(\mathbb{1}-MA^{T}c)}_{f}\overrightarrow{z}\\
>\Longrightarrow\space&\overrightarrow{i}= f\overrightarrow{z}
\end{align*}$$
