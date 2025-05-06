>[!note]
>Per riportare sul dominio dei fasori tutti i risultati visti in precedenza è necessario:
>1. Sostituire ad ogni grandezza elettrica il corrispondente fasore.
>2. Associare a ciascun componente la corrispondente impedenza (o ammettenza)

### Collegamento in serie di impedenze
>[!note]
>Siano $n$ impedenze connesse in serie, attraversate da una corrente $\overline{i}$ e aventi tensione totale $\overline{V}$. Si ha che l'impedenza equivalente è calcolata come: $$z= \sum\limits_{k=1}^{n}z_{k}$$
>Per quanto riguarda al partitore di tensione, si ha che: $$\overline{V}_{i}= \frac{z_{i}}{z}\overline{V}$$

### Collegamento in parallelo di impedenze
>[!note]
>Siano $n$ ammettenze connesse in parallelo, attraversate da una corrente totale $\overline{i}$ e aventi tensione $\overline{i}$. Si ha che l'ammettenza totale equivalente è calcolata come: $$y= \sum\limits_{k=1}^{n}y_{k}$$
>Per quanto riguarda al partitore di corrente, si ha che: $$\overline{i}_{i}= \frac{y_{i}}{y} \overline{i}$$

### Equivalenti di Thevenin e Norton
>[!note]
>Si ha che l'equivalente di Thevenin ha come equazioni costitutive:
>![[Pasted image 20250410145652.png|center]]
>$$\overline{V}=z_{\text{TH}}\overline{i}+\overline{e}_{\text{TH}}$$
>Analogamente, l'equivalente di Norton ha come equazioni costitutive:
>![[Pasted image 20250410145901.png|center]]
>$$\overline{i}=y_\text{NR}\overline{V}+\overline{a}_{\text{NR}}$$

### Doppi bipoli
>[!note]
>Si ha che le matrici ibride, di trasmissione e trasmissione inversa ($H$, $H'$, $T$, $T'$) mantengono il loro nome. Al contrario, le matrici di resistenza $R$ e conduttanza $G$ diventano rispettivamente matrici di impedenza $Z$ e ammettenza $Y$.

### Funzioni di rete
>[!note]
>In generale, una funzione di rete è un rapporto ingresso-uscita tra 2 grandezze fasoriali.