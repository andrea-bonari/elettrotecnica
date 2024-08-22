### Connessione in serie di bipoli
>[!note]
>Due bipoli sono connessi in serie quando sono gli unici bipoli a incidere su un dato nodo.
>![[Pasted image 20240307103859.png]]

##### Criteri per la connessione in serie
1. Entrambi i bipoli ammettono base corrente: La connessione in serie è possibile:
![[Pasted image 20240307104833.png]]
$$\begin{cases}
V_{1}=f(i) \\
V_{2}=g(i)
\end{cases}\Rightarrow V=V_{1}+V_{2}=f(i)+g(i)=h(i)$$
Nel caso del resistore:
$$V=V_{1}+V_{2}=R_{1}i+R_{2}i=(R_{1}+R_{2})i$$
![[Pasted image 20240307105125.png]]
2. Uno solo dei bipoli ammette base corrente, la connessione in serie è possibile e il bipolo equivalente è uguale a quello non definito sulla base corrente:

Nel caso di un resistore e un circuito aperto:
![[Pasted image 20240307105117.png]]

3. Entrambi i bipoli non ammettono base corrente, quindi dobbiamo valutare caso per caso se la connessione è possibile:
![[Pasted image 20240307110233.png]]
![[Pasted image 20240307110240.png]]
Per quanto riguarda la tensione generalmente non è possibile collegare in serie quando $$a_{1}(t)\neq a_{2}(t)$$
### Partitore di tensione
![[Pasted image 20240307110350.png]]
Dato il partitore di tensione in figura abbiamo che $$V_{k}=R_{k}\cdot i\qquad V=\sum\limits_{k=1}^{n}V_{k}=i\sum\limits_{k=1}^{n}R_{k}= i\cdot R_{eq}$$
Di conseguenza ricaviamo le formule:
$$i= \frac{V}{R_{eq}}\qquad V_{k}= \frac{R_{k}}{\sum\limits_{k=1}^{n}R_{k}}V$$

Nel caso particolare in cui $n=2$ le formule diventano:
$$V_{1}= \frac{R_{1}}{R_{1}+R_{2}}V\qquad V_{2}= \frac{R_{2}}{R_{1}+R_{2}}V$$

### Connessione in parallelo
>[!note]
>Due bipoli sono connessi in parallelo quando sono connessi alla stessa coppia di nodi.
>![[Pasted image 20240307111354.png]]
>
>È una condizione necessaria che i bipoli in parallelo abbiano la stessa tensione, ma non è sufficiente.

##### Criteri per la connessione in parallelo
1. Se entrambi i bipoli ammettono base tensione la connessione è sempre possibile:

nel caso dei resistori
![[Pasted image 20240307112232.png]]

$$G_{k}= \frac{1}{R_{k}}\qquad i_{1}=G_{1}V\quad i_{2}=G_{2}V$$
$$i=i_{1}+i_{2}=(G_{1}+G_{2})V=G_{eq}V$$
La resistenza equivalente risulta essere:
$$R_{eq}= \frac{1}{G_{eq}}= \frac{1}{\frac{1}{R_{1}}+ \frac{1}{R_{2}}}= \frac{R_{1}R_{2}}{R_{1}+R_{2}}$$
2. Se solo uno dei bipoli ammette base tensione la connessione in parallelo è possibile e il bipolo equivalente è uguale al bipolo non definito su base tensione:

Nel caso di un resistore e un cortocircuito:
![[Pasted image 20240307112543.png]]

3. Se nessuno dei bipoli ammette base tensione dobbiamo valutare caso per caso, se la connessione è possibile o meno:

![[Pasted image 20240307112740.png]]
![[Pasted image 20240307112748.png]]

Per quanto riguarda la corrente generalmente non è possibile collegare in parallelo quando $$e_{1}(t)\neq e_{2}(t)$$
### Partitore di corrente
![[Pasted image 20240307113933.png]]
Dato il partitore di corrente in figura abbiamo che
$$i_{k}=G_{k}V\qquad i=\sum\limits_{k=1}^{n}i_{k}=V\sum\limits^{n}_{k=1}G_{k}= VG_{eq}$$
Siccome sappiamo che $V= \frac{1}{G_{eq}}$ ricaviamo $$i_{k}= \frac{G_{k}}{\sum\limits_{k=1}^{n}G_{k}}i$$
In questo modo distribuiamo la corrente in modo proporzionale alla conduttanza.

Nel caso particolare $n=2$ abbiamo che: $$i_{1}= \frac{G_{1}}{G_{1}+G_{2}}i= \frac{\frac{1}{R_{1}}}{\frac{1}{R_{1}}+ \frac{1}{R_{2}}}\qquad i_{2}= \frac{G_{1}}{G_{1}+G_{2}}$$
