### Circuiti equivalenti di Thevenin e Norton

Supponiamo di avere una rete lineare tempo-variante e una carica in generale tempo variante.
![[Pasted image 20240308143519.png]]

>[!note] Equivalente di Thevenin
>Un bipolo composito adinamico, lineare e affine che ammette base corrente può essere rappresentato come
>![[Pasted image 20240308143632.png]]
>$$V=R_{TH}(i)+E_{TH}=f(i)$$

>[!note] Equivalente di Norton
>Un bipolo composito adinamico, lineare e affine che ammette base tensione può essere rappresentato come
>![[Pasted image 20240308143810.png]]
>$$i=G_{NR}V+A_{NR}$$

Nel caso in cui un bipolo composito ammette entrambi le basi di definizione sarà possibile definire entrambi gli equivalenti e sarà possibile passare da uno all'altro:
$$V=R_{TH}+E_{TH}\Rightarrow i= \frac{1}{R_{TH}}V- \frac{E_{TH}}{R_{TH}}$$

### Generatori pilotati
>[!note]
>I generatori pilotati sono generatori dipendenti da una grandezza pilotante, che può essere una tensione o una corrente.
>Vediamolo rappresentato come tripolo, cioè con 4 variabili descrittive e 2 equazioni costitutive:
>![[Pasted image 20240308133915.png]]
>In generale la sua potenza assorbita equivale a $$p_{a}^{T}=V_{1}i_{1}+V_{2}i_{2}$$

##### Generatore di tensione pilotato in corrente (CCVS)
>[!note]
>![[Pasted image 20240308134215.png]]
>
>| Chiave | Valore |
>| - | - |
>| Grandezza pilotante | $ri_{2}$ |
>| Equazioni costitutive | $\begin{cases} V_1 =ri_2 \\ V_2=0 \end{cases}$ |
>| Base di definizione | $(i_{1},i_{2})$ |
>| Potenza assorbita | $p_{a}^{CCVS}=V_{1}i_{1}=ri_{2}i_{1}$ |

##### Generatore di corrente pilotato in tensione (VCCS)
>[!note]
>![[Pasted image 20240308134814.png]]
>
>| Chiave | Valore |
>| - | - |
>| Grandezza pilotante | $gv_{2}$ |
>| Equazioni costitutive | $\begin{cases} i_1 =gr_2 \\ i_2=0 \end{cases}$ |
>| Base di definizione | $(V_{1},V_{2})$ |
>| Potenza assorbita | $p_{a}^{VCCS}=gV_{1}V_{2}$ |

##### Generatore di corrente pilotato in corrente (CCCS)
>[!note]
>![[Pasted image 20240308135202.png]]
>
>| Chiave | Valore |
>| - | - |
>| Grandezza pilotante | $\beta i_{2}$ |
>| Equazioni costitutive | $\begin{cases} i_1 =\beta i_2 \\ V_2=0 \end{cases}$ |
>| Base di definizione | $(V_{1},i_{2})$ |
>| Potenza assorbita | $p_{a}^{CCCS}=V_{1}i_{1}= \beta V_{1}i_{2}$ |

##### Generatore di tensione pilotato in tensione (VCVS)
>[!note]
>![[Pasted image 20240308135422.png]]
>
>| Chiave | Valore |
>| - | - |
>| Grandezza pilotante | $\alpha V_{2}$ |
>| Equazioni costitutive | $\begin{cases} V_1 =\alpha V_2 \\ i_2=0 \end{cases}$ |
>| Base di definizione | $(V_{2},i_{1})$ |
>| Potenza assorbita | $p_{a}^{VCVS}=V_{1}i_{2}= \alpha V_{2}i_{1}$ |
### Teorema di esistenza e unicità della soluzione
>[!note]
>Consideriamo le $n+l-1$ equazioni di tableau:
>$$\begin{cases}
A\overrightarrow{i}=\overrightarrow{0}&n-1 \\
\overrightarrow{v}=A^{T}\overrightarrow{u}=\overrightarrow{0}&l
\end{cases}$$
>Inoltre scriviamo un insieme di equazioni contenente tutte le $l$ equazioni costitutive del circuito: $$M(t)\overrightarrow{v}+N(t)\overrightarrow{i}=\overrightarrow{z}$$
>
>Otteniamo le $2l+n-1$ equazioni risolutive: $$\begin{cases}
A \overrightarrow{i}=\overrightarrow{0} \\
\overrightarrow{v}-A^{T}\overrightarrow{u}=\overrightarrow{0} \\
M(t)\overrightarrow{v}+N(t)\overrightarrow{i}=\overrightarrow{z}
\end{cases}$$
>
>Raggruppando tutte le incognite in un unico vettore: $$\overrightarrow{w}=\begin{pmatrix}\overrightarrow{u_{t}}\\\overrightarrow{v}\\\overrightarrow{i}\end{pmatrix}$$
>Definiamo quindi il sistema:
>$$\begin{pmatrix}\mathbb{0}&\mathbb{0}&A \\ -A^{T}&\mathbb{1}&\mathbb{0} \\ \mathbb{1}&M(t)&N(t)\end{pmatrix}\begin{pmatrix}\overrightarrow{u}\\\overrightarrow{v}\\\overrightarrow{i}\end{pmatrix}=\begin{pmatrix}\overrightarrow{0}\\\overrightarrow{0}\\\overrightarrow{z}\end{pmatrix}$$
>Dove $\mathbb{0}$ è una matrice nulla e $\mathbb{1}$ è la matrice identità
>In forma compatta $$T(t)\overrightarrow{w}(t)=\overrightarrow{y}(t)$$
>Quindi la soluzione del circuito sarà $\overrightarrow{w}(t)=T^{-1}(t)\overrightarrow{y}(t)$
>
>Il teorema di esistenza e unicità della soluzione afferma che il la soluzione del circuito esiste ed è una se e solo se $$\det(T(t))\neq0$$
>[Vedi metodo di Cramer](https://andrea-bonari.github.io/MAT-03/Sistemi%20lineari/Sistemi%20lineari.html#Metodo_di_Cramer)


>[!tip]
>Le matrici $M$ e $N$ sono matrici diagonali a blocchi

### Principio di sovrapposizione degli effetti (PSE)
>[!note]
>L'intensità di corrente e la tensione associata a ciascun lato del grafo corrispondente al circuito sono pari alla somma delle intensità di corrente e delle tensioni che ciascuno dei generatori indipendenti produrrebbe se agisse da solo con tutti gli altri generatori spenti.

>[!example]
>![[Pasted image 20240312103737.png]]
>$$V=\sum\limits_{k=1}^{M}\alpha_{k}E_{k}+\sum\limits_{j=1}^{N}+r_{j}A_{j}$$

