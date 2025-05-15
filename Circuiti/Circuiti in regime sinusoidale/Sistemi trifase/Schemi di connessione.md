>[!note]
>Lo schema generale di un circuito trifase è dato da un generatore trifase e da un carico trifase collegati tramite tre conduttori, che costituiscono la linea trifase.
>Le tensioni tra i conduttori della linea si dicono tensioni di linea o tensioni concatenate. Le correnti che scorrono nella linea trifase si chiamano correnti di linea. Si chiamano invece tensioni di fase e correnti di fase le tensioni a i capi dei singoli bipoli che costituiscono il carico (o generatori) trifase e le correnti che li attraversano.
>![[Pasted image 20250513100302.png|center]]

### Collegamento $Y$-$Y$ Bilanciato
>[!note]
>In questa configurazione, le correnti di linea corrispondono alle correnti di fase del generatore e del carico.
>![[Pasted image 20250513101058.png|center]]
>Valgono le formule: $$\overline{i}_{k}= \frac{\overline{V}_{kn}}{Z_{y}}\qquad \overline{i}_{n}=0$$
>Quindi in una rete trifase simmetrica ed equilibrata, la corrente che circola nel filo di neutro è nulla. Quindi la presenza del filo di neutro è tale per cui i centri stella sono equipotenziali ($\overline{V}_{n,N}=0$).

Si usa analizzare le trifase simmetriche di qualunque tipologia utilizzando un circuito equivalente monofase. In questo modo è possibile ricavare le correnti di fase mancanti. Il circuito monofase equivalente si può ricavare se e solo se tutti i carichi e i generatori connessi sono connessi a stella.

### Collegamento $Y$-$\triangle$ bilanciato
>[!note]
>In questa configurazione, le correnti di linea corrispondo alle correnti di fase del generatore, mentre le tensioni di linea corrispondono alle tensione di fase del carico.
>![[Pasted image 20250515105446.png|center]]
>Ipotizzando, la sequenza positiva delle tensioni di fase del generatore, le tensioni di linea sono scalate di un fattore $\sqrt{3}$ in modulo e ciascuna è in anticipo di $\frac{\pi}{6}$ rispetto alla corrispondente tensione di fase del generatore: $$\begin{align*}
>\overline{i}_{AB}&= \frac{\overline{V}_{ab}}{z_{\triangle}}= \frac{\overline{V}_{AB}}{z_{\triangle}}\\
>\overline{i}_{BC}&= \frac{\overline{V}_{bc}}{z_{\triangle}}= \frac{\overline{V}_{BC}}{z_{\triangle}}\\
>\overline{i}_{CA}&= \frac{\overline{V}_{ca}}{z_{\triangle}}= \frac{\overline{V}_{CA}}{z_{\triangle}} 
>\end{align*}$$
>Operando una trasformazione triangolo-stella del carico, è possibile ridurre il circuito ad una connessione di tipo $Y$-$Y$ e introdurre l'equivalente monofase.

### Collegamento $\triangle$-$Y$ bilanciato
>[!note]
>In questa configurazione, le correnti di linea corrispondono alle correnti di fase del carico, mentre le tensioni di linea corrispondono alle tensioni di fase del generatore.
>![[Pasted image 20250515110209.png|center]]
>Per ottenere le correnti di linea è possibile operare in modi diversi. Una possibilità è ricavare la configurazione a stella del generatore trifase equivalente al triangolo presente e riportarsi quindi ad uno schema $Y$-$Y$.

### Collegamento $\triangle$-$\triangle$ bilanciato
>[!note]
>In questa configurazione, le tensioni di linea corrispondono alle tensioni di fase del generatore e del carico.
>![[Pasted image 20250515110417.png|center]]
>Perciò le correnti di fase sono: $$\begin{align*}
>\overline{i}_{AB}&= \frac{\overline{V}_{ab}}{z_{\triangle}}= \frac{\overline{V}_{AB}}{z_{\triangle}}\\
>\overline{i}_{BC}&= \frac{\overline{V}_{bc}}{z_{\triangle}}= \frac{\overline{V}_{BC}}{z_{\triangle}}\\
>\overline{i}_{CA}&= \frac{\overline{V}_{ca}}{z_{\triangle}}= \frac{\overline{V}_{CA}}{z_{\triangle}} 
>\end{align*}$$

