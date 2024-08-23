### Potenza ed energia elettrica
>[!note]
>Consideriamo il bipolo:
>![[Pasted image 20240229105948.png]]
>Abbiamo che il lavoro compiuto da $\overrightarrow{E}$ per spostare $\triangle Q$ da $A$ a $B$ è: $$L_{AB}=\triangle Q\int _{AB}\overrightarrow{E}\cdot d\overrightarrow{l}= -\triangle Q\int_{AB}\overrightarrow{E}\cdot d\overrightarrow{l}=\triangle Q V_{AB}$$
>Abbiamo quindi che $$L_{AB}=W_{A}-W_{B}=\triangle W=\triangle Q V_{AB}$$
>Dividendo per $\triangle t$ e facendo il limite per il rapporto incrementale ottengo:
>$$\lim_{\triangle t\to0} \frac{\triangle W}{\triangle t}= \frac{dW}{dt}= \frac{dQ}{dt}V_{AB}= i\cdot V_{AB}$$
>
>Di conseguenza la potenza istantanea è definita come: $$p(t)= \frac{d}{dt}W(t)=V(t)i(t)\qquad [V\cdot A]=[J/s]=[W]$$
### Potenza assorbita ed erogata
>[!note]
>##### Convenzione normale:
>- $p(t)>0\iff \triangle W>0\iff W_{A}>W_{B}$:
>	Il bipolo ha assorbito energia e definiamo la potenza assorbita come $p_{a}(t)=v(t)i(t)$
 >- $p(t)<0$: Il bipolo ha erogato energia e definiamo la potenza erogata come $p_{e}(t)=-V(t)i(t)$
>
>##### Convenzione dei generatori:
>- Potenza erogata:$$p_{e}(t)=V(t)i(t)$$
>- Potenza assorbita: $$p_{a}(t)=-V(t)i(t)$$

>[!example]
>Consideriamo il circuito:
>![[Pasted image 20240229112221.png]]
>Possiamo dire che: $$p_{a}^{R}=V_{R}i_{r}$$$$p_{e}^{R}=V_{E}i_{E}=V_{R}i_{R}=p_{a}^{R}$$

