>[!note]
>Esistono due tipi di discontinuità:
>- Ingressi descritti da funzioni tempo-varianti, quindi la discontinuità non cambia la topologia del circuito
>- Circuito contenenti interruttori, la discontinuità cambia la topologia

### Discontinuità del primo tipo
>[!note]
>Consideriamo la funzione di Heaviside: $$u(x)\text{ o } 1(x)\iff u(x-x_{0})=\begin{cases}
>1\quad&x>x_{0} \\
>0\quad&x<x_{0}
>\end{cases}$$
>E consideriamo le seguenti funzioni: $$\begin{align*}
>e_{1}(t)=\cos(\omega t)\cdot u(t)\\
>e_{2}(t)=\sin(\omega t)\cdot u(t)
>\end{align*}$$
>Assumiamo che gli ingressi siano limitati: $$\frac{\text{d}x}{\text{d}t}= \lambda x+ u(t)$$
>E integriamo l'equazione di stato a cavallo della discontinuità: $$\int_{t_{0}^{-}}^{t_{0}^{+}} \frac{\text{d}x}{\text{d}t}=\lambda \int_{t_{0}^{-}}^{t_{0}^{+}}x(t)\text{ d}t+\int_{t_{0}^{-}}^{t_{0}^{+}}u(t)\text{ d}t=0+0$$
>Questo integrale vale $0$ perché le variabili sono limitate: $$\int_{t_{0}^{-}}^{t_{0}^{+}}x(t)=x(t_{0}^{+})-x(t_{0}^{-})=0\Longrightarrow x(t_{0}^{+})=x(t_{0}^{-})$$
>Quindi le variabili di stato sono continue in presenza di una discontinuità. Le variabili non di stato possono essere discontinue.

