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
>Sia un induttore collegato ad un generatore di tensione, e si aggiunga in parallelo al carico un condensatore di rifasamento in parallelo al carico ($Q_{C}<0$), dal teorema di Boucherot si ha che $Q_{G}+Q_{Z}=0$. Affinché avvenga il rifasamento perfetto è necessario che: $$Q_{C}=Q_{Z}=0$$
>Si ha che: $$\begin{cases}
>Q_{C}= -\frac{VI}{2}= - \frac{\omega CV^{2}}{2}= - \frac{\omega C|\overline{e}|^{2}}{2} \\
>Q_{Z}= \frac{|\overline{e}|^{2}}{2|z|}\sin\varphi_{z}
>\end{cases}$$
>E quindi: $$\frac{|\overline{e}|^{2}}{2|z|}\sin\varphi_{z}- \frac{\omega C|\overline{e}|^{2}}{2}=0\Longrightarrow C= \frac{\sin\varphi_{z}}{\omega|z|}$$
>Si ha che per questo valore di $C$, la potenza reattiva erogata dal generatore è nulla, e quindi abbiamo rifasato perfettamente il carico.
