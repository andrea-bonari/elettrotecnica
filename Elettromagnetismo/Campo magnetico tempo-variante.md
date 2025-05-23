>[!note]
>Un campo magnetico $\overrightarrow{B}$ è detto tempo-variante quando: $$\frac{\partial}{\partial t}\overrightarrow{B}(x,y,z,t)\neq0$$

### Legge di Faraday-Henry
>[!note]
>In condizioni non stazionarie si ha che $\overrightarrow{E}$ non è conservativo, e di conseguenza non si può definire tensione e non vale la KVL. Si ha che: $$-\oint_{\gamma} \overrightarrow{E}\cdot \text{d}\overrightarrow{l}= \frac{\text{d}}{\text{d}t} \int_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}s$$

>[!example] Dimostrazione
>Consideriamo un circuito chiuso fermo e indeformabile posto in una regione di spazio in cui sia presente $\overrightarrow{B}$. Se $\overrightarrow{B}$ varia nel tempo, si osserva nel circuito una corrente, ossia delle cariche messe in movimento da un campo $\overrightarrow{E}$. Scriviamo la forza elettromotrice come: $$V_\text{fem}= - \frac{\text{d}}{\text{d}t} \Phi_{S}(B)$$
>Cioè: $$-\oint\overrightarrow{E}\cdot \text{d}\overrightarrow{l}= \frac{\text{d}}{\text{d}t} \int_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S\underbrace{=}_{\text{Se il circuito è fermo}}\int_{S} \frac{\partial}{\partial t}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S $$
>La corrente $I$ genera un campo magnetico $\overrightarrow{B}_\text{ind}$ che si oppone alla direzione del cambiamento di $\overrightarrow{B}$. Abbiamo quindi: $$-\oint_{\gamma} \overrightarrow{E}\cdot \text{d}\overrightarrow{l}= \frac{\text{d}}{\text{d}t} \int_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}s$$
>Di conseguenza in condizioni non stazionarie $\overrightarrow{E}$ non è conservativo, e di conseguenza non si può definire tensione e non vale la KVL.

>[!tip] Forza elettromotrice
>Definiamo la forza elettromotrice come il lavoro normalizzato alla carica che $\overrightarrow{E}$ compie per muovere le cariche da un punto ad un altro: $$V_\text{fem}=\int_{\gamma}\overrightarrow{E}\cdot\text{d}\overrightarrow{l}= \frac{L}{q}$$

### Legge di Ampère-Maxwell
>[!note]
>Si ha che, in regime non stazionario, la legge di Ampère-Maxwell è definita come: $$\oint_{L}\overrightarrow{B}\cdot \text{d}\overrightarrow{l}=\mu_{0}\left(\int_{S}\overrightarrow{j}\cdot\hat{u}_{n}\text{ d}S+\varepsilon_{0}\int_{S} \frac{\partial E}{\partial t}\cdot \hat{u}_{n}\text{ d}S\right)$$

Si ha che per $L\to0$, la superficie $S$ diventa chiusa: $$\oint\overrightarrow{B}\cdot \text{d}\overrightarrow{l}=0$$
In generale se $\frac{\partial E}{\partial t} \neq0$: $$\oint_{S}\overrightarrow{j}\cdot\hat{u}_{n}\text{ d}S\neq0$$
Quindi non vale la KCL.

### Leggi di Maxwell per campi elettromagnetici tempo-varianti
>[!note]
>Definiamo le leggi di Maxwell per i campi elettromagnetici tempo-varianti come: $$\begin{align*}
>&\oint_{S}\overrightarrow{E}\cdot\hat{u}_{n}\text{ d}S= \frac{Q}{\varepsilon_{0}}\qquad&\text{Legge di Gauss per il campo elettrico}\\
>&\oint_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S= 0\qquad&\text{Legge di Gauss per il campo magnetico}\\
>&\oint_{L}\overrightarrow{E}\cdot \text{d}\overrightarrow{l}= -\frac{\text{d}}{\text{d}t} \int_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S \qquad&\text{Legge di Faraday-Henry}\\
>&\oint_{L}\overrightarrow{B}\cdot \text{d}\overrightarrow{l}=\mu_{0}\left(\int_{S}\overrightarrow{j}\cdot\hat{u}_{n}\text{ d}S +\int_{S} \frac{\partial E}{\partial t} \cdot\hat{u}_{n}\text{ d}S\right) \qquad&\text{Legge di Ampère-Maxwell}
>\end{align*}$$

