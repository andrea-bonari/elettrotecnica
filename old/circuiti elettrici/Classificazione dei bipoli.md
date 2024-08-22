>[!note] Dinamici o Adinamici
>Un bipolo è dinamico se la sua equazione costitutiva contiene derivate o integrali.

>[!note] Tempo varianti o Tempo Invarianti
>Un bipolo è tempo variante se la sua equazione costitutiva cambia nel tempo.

>[!note] Lineare o non lineare
>Un componente è lineare se data l'equazione costitutiva $v=f(i)$ si ha che $$f(\alpha i_{1}+ \beta i_{2})=\alpha f(i_{1})+\beta f(i_{2})$$

>[!note] Termini energetici
>Sapendo che in convenzione lineare $p_{a}(t)=Vi$ possiamo classificare i bipoli come:
>1. **Inerte** se $p_{a}(t)=0$
>2. **Passivo** se $p_{a}(t)\geq0$
>3. **Attivo** se $p_{a}(t)\in\mathbb{R}$

### Basi di definizione
>[!note]
>Considero un generico $n$-terminali, esso si dice:
>
>1. Definito su **base tensione** se è possibile assegnare tutte le $n-1$ tensioni e ricavare le corrispondenti $n-1$ correnti: $$\overrightarrow{i}= \overrightarrow{f}(\overrightarrow{v})$$
>2. Definito su **base corrente** se è possibile assegnare tutte le $n-1$ correnti e ricavare le corrispondenti $n-1$ tensioni: $$\overrightarrow{v}=\overrightarrow{g}(\overrightarrow{i})$$
>3. Definito su **base mista** se è possibile assegnare un sottoinsieme di correnti e un sottoinsieme di tensioni e ricavare le restanti variabili descrittive $$\overrightarrow{i}=\overrightarrow{f}(\overrightarrow{v})$$

>[!tip] Porta
>Coppia di tensione-corrente di un polo

>[!example]
>![[Pasted image 20240229122148.png]]
>Supponiamo che le equazioni costitutive siano $$V_{1}=\alpha i_{1}\qquad i_{2}=\beta i_{1}+\gamma V_{2}$$
>
>Il tripolo ammette base corrente perché $$\begin{cases}
V_{1}=\alpha i_{1}&= f_{1}(i_{1},i_{2}) \\
V_{2}= - \frac{\beta}{\gamma}i_{1}+ \frac{1}{\gamma}i_{2}&=f_{2}
(i_{1},i_{2})\end{cases}$$
>Il tripolo ammette base tensione perché $$\begin{cases}
i_{1}= \frac{1}{\alpha}V_{1}&=g_{1}(V_{1},V_{2}) \\
i_{2}= \frac{\beta}{\alpha}V_{1}+ \gamma V_{2}&= g_{2}(V_{1},V_{2})
\end{cases}$$
>Il tripolo ammette $(i_{1},V_{2})$ e $(i_{2},V_{1})$ come basi miste ($(i_{1},V_{1})$ e $(i_{2},V_{2})$ non sono basi miste perché non possiamo imporre $V$ e $i$ alla stessa porta)

