>[!note]
>Supponiamo di avere una rete lineare, definibile come bipolo composito, tale che:
>![[Pasted image 20240824170611.png]]
>Supponendo che:
>- rete lineare e tempo-invariante
>- carico in generale- tempo variante
>
>Definiamo l'equivalente di Thevenin come un bipolo adinamico e lineare-affine che ammette basi di definizione corrente:
>![[Pasted image 20240824170727.png]]
>$$v=f(i)=R_{TH}i+E_{TH}$$
>Analogamente, definiamo l'equivalente di Norton come un bipolo adinamico e lineare-affine che ammette base tensione:
>![[Pasted image 20240824170902.png]]
>$$i=g(v)=G_{NR}V+A_{NR}$$
>In caso la rete lineare ammette entrambi le basi, sono definiti entrambi gli equivalenti:
>$$v=R_{TH}i+E_{TH}\Longrightarrow i= \frac{1}{R_{TH}}V- \frac{E_{TH}}{R_{TH}}$$
>![[Pasted image 20240824171139.png]]

### Teoremi di Thevenin e Norton
>[!note]
>Consideriamo un bipolo composito contenente componenti lineari, adinamici, tempo-varianti e sorgenti impressive di tensione e corrente.
>
>Il teorema di Thevenin afferma che, se circuito ammette una ed una soluzione per qualunque valore di $i$ (Cioè il bipolo composito è controllabile in corrente), allora esiste il circuito equivalente di Thevenin:
>![[Pasted image 20240830111227.png]]
>
>Analogamente, il teorema di Norton afferma che, se il circuito ammette una ed una soluzione per qualunque valore di $v$, allora esiste il circuito equivalente di Norton:
>![[Pasted image 20240830153226.png]]

>[!example] Dimostrazione del teorema di Thevenin
>Applico il principio di sovrapposizione degli effetti al circuito composto dal bipolo composito e il generatore indipendente di corrente.
>$$v=r_{0}i+\sum\limits_{k=1}^{N}r_{k}A_{k}+\sum\limits_{k=1}^{M}\alpha_{k}E_{k}$$
>Passiviamo i generatori indipendenti interni al bipolo composito e otteniamo: $$v\bigg|_{\begin{align*}
>A_{k}=0\\
>E_{k}=0
>\end{align*}}=r_{0}i\iff$$
>$$\frac{v}{i}\bigg|_{\begin{align*}
>A_{k}=0\\
>E_{k}=0
>\end{align*}}=r_{0}=R_{TH}$$
>Passiviamo il generatore indipendente $i$ e otteniamo:
>$$v\bigg|_{i=0}=\sum\limits_{k=1}^{N}r_{k}A_{k}+\sum\limits_{k=1}^{M}\alpha_{k}E_{k}=E_{TH}$$

>[!example] Dimostrazione Teorema di Norton
>Analoga alla dimostrazione del Teorema di Norton

