>[!note]
>Un vettore è una $n$-upla di numeri reali caratterizzato da norma, direzione e verso, può essere definito come vettore colonna o vettore riga: $$\overrightarrow{v}\in\mathbb{R}^{n}\qquad\overrightarrow{v}=\begin{pmatrix}v_{1}\\v_{2}\\\vdots\\v_{n}\end{pmatrix}$$

Un $n$-vettore descrive la posizione, quindi le coordinate, di un punto in uno spazio $n$-dimensionale. La norma (norma euclidea, norma 2) di un vettore è la lunghezza del vettore stesso, è definita con le seguenti notazioni e si calcola con la seguente formula
$$||\overrightarrow{v}||=|\overrightarrow{v}|=v=\sqrt{\sum\limits_{i=0}^{n}v_{i}^{2}}$$
### Prodotto di un vettore per uno scalare
>[!note]
>Dati uno scalare $a\in\mathbb{R}$ e un vettore $\overrightarrow{v}\in\mathbb{R}^{n}$
>Il prodotto $n\cdot\overrightarrow{v}$ è $$n\cdot\begin{pmatrix}v_{1}\\v_{2}\\\vdots\\v_{n}\end{pmatrix}=\begin{pmatrix}n\cdot v_{1}\\ n\cdot v_{2}\\\vdots\\ n\cdot v_{n}\end{pmatrix}$$

### Somma e differenza
>[!note]
>Dati due vettori $a,b\in\mathbb{R}^{n}$
>$$a+b=\begin{pmatrix}a_{1}+b_{1}\\a_{2}+b_{2}\\\vdots\\a_{n}+b_{n}\end{pmatrix}$$

### Versori e normalizzazione
>[!note]
>Un vettore con norma unitaria viene definito versore e in simboli si indica:
>$$\widehat{v}\iff|\overrightarrow{v}|=1$$
>
>Per normalizzare un vettore si deve dividerlo per la norma
>$$\widehat{v}=\frac{\overrightarrow{v}}{|\overrightarrow{v}|}$$

### Prodotto scalare
>[!note]
>Il prodotto scalare tra due vettori da come risultato la somma del prodotto tra le singole componenti corrispondenti dei vettori
>$$\overrightarrow{v}\cdot\overrightarrow{w}=|\overrightarrow{v}||\overrightarrow{w}\cdot\cos\theta=v_{1}w_{1}+v_{2}+w_{2}+\cdots+v_{n}w_{n}$$dove $\theta$ è l'angolo minimo tra i due vettori.
>
>Il valore risultante è la norma della proiezione di $v$ su $w$.

### Prodotto vettore
>[!note]
>Siano $\overrightarrow{a},\overrightarrow{b}$ due vettori, allora il prodotto vettore $\overrightarrow{a}\times\overrightarrow{b}=\overrightarrow{c}$ ha:
>- modulo: $|\overrightarrow{c}|=|\overrightarrow{a}||\overrightarrow{b}||\sin\theta|$ dove $\theta$ è l'angolo minimo.
>- direzione perpendicolare al piano su cui giaciono i due vettori.
>- Verso: determinato con regola della mano destra.
>
>Può essere calcolato con l'abuso di notazione:
>$$\overrightarrow{c}=\begin{vmatrix}\overrightarrow{i}&\overrightarrow{j}&\overrightarrow{k}\\a_{1}&a_{2}&a_{3}\\b_{1}&b_{2}&b_{3}\end{vmatrix}$$

