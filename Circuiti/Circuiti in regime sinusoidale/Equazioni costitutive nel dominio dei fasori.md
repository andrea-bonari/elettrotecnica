>[!note]
>
>| Componente                          | Dominio del tempo                                                               | Dominio dei fasori                                                                                                          |
>| ----------------------------------- | ------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
>| Corto circuito                      | $$V(t)=0$$                                                                      | $$\overline{V}=0$$                                                                                                          |
>| Circuito aperto                     | $$i(t)=0$$                                                                      | $$\overline{i}=0$$                                                                                                          |
>| Generatore indipendente di tensione | $$V(t)=E\cos(\omega t+\varphi_{V})$$                                            | $$\overline{V}=E e^{i\varphi_{V}}$$                                                                                         |
>| Generatore indipendente di corrente | $$i(t)=A\cos(\omega t+\varphi_{i})$$                                            | $$\overline{i}=Ae^{i\varphi_{i}}$$                                                                                          |
>| Resistore                           | $$V(t)=Ri(t)$$                                                                  | $$\overline{V}=R\overline{i}$$                                                                                              |
>| Generatore pilotato (generico)      | $$\begin{cases}V_{1}(t)=ri_{2}(t)\\V_{2}(t)=0\end{cases}$$                      | $$\begin{cases}\overline{V}_{1}(t)=r\overline{i}_{2}(t)\\\overline{V}_{2}(t)=0\end{cases}$$                                 |
>| Trasferitore di potenza ideale      | $$\begin{cases}V_{1}(t)=n V_{2}(t)\\i_{1}(t)=- \frac{1}{n}i_{2}(t)\end{cases}$$ | $$\begin{cases}\overline{V}_{1}(t)=n \overline{V}_{2}(t)\\\overline{i}_{1}(t)=- \frac{1}{n}\overline{i}_{2}(t)\end{cases}$$ |
>| Condensatore                        | $$i(t)= C \frac{\text{d}V(t)}{\text{d}t}$$                                      | $$\overline{i}=i\omega C\overline{V}$$                                                                                      |
>| Induttore                           | $$V(t)= L \frac{\text{d}i(t)}{\text{d}t}$$                                      | $$\overline{V}=i\omega L\overline{i}$$                                                                                      |

### Impedenza e ammettenza
>[!note]
>L'impedenza e ammettenza generalizzano al dominio dei fasori i concetti di resistenza e conduttanza. Definiamo l'impedenza come: $$z(i\omega)= \frac{\overline{V}}{\overline{i}}=\underbrace{R}_{\text{Resistenza}}+i\underbrace{X}_{\text{Reattanza}}\qquad [z]=\ohm$$
>Analogamente, definiamo l'ammettenza come: $$y(i\omega)= \frac{\overline{i}}{\overline{V}}=\underbrace{G}_{\text{Conduttanza}}+i\underbrace{B}_{\text{Suscettanza}}\qquad[y]=\text{S}$$
>Si ha che $z$ e $y$ sono numeri complessi, tuttavia non sono fasori.

>[!tip] Analisi fasoriale di un resistore
>Si ha che l'impedenza di un resistore è definita come: $$z=R$$
>Si ha quindi la relazione nel dominio dei fasori: $$\begin{cases}
V=Ri \\
>Ve^{i\varphi_{V}}=Re^{i0}\cdot Ie^{i\varphi_{I}}
>\end{cases}\Longrightarrow \varphi_{V}=\varphi_{I}+0$$
>E quindi geometricamente:
>![[Pasted image 20250410143338.png|center]]

>[!tip] Analisi fasoriale di un condensatore
>Si ha che l'impedenza di un condensatore è definita come: $$z=i\left(- \frac{1}{\omega C}\right)$$
>Si ha quindi come relazione nel dominio dei fasori: $$\begin{cases}
>V= \frac{1}{\omega C}I \\
>Ve^{i\varphi_{V}}= \frac{1}{\omega C}e^{-i \frac{\pi}{2}}\cdot Ie^{i\varphi_{I}}
>\end{cases}\Longrightarrow \varphi_{V}=\varphi_{I} - \frac{\pi}{2}$$
>E quindi geometricamente: 
>![[Pasted image 20250410143409.png|center]]

>[!tip] Analisi fasoriale di un induttore
>Si ha che la reattanza di un di un induttore è definita come: $$y=i(\omega L)$$
>Si ha quindi come relazione nel dominio dei fasori: $$\begin{cases}
>V= \omega LI \\
>Ve^{i\varphi_{V}}=  \omega L e^{i \frac{\pi}{2}}\cdot Ie^{i\varphi_{I}}
>\end{cases}\Longrightarrow \varphi_{V}=\varphi_{I} + \frac{\pi}{2}$$
>E quindi geometricamente: 
>![[Pasted image 20250410143553.png|center]]

### Classificazione delle impedenze
>[!note]
>Si ha che un impedenza $z(i\omega)$ è:
>- Capacitiva se $x(\omega)<0$
>- Induttiva se $x(\omega)>0$
>- Resistiva se $x(\omega)=0$

### Pulsazione di risonanza
>[!note]
>Dati un induttore e un condensatore in serie, si ottiene un impedenza equivalente con equazione costitutiva: $$z(i\omega)= i \left( \omega L- \frac{1}{\omega C}\right)= i \frac{\omega^{2}LC-1}{\omega C}$$
>Si ha che se $\omega= \frac{1}{\sqrt{LC}}$ allora $z=0$, e quindi l'impedenza equivalente si comporta come un corto circuito.
>
>Dati, invece, un induttore e un condensatore in parallelo, si ottiene un impedenza equivalente con equazione costitutiva: $$y(i\omega)=i\left(\omega C- \frac{1}{\omega L}\right)= i \frac{\omega^{2}LC-1}{\omega L}$$
>Si ha che se $\omega= \frac{1}{\sqrt{LC}}$ allora $y=0$, e quindi l'impedenza equivalente si comporta compo un circuito aperto.
