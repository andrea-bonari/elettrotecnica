>[!note]
>È possibile estendere l'equazione costitutiva di un induttore $\Phi= Li$ ad un numero $n$ arbitrario di avvolgimenti: $$\overrightarrow{\Phi}=L \overrightarrow{i}$$
>Dove $L$ è la matrice di induttanze.

### Caso $n=2$
>[!note]
>Per il caso $n=2$ si ha che il componente è rappresentato come:
>![[Pasted image 20250508113641.png|center]]
>Si ha che: $$L=\begin{pmatrix}L_{1}&M\\M&L_{2}\end{pmatrix}\iff\begin{cases}
>V_{1}= L_{1} \frac{\text{d}i_{1}}{\text{d}t} + M \frac{\text{d}i_{2}}{\text{d}t}\\
>V_{2}= M \frac{\text{d}i_{1}}{\text{d}t} + L_{2} \frac{\text{d}i_{2}}{\text{d}t}
>\end{cases}$$
>Dove $M$ è detta mutua induttanza. Definiamo inoltre il coefficiente di accoppiamento come: $$k= \frac{M}{\sqrt{L_{1}L_{2}}}$$
>Si ha che se $\det(L)=0$ ci troviamo nella condizione di accoppiamento perfetto ($k=\pm 1$).
>Si ha inoltre che l'energia immagazzinata sarà: $$p(t)= \frac{\text{d}}{\text{d}t} W(t)$$

>[!example] Dimostrazione
>$$\begin{align*}
>p(t)&= V_{1}i_{1}+V_{2}i_{2}= L_{1} \frac{\text{d}i_{1}}{\text{d}t}i_{1}+M \frac{\text{d}i_{2}}{\text{d}t}i_{1} +M \frac{\text{d}i_{1}}{\text{d}t}i_{2}+L_{2} \frac{\text{d}i_{2}}{\text{d}t}i_{2}\\
>&= \frac{\text{d}}{\text{d}t} \underbrace{\left(\frac{1}{2} L_{1}i_{1}^{2}+ \frac{1}{2}L_{2}i_{2}^{2}+Mi_{1}i_{2}\right)}_{W(t)}
>\end{align*}$$

