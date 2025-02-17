### Classificazione dei bipoli
>[!note]
>I bipoli possono essere classificati secondo vari criteri:
>- Dinamicità
>- Tempo-varianza
>- Linearità
>- Termini energetici

>[!tip] Dinamici o Adinamici
>Un bipolo è dinamico se nella sua equazione costitutiva compaiono derivate o integrali. Viceversa, se un bipolo non contiene derivate o integrali è detto adinamico.

>[!example]
>![[Pasted image 20240823165154.png]]
>Il primo componente è una resistenza e la sua equazione costitutiva è $V=Ri$, che non contiene derivate o integrali, ed è quindi adinamico.
>Il secondo componente è un induttore e la sua equazione costitutiva è $V= L \frac{\text{d}i}{\text{d} t}$, che contiene una derivata, ed è quindi dinamico.

>[!tip] Tempo-varianti o Tempo-invarianti 
>Un bipolo è tempo-variante se la sua equazione costitutiva cambia nel tempo. Viceversa un bipolo è tempo-invariante se la sua equazione costitutiva non cambia nel tempo.

>[!example]
>![[Pasted image 20240823165711.png]]
>Il primo componente è un induttore e la sua equazione costitutiva è $V=L \frac{\text{d} i}{\text{d}t}$, che non varia nel tempo, ed è quindi tempo-invariante.
>Il secondo componente è un potenziometro e la sua equazione costitutiva è $V=R(t)i$, che varia nel tempo, ed è quindi tempo-variante.

>[!tip] Linearità o Non Linearità
>Un bipolo è lineare se, data la sua equazione costitutiva $v=f(i)$, vale la seguente equazione: $$f(\alpha i_{1}+ \beta i_{2})= \alpha f(i_{1})+ \beta f(i_{2})= \alpha v_{1}+ \beta v_{2}$$Viceversa se non vale l'equazione un bipolo è detto non lineare.

>[!example]
>L'equazione di un resistore è $V=Ri$, poniamo quindi $i= \alpha i_{1} + \beta i_{2}$:
>$$V = R( \alpha i_{1} +\beta i_{2})= \alpha R i_{1} + \beta R i_{2} = \alpha v_{1} + \beta v_{2}$$
>Di conseguenza è un bipolo lineare.
>Viceversa, se avessimo un bipolo con equazione costitutiva $V=k i^{2}$, potremmo dire che non è lineare.

>[!tip] Classificazione in termini energetici
>In base alla potenza assorbita possiamo dire che un bipolo è:
>- Inerte se $p_{a}(t)\equiv0$
>- Passivo se $p_{a}(t)\geq0$
>- Attivo se $p_{a}(t)\in\mathbb{R}$

### Bipoli notevoli
>[!tip] Resistore lineare
>![[Pasted image 20240823172922.png]]
>
>| $$\text{Equazione costitutiva}$$ | $$V=Ri\iff i= \frac{V}{R}= Gs$$                            |
>| - | - |
>| $$\text{Caratteristiche}$$       | $$\begin{align*}&\text{adinamico}\\&\text{lineare}\\&\text{tempo-invariante}\\&\text{passivo}\end{align*}$$ |
>| $$\text{Base tensione}$$         | $$\checkmark$$                                                                                           |
>| $$\text{Base corrente}$$         | $$\checkmark$$                                                                                           |
>| $$\text{Potenza}$$               | $$p_{a}= Vi= Ri^{2}= \frac{V^{2}}{R}$$                                                                   |

>[!tip] Corto circuito
>![[Pasted image 20240823174045.png]]
>
>| $$\text{Equazione costitutiva}$$ | $$V=0$$                            |
>| - | - |
>| $$\text{Caratteristiche}$$       | $$\begin{align*}&\text{adinamico}\\&\text{lineare}\\&\text{tempo-invariante}\\&\text{inerte}\end{align*}$$ |
>| $$\text{Base tensione}$$         | $$\times$$                                                                                           |
>| $$\text{Base corrente}$$         | $$\checkmark$$                                                                                           |
>| $$\text{Potenza}$$               | $$p_{a}= Vi= 0$$                                                                   |

>[!tip] Circuito aperto
>![[Pasted image 20240823174318.png]]
>
>| $$\text{Equazione costitutiva}$$ | $$i=0$$                            |
>| - | - |
>| $$\text{Caratteristiche}$$       | $$\begin{align*}&\text{adinamico}\\&\text{lineare}\\&\text{tempo-invariante}\\&\text{inerte}\end{align*}$$ |
>| $$\text{Base tensione}$$         | $$\checkmark$$                                                                                           |
>| $$\text{Base corrente}$$         | $$\times$$                                                                                           |
>| $$\text{Potenza}$$               | $$p_{a}= Vi= 0$$                                                                   |

>[!tip] Generatore indipendente di tensione
>![[Pasted image 20240823174724.png]]
>
>| $$\text{Equazione costitutiva}$$ | $$V=e(t)$$                            |
>| - | - |
>| $$\text{Caratteristiche}$$       | $$\begin{align*}&\text{adinamico}\\&\text{lineare se }e(t)=0\text{, non lineare se }e(t)\neq0\\&\text{tempo-variante}\\&\text{attivo}\end{align*}$$ |
>| $$\text{Base tensione}$$         | $$\times$$                                                                                           |
>| $$\text{Base corrente}$$         | $$\checkmark$$                                                                                           |
>| $$\text{Potenza}$$               | $$p_{a}= e(t)i(t)\in\mathbb{R}$$                                                                   |

>[!tip] Generatore indipendente di corrente
>![[Pasted image 20240823175125.png]]
>
>| $$\text{Equazione costitutiva}$$ | $$i=a(t)$$                            |
>| - | - |
>| $$\text{Caratteristiche}$$       | $$\begin{align*}&\text{adinamico}\\&\text{lineare se }e(t)=0\text{, non lineare se }e(t)\neq0\\&\text{tempo-variante}\\&\text{attivo}\end{align*}$$ |
>| $$\text{Base tensione}$$         | $$\checkmark$$                                                                                           |
>| $$\text{Base corrente}$$         | $$\times$$                                                                                           |
>| $$\text{Potenza}$$               | $$p_{a}= V(t)a(t)\in\mathbb{R}$$                                                                   |

### Principio di equivalenza
>[!note]
>Due bipoli si dicono equivalenti se le loro equazioni costitutive coincidono.