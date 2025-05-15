>[!note]
>Consideriamo un circuito dinamico, lineare, tempo-invariante che opera in regime sinusoidale alla frequenza $\omega$. Definiamo la potenza assorbita di un generico lato come: $$P_{a}(t)= \frac{VI}{2}\cos \varphi_{z}+ \frac{VI}{2}\cos(2\omega t+ 2\varphi_{V})+ \frac{VI}{2}\sin\varphi_{z}\sin(2\omega t +2\varphi_{V})$$
>Definiamo inoltre la potenza media come: $$\langle P_{a}(t)\rangle= \frac{1}{T}\int_{t}^{t+T}P_{A}(t)\text{ d}t= \frac{VI}{2}\cos\varphi_{z}$$

>[!example] Dimostrazione
>Vogliamo scrivere l'espressione della potenza istantanea assorbita da un generico lato, a cui associamo $v(t)$ e $i(t)$ prese in convenzione normale: $$\begin{align*}
>v(t)&= V\cos(\omega t+\varphi_{V})\\
>i(t)&= I\cos(\omega t+\varphi_{I})
>\end{align*}$$
>Quindi la potenza assorbita + definita come: $$P_{a}(t)=V(t)i(t)=VI\cos(\omega t +\varphi_{V})\cos(\omega t+ \varphi_{I})$$
>Sfruttando la formula trigonometrica $\cos \alpha\cdot \cos \beta= \frac{1}{2}(\alpha -\beta)+ \frac{1}{2}(\alpha+ \beta)$: $$\begin{align*}
>P_{a}(t)&= \frac{VI}{2}\cos(\varphi_{V}-\varphi_{I})+ \frac{VI}{2}\cos(2 \omega t+ \varphi_{V}+ \varphi_{I} +\varphi_{V} -\varphi_{V})\\
>&= \frac{VI}{2}\cos(\varphi_{V}-\varphi_{I})+ \frac{VI}{2}\cos(\underbrace{2\omega t+ 2\varphi_{V}}_{\alpha} +\underbrace{\varphi_{I} -\varphi_{V}}_{\beta})\\
>\end{align*}$$
>Sfruttando la formula trigonometrica della somma $\cos(\alpha + \beta)=\cos \alpha\cos \beta-\sin \alpha\sin\beta$ e considerando la parità del coseno e la disparità del seno: $$\frac{VI}{2}\cos(\varphi_{V}-\varphi_{I})+ \frac{VI}{2}\cos(\varphi_{V}-\varphi_{I})\cos(2\omega t+2\varphi_{V})+ \frac{VI}{2}\sin(\varphi_{V}-\varphi_{I})\sin(2\omega t+2\varphi_{V})$$
>Siccome: $$\overline{V}=z(i\omega)\overline{i}\space\Longrightarrow\space Ve^{i\varphi_{V}}=ze^{i\varphi_{z}}\cdot Ie^{i\varphi{I }}$$
>E quindi le fasi sono $\varphi_{V}-\varphi_{I}=\varphi_{z}$: $$P_{a}(t)= \underbrace{\frac{VI}{2}\cos\varphi_{z}}_{\text{Potenza media}}+ \underbrace{\underbrace{\frac{VI}{2}\cos(\varphi_{z})}_{P}\cos(2\omega t+2\varphi_{V})}_{\text{Potenza attiva istantanea}}+\underbrace{\underbrace{\frac{VI}{2}\sin(\varphi_{z})}_{Q}\sin(2\omega t+2\varphi_{V})}_{\text{Potenza reattiva istantanea}}$$

>[!tip] Potenza istantanea di un resistore in regime sinusoidale
>Si ha che, in fasori, l'equazione costitutiva è: $$Ve^{i\varphi_{V}}=Re^{i0}\cdot Ie^{i\varphi_{I}}$$E quindi $\varphi_{z}=0$. Di conseguenza: si ha: $$P_{a}(t)= \frac{VI}{2}+ \frac{VI}{2}\cos(2\omega t+2\varphi_{V})$$

>[!tip] Potenza istantanea di un condensatore in regime sinusoidale
>Si ha che, in fasori, l'equazione costitutiva è: $$Ve^{i\varphi_{V}}= \frac{1}{\omega C}e^{- \frac{\pi}{2}i}Ie^{i\varphi_{I}}$$
>E quindi $\varphi_{z}=- \frac{\pi}{2}$. Di conseguenza si ha: $$P_{a}(t)=- \frac{VI}{2}\sin(2\omega t+ 2\varphi_{V})$$

>[!tip] Potenza istantanea di un induttore in regime sinusoidale
>Si ha che, in fasori, l'equazione costitutiva è: $$Ve^{i\varphi_{V}}= \omega Le^{- \frac{\pi}{2}i}Ie^{i\varphi_{I}}$$
>E quindi $\varphi_{z}=\frac{\pi}{2}$. Di conseguenza si ha: $$P_{a}(t)= \frac{VI}{2}\sin(2\omega t+ 2\varphi_{V})$$

### Potenza complessa
>[!note]
>Definiamo come potenza complessa erogata il seguente numero complesso:
>$$\hat{A}=P+iQ= \frac{VI}{2}\cos(\varphi_{z})+ i \frac{VI}{2}\sin(\varphi_{z})=\frac{VI}{2}e^{i\varphi_{z}}$$
>Da questa definizione definiamo la potenza apparente $|\hat{A}|=\sqrt{P^{2}+Q^{2}}$, con $P=|\hat{A}|\cos\varphi_{z}$ e $Q=|\hat{A}|\sin\varphi_{z}$.

### Triangolo delle potenze
>[!note]
>Abbiamo che $\overrightarrow{V}=z\overrightarrow{i}$ e quindi che: $$\begin{cases}
>V=|z|I \\
>\varphi_{V}-\varphi_{I}=\varphi
>\end{cases}$$
>Sappiamo anche che: $$\begin{align*}
>\hat{A}&= P+iQ\\
>P&= \frac{VI}{2}\cos\varphi\\
>Q&= \frac{VI}{2}\sin\varphi
>\end{align*}$$
>Consideriamo $\varphi\in\left[- \frac{\pi}{2}, \frac{\pi}{2}\right]$. Osserviamo che per qualunque valore di $\varphi$ la potenza attiva (reale) sarà sempre positiva. Se $\varphi>0$, e quindi $Q>0$, viceversa se $\varphi<0$ anche $Q<0$, possiamo quindi capire facilmente se l'impedenza è capacitiva o induttiva.
>
>Definiamo il fattore di potenza come: $$\cos(\varphi)= \frac{P}{|\hat{A}|}$$
>Se $P$ è in ritardo rispetto ad $|\hat{A}|$, allora l'impedenza è induttiva, viceversa se $P$ è in anticipo rispetto ad $|\hat{A}|$, allora l'impedenza è capacitiva.
