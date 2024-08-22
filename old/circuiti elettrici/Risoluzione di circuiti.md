### Potenza istantanea di un $n$-polo
>[!note]
>Generalizziamo il concetto di potenza istantanea al caso di un $n$-polo:
>![[Pasted image 20240301135827.png]]
>
>Supponiamo che:
>- l'$n$-polo sia descritto con nodo di riferimento
>- utilizziamo la convenzione normale
>$$p_{a}(t)=\sum\limits_{k=1}^{n-1}\underbrace{V_{k}(t)i_{K}(t)}_{\text{potenza assorbita da ogni porta}}$$

### Teorema di Tellegen
>[!note]
>Supponiamo di avere:
>- Un circuito il cui grafo è connesso e contiene $n$ nodi e $l$ lati.
>- Convenzione normale per tutti i lati del grafo associato al circuito.
>
>Definiamo tensioni e correnti compatibili con il grafo:
>$$\overrightarrow{i}=\begin{pmatrix}i_{1}\\i_{2}\\\vdots\\i_{n}\end{pmatrix}\qquad \overrightarrow{V}=\begin{pmatrix}V_{1}\\V_{2}\\\vdots\\V_{n}\end{pmatrix}$$
>
>Il teorema di Tellegen afferma che $$\overrightarrow{V}\text{ }^{T}\overrightarrow{i}= \overrightarrow{i}\text{ }^{T}\overrightarrow{V}=\sum\limits_{k=1}^{n}\underbrace{V_{k}i_{k}}_\text{potenza assorbita da ciascun lato}=0$$

>[!abstract] Dimostrazione
>Usiamo le equazioni di Tableau:
>$$\begin{cases}
A\overrightarrow{i}=\overrightarrow{0} \\
A^{T}\overrightarrow{u}-\overrightarrow{v}=\overrightarrow{0}&\Rightarrow& \overrightarrow{V}=A^{T}\overrightarrow{u}
\end{cases}$$
$$\overrightarrow{V}\text{ }^{T}\overrightarrow{i}=(A^{T}\overrightarrow{u})^{T}\overrightarrow{i}=\overrightarrow{u}\text{ }^{T}\underbrace{A\overrightarrow{i}}_\text{nullo}=0$$

### Principio di equivalenza
>[!note]
>Due bipoli si dicono equivalenti quando le loro equazioni costitutive coincidono:
>![[Pasted image 20240301141641.png]]
