>[!note]
>Un fasore $\overline{x}$ è un numero complesso che ha come modulo e angolo rispettivamente l'ampiezza e la fase della sinusoide associata: $$x(t)=X\cos(\omega t+ \varphi)\iff \overline{x}=Xe^{i\varphi}$$
>Si ha che: $$x(t)=\text{Re}\left(\overline{x}\cdot e^{i\omega t}\right)$$

Si ha che i fasori sono unici e lineari:
$$\begin{align*}
&\overline{x}_{1}=\overline{x}_{2}\iff x_{1}(t)=x_{2}(t)\\
&\overline{x}=\alpha \overline{x}_{1}+\beta \overline{x}_{2} \iff x(t)=\alpha x_{1}(t)+\beta x_{2}(t)
\end{align*}$$
### Derivabilità dei fasori
>[!note]
>Si ha che la derivata di un fasore è proporzionale a se stesso: $$\frac{\text{d}}{\text{d}t} \overline{x}=i\omega \overline{x}$$

>[!example] Dimostrazione
>Sia: $$y(t)= \frac{\text{d}}{\text{d}t} \bigg(X\cos(\omega t+ \varphi)\bigg)=-\omega X\sin(\omega t+\varphi)$$
>Siccome $\sin(x)=-\cos\left(x + \frac{\pi}{2}\right)$: $$y(t)=\omega X \cos\left(\omega t+\varphi + \frac{\pi}{2}\right)$$
>Convertendo questo valore in fasore: $$\overline{y}= \omega Xe^{i\left(\varphi + \frac{\pi}{2}\right)}= \omega Xe^{i\varphi}\left(\cos \frac{\pi}{2}+ i\sin \frac{\pi}{2}\right)= i\omega Xe^{i\varphi}$$
>Notando che $\overline{x}=Xe^{i\varphi}$ è il fasore di $x(t)$, si ha che: $$\overline{y}=i\omega \overline{x}$$

### Metodo dei fasori
>[!note]
>Dato un circuito costituito da $n$-terminali lineari, dinamici e sorgenti impressive di tipo sinusoidale a frequenza fissa, possiamo sostituire ciascuna tensione e corrente con il corrispondente fasore.

Nel dominio dei fasori le KCL e KVL continuano ad essere valide.
