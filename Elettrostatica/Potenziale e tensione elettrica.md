>[!note]
>![[Pasted image 20240822131358.png]]
>Scomponiamo il vettore $\text{d}\overrightarrow{l}$ nelle sue componenti parallele e perpendicolari ad $\overrightarrow{E}$:
>$$\text{d}\overrightarrow{l}=\text{d}\overrightarrow{l}_{\parallel}+\text{d}\overrightarrow{l}_{\perp}$$
>Possiamo quindi dire, dalle precedenti dimostrazioni, che: $$\begin{align*}
\text{d}L&=-q\overrightarrow{E}\cdot \text{d}\overrightarrow{l}= - \frac{1}{4\pi\varepsilon_{0}}\cdot\frac{qQ}{r^{2}}\hat{r}\cdot \left(\text{d}\overrightarrow{l}_{\parallel}+\text{d}\overrightarrow{l}_{\perp}\right)\\
&\Longrightarrow \hat{r}\cdot \text{d}\overrightarrow{l}_{\parallel}+\underbrace{\hat{r}\cdot \text{d}\overrightarrow{l}_{\perp}}_{0}=\text{d}l\cos\theta=\text{d}r\\
&\Longrightarrow \text{d}L=- \frac{qQ}{4\pi\varepsilon_{0}}\cdot\frac{\text{d}r}{r^{2}}\\
\Longrightarrow L_{AB}&= -\frac{qQ}{4\pi\varepsilon_{0}}\int \frac{1}{r^{2}}\space\text{d}r= \frac{qQ}{4\pi\varepsilon_{0}}\cdot \left[\frac{1}{r}\right]^{B}_{A}\\
&= \frac{qQ}{4\pi\varepsilon_{0}r_{B}}-\frac{qQ}{4\pi\varepsilon_{0}r_{A}}\\
&= W(B)-W(A)= q(V_{B}-V_{A})=qV_{BA}
\end{align*}$$
>Definiamo:
>- $W(P)$ come energia potenziale del campo elettrico $\overrightarrow{E}$ nel punto $P$.
>- $V(P)$ come potenziale elettrico del campo elettrico $\overrightarrow{E}$ nel punto $P$.
>- $V_{BA}$ come differenza di potenziale tra $B$ e $A$, oppure tensione.

### Campo elettrico conservativo
>[!note] 
>Se il lavoro non dipende dal percorso, il campo elettrico $\overrightarrow{E}$ è conservativo. Si può dimostrare che se $\overrightarrow{E}$ è quasi-stazionario allora è conservativo.

Calcoliamo il lavoro necessario per un circuito chiuso $\gamma$ formata dall'unione di da $\gamma_{1}$ e $\gamma_{2}$:
![[Pasted image 20240822133332.png]]

$$L^{\gamma_{1}}_{AB}=q(V_{B}-V_{A})\qquad L^{\gamma_{2}}_{BA}=q(V_{A}-V_{B})$$
$$L^{\gamma}=L^{\gamma_{1}}_{AB}+L^{\gamma_{2}}_{BA}=0$$
e quindi:
$$-q\oint_{\gamma}\overrightarrow{E}\cdot\text{d}\overrightarrow{l}=0$$

Quindi in regime quasi-stazionario, la circuitazione del campo elettrico $\overrightarrow{E}$ è nulla, e quindi la tensione complessiva su una linea chiusa è pari a $0$.

### Legge di Kirchhoff per le tensioni (KVL)
>[!note]
>Lungo una qualunque linea chiusa, la somma algebrica delle tensioni, prese con il segno opportuno in base al verso di percorrenza della linea, è nulla.

>[!example]-
>![[Pasted image 20240822134009.png]]
>$$V_{BA}+V_{CB}+V_{AC}=0$$

>[!example]-
>![[Pasted image 20240822134145.png]]
>$$V_{BA}-V_{BC}+V_{AC}=0$$
