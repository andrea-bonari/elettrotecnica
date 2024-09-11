>[!note]
>In un componente dinamico, il valore di tensione o corrente, dipende dai valori precedenti dell'andamento della corrente o tensione.

### Condensatore
>[!note]
>![[Pasted image 20240902165202.png]]
>Nella rappresentazione circuitale:
>![[Pasted image 20240902165330.png]]
>Dove $C$ è la capacità ($[F]$). L'equazione costitutiva è:
>$$Q=Cv$$
>Dove $Q$ è la quantità di carica. Quindi:
>$$i= \frac{\text{d}Q}{\text{d}t}= C \frac{\text{d}v}{\text{d}t}$$
>È definito come un componente dinamico, lineare e tempo-invariante. Ammette base corrente. In regime stazionario avremo $i=0$, quindi:
>![[Pasted image 20240902174812.png]]
>La potenza istantanea è: $$p_{a}=vc \frac{\text{d}v}{\text{d}t}= \frac{\text{d}}{\text{d}t} \left( \frac{1}{2}cv^{2}\right)= \frac{\text{d}}{\text{d}t} w_{c}(t)$$
>dove $w_{c}(t)= \frac{1}{2}cv^{2}$ è l'energia immagazzinata nel componente. È un componente attivo.
### Induttore
>[!note]
>![[Pasted image 20240902165224.png]]
>Nella rappresentazione circuitale:
>![[Pasted image 20240902165354.png]]
>Dove $L$ è l'induttanza ($[H]$). L'equazione costitutiva è: $$\Phi=Li$$
>Dove $\Phi$ è la quantità di flusso del campo magnetico. Quindi:
>$$v= \frac{\text{d}\Phi}{\text{d}t}=L \frac{\text{d}i}{\text{d}t}$$
>È definito come un componente dinamico, lineare e tempo-invariante. Ammette base tensione. In regime stazionario avremo $v=0$, quindi:
>![[Pasted image 20240902174842.png]]
>La potenza istantanea è: $$p_{a}=vc \frac{\text{d}v}{\text{d}t}= \frac{\text{d}}{\text{d}t} \left( \frac{1}{2}Lv^{2}\right)= \frac{\text{d}}{\text{d}t} w_{c}(t)$$
>dove $w_{c}(t)= \frac{1}{2}Lv^{2}$ è l'energia immagazzinata nel componente. È un componente attivo.

>[!tip] Circuito a regime
>È un circuito le cui fasi transitorie sono esaurite

>[!tip] Regime stazionario
>È un regime in cui tutte le grandezze elettriche sono costanti. 

