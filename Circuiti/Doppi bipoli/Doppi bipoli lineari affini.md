>[!note]
>Un doppio bipolo è detto lineare affine quando le sue equazioni costitutive sono rappresentabili con equazioni costitutive: $$A\overrightarrow{V}+B\overrightarrow{i}+\overrightarrow{c}=0\qquad\begin{align*}
>\overrightarrow{v}&= (v_{1},v_{2})\\\overrightarrow{i}&= (i_{1},i_{2})
>\end{align*}$$
>![[Pasted image 20250324185052.png|center]]

Se $\overrightarrow{c}=\overrightarrow{0}$, cioè il doppio bipolo non presenta generatori indipendenti, allora è possibile scrivere le equazioni costitutive nella forma: $$\overrightarrow{u}=M\overrightarrow{w}$$
Dove $\overrightarrow{w}$ sono variabili indipendenti, e $\overrightarrow{u}$ sono le variabili dipendenti.

### Matrici di rappresentazione
>[!note]
>Le basi di definizione canoniche di un doppio bipolo lineare affine sono: $$\begin{pmatrix}i_{1}\\i_{2}\end{pmatrix}\qquad\begin{pmatrix}V_{1}\\V_{2}\end{pmatrix}\qquad \begin{pmatrix}i_{1}\\V_{2}\end{pmatrix}\qquad \begin{pmatrix}i_{2}\\V_{1}\end{pmatrix}$$
>Nel caso della base corrente $(i_{1}, i_{2})$, si ha la matrice di resistenza, e quindi che l'equazione costitutiva è: $$V=R\overrightarrow{i}\qquad [R_{ij}]=\ohm$$
>Nel caso della base tensione $(V_{1},V_{2})$, si ha la matrice di conduttanza, e quindi che l'equazione costitutiva è: $$\overrightarrow{i}=G\overrightarrow{v}\qquad [G_{ij}]=\text{S}$$
>Nel caso della base $(i_{1}, V_{2})$, si ha la matrice ibrida di tipo 1, e quindi che l'equazione costitutive è: $$\begin{pmatrix}V_{1}\\i_{2}\end{pmatrix}=H\begin{pmatrix}i_{1}\\V_{2}\end{pmatrix}\qquad [H_{11}]=\ohm\quad [H_{22}]=\text{S}\quad [H_{21}],[H_{12}]=1$$
>Nel caso della base $(i_{2},V_{1})$, si ha la matrice ibrida di tipo 2, e quindi che l'equazione costitutiva è: $$\begin{pmatrix}i_{1}\\V_{2}\end{pmatrix}=H'\begin{pmatrix}V_{1}\\i_{2}\end{pmatrix}\qquad [H'_{11}]=\text{S}\quad [H'_{22}]=\ohm\quad [H'_{21}],[H'_{12}]=1$$
>Esiste inoltre il caso speciale della base $(V_{2},-i_{2})$, in questo caso si ha la matrice di trasmissione diretta, e quindi che l'equazione costitutiva è: $$\begin{pmatrix}V_{1}\\i_{1}\end{pmatrix}=T\begin{pmatrix}V_{2}\\-i_{2}\end{pmatrix}\qquad [T_{12}]=\ohm\quad [T_{21}]=\text{S}\quad [T_{11}],[T_{22}]=1$$
>Esiste anche il caso speciale della base $(V_{1},i_{1})$, in questo caso si ha la matrice di trasmissione inversa, e quindi che l'equazione costitutiva è: $$\begin{pmatrix}V_{2}\\i_{2}\end{pmatrix}=T'\begin{pmatrix}V_{1}\\i_{1}\end{pmatrix}\qquad [T'_{12}]=\ohm\quad [T'_{22}]=\text{S}\quad [T'_{11}],[H'_{22}]=1$$

È possibile ricavare ogni matrice utilizzando il metodo delle prove semplici.
### Simmetria di doppi bipoli
>[!note]
>Un doppio bipolo è detto simmetrico se è possibile scambiare le variabili descrittive lasciando invariate le equazioni costitutive. Cioè il doppio bipolo si comporta alla stessa maniera indipendentemente di come è collegato al circuito.

>[!tip] Condizioni di simmetricità per le matrici di rappresentazione
>| $$\text{Matrice}$$                     | $$\text{Condizione di simmetricità}$$                    |
>| -------------------------------------- | -------------------------------------------------------- |
>| $$\text{Matrice di resistenza }R$$     | $$R_{11}=R_{22}$$ |
>| $$\text{Matrice di conduttanza }G$$    | $$G_{11}=G_{22}$$ |
>| $$\text{Matrice ibrida di tipo 1 }H$$  | $$det(H)=1$$    |
>| $$\text{Matrice ibrida di tipo 2 }H'$$ | $$\det(H')=1$$ |
>| $$\text{Matrice di trasmissione } T$$  | $$T_{11}=T_{22}$$     |

La simmetria è una proprietà intrinseca di un doppio bipolo, cioè non dipende dalla rappresentazione scelta.