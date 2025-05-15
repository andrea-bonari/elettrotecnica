>[!note]
>Il teorema di Boucherot estende il teorema di Tellegen al regime sinusoidale: $$\begin{cases}
>\sum\limits_{k=1}^{l}P_{k}=0 \\
>\sum\limits_{k=1}^{l}Q_{k}=0 \\
>\end{cases}$$

>[!example] Dimostrazione
>Dal teorema di Tellegen si ha: $$\overrightarrow{V}\space^{T}(t)\cdot\overrightarrow{i}(t)=0$$
>Con $\overrightarrow{V}$ e $\overrightarrow{i}$ vettori di tensioni e correnti compatibili con il grafo del circuito. Il teorema di Tellegen vale anche in regime sinusoidale. Passando al dominio dei fasori: $$\overrightarrow{\overline{V}}\space^{T}\cdot\overrightarrow{\overline{i}}=0$$
>Per ragionare in potenza complessa, si vuole avere che: $$\frac{1}{2}\overrightarrow{\overline{V}}\space^{T}\cdot\overrightarrow{\overline{i}}\space^{*}=0$$
>Se $\overrightarrow{\overline{i}}$ è un vettore di correnti compatibile con il grafo del circuito, verifichiamo che lo è anche $\overrightarrow{\overline{i}}\space^{*}$. Scriviamo la KCL al $k$-esimo nodo del circuito: $$\sum\limits_{h=1}^{n}\alpha_{h}\overline{i}_{h}=0$$
>E quindi: $$\sum\limits_{h=1}^{n}\alpha_{h}\text{Re}(\overline{i}_{h})+i\sum\limits^{n}_{h=1}\alpha_{h}\text{Im}(\overline{i}_{h})=0$$
>Che è verificata se e solo se: $$\begin{cases}
>\sum\limits_{h=1}^{n}\alpha_{h}\text{Re}(\overline{i}_{h})=0 \\\sum\limits_{h=1}^{n}\alpha_{h}\text{Im}(\overline{i}_{h})=0
>\end{cases}$$
>Sostituisco ad $\overline{i}_{h}$ il suo complesso coniugato: $$\sum\limits_{h=1}^{n}\alpha_{h}\overline{i}^{*}_{h}=0$$
>Si ha quindi che: $$\begin{cases}
>\sum\limits_{h=1}^{n}\alpha_{h}\text{Re}(\overline{i}_{h})=\sum\limits_{h=1}^{n}\alpha_{h}\text{Re}(\overline{i}^{*}_{h})=0 \\\sum\limits_{h=1}^{n}\alpha_{h}\text{Im}(\overline{i}_{h})=-\sum\limits_{h=1}^{n}\alpha_{h}\text{Im}(\overline{i}_{h}^{*})=0
>\end{cases}$$
>Che è verificata, di conseguenza $\overrightarrow{\overline{i}}\space^{*}$ è un vettore di correnti compatibili con il grafo del circuito. Quindi: $$\frac{1}{2}\overrightarrow{\overline{V}}\space^{T}\cdot\overrightarrow{\overline{i}}\space^{*}=\sum\limits_{k=1}^{l}(P_{k}+iQ_{k})=0$$
>E di conseguenza: $$\begin{cases}
>\sum\limits_{k=1}^{l}P_{k}=0 \\
>\sum\limits_{k=1}^{l}Q_{k}=0 \\
>\end{cases}$$

### Rifasamento
>[!note]
>Sia un circuito composto da un generatore di tensione $\overline{E}$ connesso ad un carico $z(i\omega)$. Per farlo è necessario mettere in parallelo al carico un condensatore di valore: $$C= \frac{\sin\varphi_{z}}{\omega|z|}$$
>![[Pasted image 20250508110158.png|center]]
>

>[!example] Dimostrazione
>Sia un circuito composto da un generatore di tensione $\overline{E}$ connesso ad un carico $z(i\omega)$. Tipicamente $z(i\omega)$ è induttiva, e avrà quindi $Q_{Z}$ potenza reattiva, mentre il generatore $\overline{E}$ avrà potenza reattiva $Q_{G}$. Per il teorema di Boucherot si ha che: $$Q_{G}+Q_{Z}=0$$
>Minimizziamo la potenza reattiva del generatore $\overline{E}$. Per farlo poniamo in parallelo tra il carico e il generatore un condensatore di rifasamento di conduttanza $- \frac{i}{\omega C}$.
>In questo caso il teorema di Boucherot diventa: $$Q_{G}+Q_{Z}+Q_{C}=0$$
>Voglio imporre $Q_{G}=0$, e quindi $Q_{Z}+Q_{C}=0$. Si ha che: $$Q= \frac{VI}{2}\sin\varphi_{z}$$
>Nel caso della nostra impedenza: $$Q_{Z}= \frac{|\overline{E}|^{2}}{2|z|}\sin\varphi_{z}$$
>Mentre per il condensatore: $$Q_{C}= - \frac{\omega C |\overline{E}|^{2}}{2}$$
>Quindi: $$\frac{|\overline{E}|^{2}}{2|z|}\sin\varphi_{z}- \frac{\omega C|\overline{E}|^{2}}{2}=0$$
>E di conseguenza, per un rifasamento perfetto e completo si deve avere: $$C= \frac{\sin\varphi_{z}}{\omega |z|}$$
>In alternativa, per rifasare perfettamente un carico, è sufficiente far si che il carico complessivo sia puramente resistivo: $$C=\frac{L}{R^{2}+\omega^{2}L^{2}}$$
