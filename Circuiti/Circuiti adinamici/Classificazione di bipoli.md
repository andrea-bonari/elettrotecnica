>[!note] Dinamicità
>Un bipolo è dinamico se nella sua equazione costitutiva contiene derivate o integrali.

>[!note] Tempo varianza
>Un bipolo è tempo variante se la sua equazione costitutiva varia nel tempo.

>[!note] Linearità
>Un bipolo è lineare se, data la sua equazione costitutiva $v=f(i)$, vale la definizione di linearità: $$f(\alpha i_{1}+\beta i_{2})= \alpha f(i_{1})+ \beta f(i_{2})$$

>[!note] Classificazione in termini energetici
>In base all'equazione costitutiva $v=f(i)$ possiamo dire che un bipolo è: $$\begin{cases}
\text{passivo}&\text{sse }p_{a}(t)\geq0 \\
\text{attivo}&\text{sse }p_{a}(t)\lesseqgtr0 \\
\text{interte}&\text{sse }p_{a}(t)=0\quad \forall t 
\end{cases}$$

### Bipoli notevoli
>[!note] 
>
>| Simbolo | Nome | Equazione costitutiva | Caratteristiche | Basi di definizione |
>| - | - | - | - | - |
>| ![[Pasted image 20240823172922.png]] | Resistore lineare | $$\begin{matrix}V=Ri&[R]=\ohm\\i=GV&[G]=\text{S}\end{matrix}$$ | $$\begin{align*}&\text{Adinamico}\\&\text{Lineare}\\&\text{Tempo invariante}\\&\text{Passivo}\end{align*}$$ | $$\begin{align*}&\text{Base corrente}\\&\text{Base tensione} \end{align*}$$ |
>| ![[Pasted image 20240823174045.png]] | Corto circuito | $$V=0$$ | $$\begin{align*}&\text{Adinamico}\\&\text{Lineare}\\&\text{Tempo invariante}\\&\text{Inerte}\end{align*}$$ | $$\text{Base corrente}$$ |
>| ![[Pasted image 20240823174318.png]] | Circuito aperto | $$i=0$$ | $$\begin{align*}&\text{Adinamico}\\&\text{Lineare}\\&\text{Tempo invariante}\\&\text{Inerte}\end{align*}$$ | $$\text{Base tensione}$$ |
>| ![[Pasted image 20240823174724.png]] | Generatore indipendente di tensione | $$V=e(t)$$ | $$\begin{align*}&\text{Adinamico}\\&\text{Lineare sse }e(t)\equiv0\\&\text{Tempo variante}\\&\text{Attivo}\end{align*}$$ | $$\text{Base corrente}$$ |
>| ![[Pasted image 20240823175125.png]] | Generatore indipendente di corrente | $$i=a(t)$$ | $$\begin{align*}&\text{Adinamico}\\&\text{Lineare sse }a(t)\equiv0\\&\text{Tempo variante}\\&\text{Attivo}\end{align*}$$ | $$\text{Base tensione}$$ |

### Principio di equivalenza
>[!note]
>Due bipoli si dicono equivalenti se le loro equazioni costitutive coincidono.