>[!note]
>Si ha che tipicamente nelle reti elettriche si esercita corrente alterata alla frequenza di $50\text{ Hz}$ o $60 \text{Hz}$ utilizzando tre fasi. Questo sistema è detto trifase.

Considereremo sempre reti trifase simmetriche ed equilibrate, inoltre riferiremo i fasori delle tensioni e correnti rispetto al valore efficace.

### Valori efficaci
>[!note]
>Definiamo il valore efficace di una grandezza periodica $x(t)$ di un periodo $T$ come: $$X_\text{eff}=\sqrt{\frac{1}{T}\int_{t_{0}}^{t_{0}+T}x^{2}(t)\text{ d}t}$$
>Per una grandezza sinusoidale $x(t)=X_{m}\cos(\omega t+\varphi)$ il valore efficace è quindi: $$X_\text{eff}= \frac{X_{m}}{\sqrt{2}}$$

È possibile esprimere il fasore di una qualsiasi grandezza sinusoidale rispetto al valore massimo o rispetto al valore efficace. Se il fasore è riferito al valore massimo: $$\overline{x}= X_{m}e^{i\varphi}\Longrightarrow x(t)=\text{Re}(\overline{x}e^{i\omega t})$$
Mentre se è riferito al valore efficace: $$\overline{x}=X_{\text{eff}}= \frac{X_{m}}{\sqrt{2}}e^{i\varphi}\Longrightarrow x(t)=\text{Re}(\sqrt{2\overline{x}e^{i\omega t}})$$

>[!tip] Potenze complesse nei trifase
>Se il fasore è riferito al valore massimo: $$\begin{cases}
>V(t)=V_{m}\cos(\omega t+\varphi_{V})\Longrightarrow \overline{V}=V_{m} e^{i\varphi_{V}} \\
>i(t)=I_{m}\cos(\omega t+\varphi_{I})\Longrightarrow \overline{I}=I_{m} e^{i\varphi_{I}}
>\end{cases}\Longrightarrow \hat{A}= \frac{V_{m}e^{i\varphi_{V}}I_{m}e^{i\varphi_{I}}}{2}$$
>Se il fasore è riferito al valore efficace: $$\begin{cases}
>V(t)=V_{m}\cos(\omega t+\varphi_{V})\Longrightarrow \overline{V}=\frac{V_{m}}{\sqrt{2}} e^{i\varphi_{V}} \\
>i(t)=I_{m}\cos(\omega t+\varphi_{I})\Longrightarrow \overline{I}=\frac{I_{m}}{\sqrt{2}} e^{i\varphi_{I}}
>\end{cases}\Longrightarrow \hat{A}= V_{m}e^{i\varphi_{V}}I_{m}e^{i\varphi_{I}}$$

### Tensioni trifase bilanciate
>[!note]
>Un insieme di tensioni trifase bilanciate (o simmetriche) è per definizione costituito da tre tensioni sinusoidali alla medesima pulsazione, con il medesimo valore efficace ma sfasate tra loro di $\frac{2}{3}\pi$. Definiamo quindi la sequenza (o positiva): $$\begin{cases}
>V_{a}(t)=V_{0}(\omega t+ \varphi_{0})\\
>V_{b}(t)=V_{0}(\omega t+ \varphi_{0}- \frac{2}{3}\pi)\\
>V_{c}(t)=V_{0}(\omega t+ \varphi_{0}- \frac{4}{3}\pi)=V_{0}\cos(\omega t+\varphi_{0} + \frac{2}{3}\pi)
>\end{cases}$$
>Definiamo inoltre la sequenza acb (o negativa): $$\begin{cases}
>V_{a}(t)=V_{0}(\omega t+ \varphi_{0})\\
>V_{c}(t)=V_{0}(\omega t+ \varphi_{0}- \frac{2}{3}\pi)\\
>V_{b}(t)=V_{0}(\omega t+ \varphi_{0}- \frac{4}{3}\pi)=V_{0}\cos(\omega t+\varphi_{0} + \frac{2}{3}\pi)
>\end{cases}$$
>
>Entrambe queste sequenze godono della proprietà: $$V_{a}(t)+V_{b}(t)+V_c(t)=0$$

>[!example] Dimostrazione
>Si ha che: $$\begin{align*}
>\overline{V}_{a}+\overline{V}_{b}+\overline{V}_{c}&= V_{p}\left(1+ e^{-i \frac{2}{3}\pi}+e^{-i \frac{4}{3}\pi}\right)= V_{p}\left(1+ e^{-i \frac{2}{3}\pi}+e^{i\frac{2}{3}\pi}\right)\\
>&= V_{p}\left(1+2\cos\left( \frac{2}{3}\pi\right)\right)=V_{p}\left(1+ 2\left(- \frac{1}{2}\right)\right)=0
>\end{align*}$$
>Ricordando che $V_{p}= \frac{V_{0}}{\sqrt{2}}$.

>[!tip] Generazione di tensioni trifase bilanciate
>Le due sequenze vengono tipicamente prodotte da un generatore di tensione trifase (alternatore), costituito da un magnete rotante (rotore) circondato da un sistema di avvolgimenti fisso (statore).
>
>Lo statore include tre avvolgimenti separati, i cui terminali sono spaziati di $\frac{2}{3}\pi$ lungo la circonferenza. Quando il rotore ruota attorno ad un asse ortogonale, il suo campo magnetico produce un flusso tempo-variante nei tre avvolgimenti e quindi una tensione indotta ai morsetti. La sequenza positiva viene generata quando il rotore gira in senso orario, viceversa si genera la sequenza negativa.
>![[Pasted image 20250513091146.png|center]]

La connessione dei morsetti $a'$, $b'$ e $c'$ in un unico morsetto comune $n$ (detto neutro), genera la connessione detta a stella (o ad $Y$) dei tre generazioni.
![[Pasted image 20250513095141.png|center]]

Alternativamente alla connessione a stella è possibile ottenere la connessione a triangolo:
![[Pasted image 20250513095209.png|center]]

Nell'ipotesi di sequenza positiva, le tensioni di linea sono scalate di $\sqrt{3}$ in modulo e ciascuna è in anticipo di $\frac{1}{6}\pi$ rispetto alla corrispondente tensione di fase. Nell'ipotesi di sequenza negativa, le tensioni di linea sono scalate di $\sqrt{3}$ in modulo e ciascuna è in ritardo di $\frac{1}{6}\pi$ rispetto alla corrispondente tensione di fase. La somma delle tensioni di linea è sempre nulla, come accade per quelle di fase.

### Carico trifase bilanciato
>[!note]
>Dato che il sistema trifase è considerato per i nostri scopi in regime sinusoidale permanente i carichi saranno modellati come delle impedenze. Come con i generatori, anche i carichi dei una rete trifase possono essere collegati a stella o triangolo. Il carico si dice bilanciato (o equilibrato) se le impedenze della stella o del triangolo hanno tutte lo stesso modulo e lo stesso argomento. Inoltre, nel caso le impedenze siano tutte uguali, vale la relazione: $$Z_{\triangle}=3Z_{Y}$$



