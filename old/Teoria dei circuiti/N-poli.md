### Basi di definizione
>[!note]
>Consideriamo un generico $n$-poli. Esso si dice:
>- Definito su base corrente se è possibile assegnare le $n-1$ correnti e ricavare univocamente $n-1$ tensioni. Avrà quindi equazioni costitutive: $$\overrightarrow{v}=f(\overrightarrow{i})$$
>- Definito su base tensione se è possibile assegnare le $n-1$ tensioni e ricavare univocamente $n-1$ correnti. Avrà quindi equazioni costitutive: $$\overrightarrow{i}=g(\overrightarrow{v})$$
>- Definito su base mista se è possibile assegnare un sottoinsieme di correnti e sottoinsieme di tensioni e ricavare le restanti variabili descrittive. Avrà quindi equazioni costitutive: $$\overrightarrow{y}=h(\overrightarrow{x})$$

### Teorema di Tellegen
>[!note]
>Supponiamo di:
>- avere un circuito il cui grafo è connesso e contiene $n$ nodi e $l$ lati
>- usare la convenzione normale per tutti i lati del grafo.
>
>Definisco tensioni e correnti compatibili (rispettano leggi di Kirchhoff)con il grafo con i seguenti vettori: $$\overrightarrow{i}=\begin{pmatrix}i_{1}\\i_{2}\\\vdots\\i_{n}\end{pmatrix}\qquad \overrightarrow{v}=\begin{pmatrix}v_{1}\\v_{2}\\\vdots\\v_{n}\end{pmatrix}$$Il teorema di Tellegen afferma che: $$\overrightarrow{v}\space^{T}\cdot \overrightarrow{i}=\overrightarrow{v}\cdot \overrightarrow{i}\space^{T}=\sum\limits_{k=1}^{n}v_{k}i_{k}=0$$

>[!example] Dimostrazione
>Per dimostrare il teorema di Tellegen usiamo le equazioni di Tableau: $$\begin{cases}
A\overrightarrow{i}=\overrightarrow{0} \\
A^{T}\overrightarrow{u}-\overrightarrow{v}=\overrightarrow{0}
\end{cases}$$
>Dalla seconda equazione, e sfruttando l'identità della prima equazione:
>$$\begin{align*}
\overrightarrow{v}= A^{T}\overrightarrow{u}\iff \overrightarrow{V}\space^{T}\cdot\overrightarrow{i}= (A^{T}\overrightarrow{u})^{T}\cdot\overrightarrow{i} = \overrightarrow{u}\space^{T}A\overrightarrow{i}=0
\end{align*}$$
