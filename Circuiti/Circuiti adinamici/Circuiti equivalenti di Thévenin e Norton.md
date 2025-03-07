>[!note]
>Sia un bipolo posto ai capi di un bipolo composito, e siano $i$ e $V$ le sue variabili descrittive. I circuiti equivalenti di Thévenin e Norton ci permettono di rappresentare il bipolo composito con un circuito più semplice. È necessario che il bipolo composito sia un rete lineare e tempo-invariante.

### Equivalente di Thévenin
>[!note]
>Definiamo l'equivalente di Thévenin come un bipolo adinamico e lineare-affine che ammette base di definizione corrente: $$V= R_{\text{th}}i+E_{\text{th}}$$
>![[Pasted image 20250306230840.png|center]]

### Equivalente di Norton
>[!note]
>Definiamo l'equivalente di Norton come un bipolo adinamico e lineare-affine che ammetta base di definizione tensione: $$i=G_\text{nr}V+A_\text{nr}$$
>![[Pasted image 20250306230915.png|center]]

### Sostituire equivalenti
>[!note]
>Se la rete lineare ammette entrambe le basi, sono definiti entrambi gli equivalenti: $$\begin{align*}
V= R_{\text{th}}i+E_{\text{th}}&\qquad\Longrightarrow &i=&  \frac{1}{R_{\text{rh}}}V- \frac{E_{\text{th}}}{R_{\text{th}}}\\
i=G_{\text{nr}}V+A_{\text{nr}}&\qquad\Longrightarrow &V=& \frac{1}{G_{\text{nr}}}i- \frac{A_{\text{nr}}}{G_{\text{nr}}}
\end{align*}$$
