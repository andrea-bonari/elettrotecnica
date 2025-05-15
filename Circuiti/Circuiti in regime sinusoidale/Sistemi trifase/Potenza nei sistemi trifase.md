>[!note]
>Definiamo la potenza istantanea assorbita nei sistemi trifase come: $$p_{a}^{Z_{Y}}(t)=3V_{p}I_{p}\cos\theta$$
>L'espressione della potenza istantanea relativa ad una singola fase è la seguente: $$p_{a}(t)=V_{p}I_{p}\cos\theta+V_{p}I_{p}\cos\theta\cos(2\omega t+2\phi_{V})+V_{p}I_{p}\sin\theta\sin(2\omega t+2\phi_{V})$$
>Poiché la potenza istantanea complessiva è indipendente dal tempo, la potenza media assorbita per fase per il carico a stella o triangolo è: $$\frac{p_{a}^{Z_{Y}}}{3}= \frac{p_{a}^{Z_\triangle}}{3}=V_{p}I_{p}\cos\theta$$
>La potenza attiva e reattiva per fase sono dunque: $$P_{p}=V_{p}I_{p}\cos\theta\qquad Q_{p}=V_{p}I_{p}\sin\theta$$
>La potenza complessa assorbita per fase è pari a: $$\hat{A}_{p}=P_{p}+iQ_{p}$$
>E la potenza complessa assorbita dal carico trifase è pari a: $$\hat{A}_{3ph}=3\hat{A}_{p}$$

>[!example] Dimostrazione
>Consideriamo il calcolo delle potenze di un circuito trifase bilanciato e simmetrico. La potenza istantanea assorbita dal carico trifase, supponendolo collegato a $Y$, si scrive nel dominio del tempo a partire dalle tensioni di fase, per le quali assumiamo potenza positiva: $$\begin{align*}
>V_{AN}(t)&= \sqrt2 V_{p}\cos(\omega t)\\
>V_{BN}(t)&= \sqrt2 V_{p}\cos(\omega t - \frac{2}{3}\pi)\\
>V_{CN}(t)&= \sqrt{2} V_{p}\cos(\omega t- \frac{4}{3}\pi)
>\end{align*}$$
>Assumendo un impedenza di carico $Z_{Y}=|Z_{y}|e^{i\text{arg}(Z_{Y})}=Ze^{i\theta}$ le correnti di fase si possono scrivere come: $$\begin{align*}
>i_{a}(t)&= \sqrt{2} I_{p}\cos(\omega t-\theta)\\
>i_{b}(t)&= \sqrt2 I_{p}\cos(\omega t - \theta - \frac{2}{3} \pi)\\
>i_{c}(t)&= \sqrt{2} I_{p}\cos(\omega t - \theta - \frac{4}{3} \pi)
>\end{align*}$$
>Quindi si ha che: $$\begin{align*}
>p_{a}^{Z_{y}}(t)&= V_{AN}(t)i_{a}(t)+V_{BN}(t)i_{b}(t)+V_{CN}(t)i_{c}(t)=\\
>&= 2V_{p}I_{p}\bigg(\cos(\omega t)\cos(\omega t - \theta) + \cos\left(\omega t- \frac{2}{3}\pi\right)\cos\left(\omega t - \frac{2}{3}\pi- \theta\right)+\\
>&\quad+\cos\left(\omega t- \frac{4}{3}\pi \right)\cos\left(\omega t- \frac{4}{3}\pi - \theta\right)\bigg)\\
>&= V_{p}I_{p}\left(3\cos\theta+\cos(2\omega t -\theta)+\cos\left(2\omega t- \theta- \frac{4}{3}\pi \right)+\cos\left(2\omega t - \theta - \frac{8}{3}\pi \right)\right)=\\
>&= V_{p}I_{p}\bigg(3\cos\theta+\cos\gamma+\cos\gamma\cos\left(\frac{4}{3}\pi\right)+\sin\gamma\sin \left(\frac{4}{3}\pi\right)+\cos\gamma\cos\left(\frac{2}{3}\pi\right)\\&\quad+\sin\gamma\sin\left(\frac{2}{3}\pi\right)\bigg)=\\
>&= V_{p}I_{p}\left(3\cos\theta+\cos\gamma+2\cos\gamma\cos \left(\frac{4}{3}\pi \right)+\sin\gamma\sin\left(\frac{4}{3}\pi\right)-\sin\gamma\sin\left(\frac{4}{3}\pi\right)\right)=\\
>&= V_{p}I_{p}\left(3\cos\theta+\cos\gamma+2\left(- \frac{1}{2}\right)\cos\gamma\right)=3V_{p}I_{p}\cos\theta
>\end{align*}$$
>Dove $\gamma=2\omega t-\theta$.

### Rifasamento
>[!note]
>Per effettuare il rifasamento si effettua l'installazione in parallelo al carico di un banco di condensatori, che eroga almeno una parte della potenza reattiva assorbita dal carico.
>![[Pasted image 20250515114320.png]]
>Il rifasamento permette di ridurre la corrente di linea a monte del complesso costituito dal carico e banco di condensatori: $$I_{l}= \frac{P_{1}}{\sqrt3 V_{l}\cos\varphi}\qquad I_{l_{R}}= \frac{P_{1}}{\sqrt3 V_{l}\cos\varphi_{R}}$$
>Ciò comporta diversi vantaggi, tra cui:
>- La potenza persa delle linee si riduce, diminuiscono quindi gli oneri di trasporto nella bolletta.
>- La caduta di tensione sulle linee si riduce. I carichi domestici operano ad una tensione più vicina alla nominale
>- Cavi di sezione minore



