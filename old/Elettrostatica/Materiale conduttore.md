>[!note]
>Un materiale conduttore è un materiale in cui vi sono cariche libere di muoversi.
>![[Pasted image 20240822171354.png]]
>Il movimento degli elettroni è casuale, tuttavia, in media la corrente complessiva sarà pari a $0$ ($I=0$). Nel momento in cui sarà applicato un campo elettrico $\overrightarrow{E}$, gli elettroni saranno soggetti ad una forza $-e\overrightarrow{E}$, e cominceranno a spostarsi all'interno del conduttore con una velocità $\overrightarrow{v}$. La velocità che raggiungono gli elettroni (non MRUA) è detto "di Drift" ed è definita come: $$\overrightarrow{v}=-\mu\overrightarrow{E}$$
>Con $\mu>0$ detta mobilità delle cariche libere.

### Legge di Ohm
>[!note]
>La resistenza dipende sia dalle caratteristiche fisiche del materiale sia dalla sua geometria:
>$$I=\underbrace{\gamma}_{\text{conduttività } [S\cdot m^{-1}]} \frac{\Delta S}{\Delta l}V_{AB}= \underbrace{G}_{\text{conduttanza } [S]} V_{AB}$$
>$$V_{AB}= \underbrace{\rho}_{\text{Resistività } [\ohm\cdot m]} \frac{\Delta l}{\Delta S}I=\underbrace{R}_{\text{Resistenza } [\ohm]}I$$

>[!example] Dimostrazione
>![[Pasted image 20240822173135.png]]
>Supponiamo per ipotesi che i portatori di carica siano elettroni ($\rho_{v}<0$) e che il campo elettrico $\overrightarrow{E}$ sia costante all'interno del materiale.
>$$\begin{align*}
V_{AB}&=V_{A}-V_{B}=-\int_{\gamma}\overrightarrow{E}\cdot \text{d}\overrightarrow{l}=-E\int_{\gamma}\hat{E}\cdot \text{d}\overrightarrow{l}\\
&= E\cdot \Delta l\iff E= \frac{V_{AB}}{\Delta l}\\
\Longrightarrow \Delta Q&=\rho_{r}\cdot v\cdot\Delta t\cdot\Delta S=\rho_{r}\cdot \mu E\cdot\Delta t\cdot\Delta S\\
\Longrightarrow I&= \frac{\Delta Q}{\Delta t}=\rho_{r}\cdot\mu \cdot \frac{V_{AB}}{\Delta l}\Delta S\\
&= \underbrace{\gamma}_{\text{conduttività } [S\cdot m^{-1}]} \frac{\Delta S}{\Delta l}V_{AB}= \underbrace{G}_{\text{conduttanza } [S]} V_{AB}\\
\Longrightarrow V_{AB}&= \underbrace{\rho}_{\text{Resistività } [\ohm\cdot m]} \frac{\Delta l}{\Delta S}I=\underbrace{R}_{\text{Resistenza } [\ohm]}I
\end{align*}$$

>[!warning] "Verso" della corrente
>Indipendentemente dal tipo di portatore di carica, la densità di corrente sarà sempre orientata nello stesso modo e la corrente sarà sempre positiva nello stesso verso.
