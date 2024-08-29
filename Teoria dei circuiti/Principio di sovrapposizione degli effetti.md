>[!note]
>L'intensità di corrente e la tensione associata a ciascun lato del grafo corrispondente al circuito sono pari, rispettivamente, alla somma delle intensità di corrente e delle tensioni che ciascuno dei generatori indipendenti produrrebbe se agisse da solo con tutti gli altri generatori spenti.
>![[Pasted image 20240829141112.png]]
>Con $N$ generatori indipendenti di corrente e $M$ generatori indipendenti di tensione: $$V=\sum\limits^{N}_{j=1}r_{j}A_{j}+\sum\limits^{M}_{k=1}\alpha_{k}E_{k}$$
>$$i=\sum\limits_{j=1}^{N}\beta_{j}A_{j}+\sum\limits_{k=1}^{M}g_{k}E_{k}$$

>[!example] Dimostrazione
>Dall'equazione delle $l$ equazioni costitutive: $$M\overrightarrow{v}+N\overrightarrow{i}=\overrightarrow{z}$$
>Esplicito le correnti: $$\overrightarrow{i}=N^{-1}\left(\overrightarrow{z}-M\overrightarrow{v}\right)$$
>Sfruttando le equazioni di Tableau:
>$$\begin{align*}
\overrightarrow{i}&= N^{-1}\left(\overrightarrow{z}-M\overrightarrow{v}\right)\\
\iff \overrightarrow{i}&= N^{-1}\left(\overrightarrow{z}-MA^{T}\space\overrightarrow{u}\right)\\
\iff A\overrightarrow{i}&= A^{N-1}\left(\overrightarrow{z}-MA^{T}\space\overrightarrow{u}\right)=\overrightarrow{0}\\
\iff AN^{-1}\space\overrightarrow{z}&= AN^{-1}MA^{T}\space\overrightarrow{u} \\
\iff a\overrightarrow{u}&= b\overrightarrow{z}\iff \overrightarrow{u}=a^{-1}b\overrightarrow{z}=c\overrightarrow{z}
\end{align*}$$
>$\overrightarrow{u}$ è una combinazione lineare degli ingressi (contenuti nel vettore $\overrightarrow{z}$) tramite la matrice $c$. Quindi: $$\overrightarrow{v}=A^{T}\space\overrightarrow{u}=A^{T}c\overrightarrow{z}=d\overrightarrow{z}$$$$\overrightarrow{i}=Z^{-1}\left(\overrightarrow{z}-MA^{T}\space\overrightarrow{u}\right)=N^{-1}\left(\mathbb{1}-MA^{T}c\right)\overrightarrow{z}=f\overrightarrow{z}$$
>Quindi: 
>$$i_{k}=\sum\limits^{l}_{j=1}f_{kj}z_{j}$$



