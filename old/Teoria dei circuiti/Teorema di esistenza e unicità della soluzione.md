>[!note]
>Consideriamo un circuito con $n$ nodi e $l$ lati. Consideriamo quindi il numero di incognite $2l+n-1$, le relative equazioni di Tableau: $$\begin{cases}
A\overrightarrow{i}=\overrightarrow{0}&n-1 &\text{KCL} \\
A^{T}\space\overrightarrow{u}-\overrightarrow{V}=\overrightarrow{0}& l & \text{KVL-I}
\end{cases}$$
>Scriviamo le $l$ equazioni costitutive dei componenti nel seguente modo:
>$$M_{j}\overrightarrow{v}_{j}+N_{j}\overrightarrow{i}_{j}=\overrightarrow{z}_{j}$$
>Dove $\overrightarrow{v}$ sono le tensioni descrittive del componente $j$, $\overrightarrow{i}$ sono le correnti descrittive del componente $j$ e $\overrightarrow{z}$ sono i termini noti descrittivi del componente $j$.
>>[!example]
>>Nel caso del resistore: $$V=Ri\iff V-Ri=0\Longrightarrow$$
>>$$(1)V+ (-R)i= (0)$$
>
>>[!example]
>>Nel caso del generatore di tensione: $$v(t)=e(t)\Longrightarrow$$
>>$$(1)V+(0)i=(e)$$
>
>>[!example]
>>Nel caso di un generatore di corrente pilotato in tensione: $$\begin{cases}
>>i_{1}= gv_{2} \\
i_{2}=0
\end{cases}\Longrightarrow $$
$$\begin{pmatrix}0&-g\\0&0\end{pmatrix}\begin{pmatrix}V_{1} \\ V_{2}\end{pmatrix}+\begin{pmatrix}1&0\\0&1\end{pmatrix}\begin{pmatrix}i_{1} \\ i_{2}\end{pmatrix}=\begin{pmatrix}0\\0\end{pmatrix}$$
>
>Consideriamo adesso il sistema di equazioni contenente tutte le $l$ equazioni costitutive del circuito: $$M(t)\overrightarrow{v}+N(t)\overrightarrow{i}=\overrightarrow{0}$$
>Dove le matrici $M(t)$ e $N(t)$ sono matrici diagonali a blocchi.
>
>>[!example]
>>![[Pasted image 20240829092700.png]]
>>$$\begin{cases}
v_{1}=E \\
i_{2}=0 \\
i_{3}=gv_{2} \\
v_{4}=Ri_{4}
\end{cases}\Longrightarrow$$
$$\begin{pmatrix}1&0&0&0\\0&0&0&0\\0&-g&0&0\\0&0&0&1\end{pmatrix}\begin{pmatrix}v_{1}\\v_{2}\\v_{3}\\v_{4}\end{pmatrix}+\begin{pmatrix}0&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&-R\end{pmatrix}\begin{pmatrix}i_{1}\\i_{2}\\i_{3}\\i_{4}\end{pmatrix}=\begin{pmatrix}E\\0\\0\\0\end{pmatrix}$$
>
>Aggiungiamo le $l$ equazioni di costitutive alle equazioni di Tableau:
>$$\begin{cases}
A\overrightarrow{i}=\overrightarrow{0} \\
A^{T}\space\overrightarrow{u}-\overrightarrow{v}=\overrightarrow{0} \\
M(t)\overrightarrow{v}+N(t)\overrightarrow{i}=\overrightarrow{z}
\end{cases}$$
>Raccogliendo tutte le incognite in un unico vettore:
>$$\overrightarrow{w}=\begin{pmatrix}\overrightarrow{u}\\\overrightarrow{v}\\\overrightarrow{i}\end{pmatrix}\Longrightarrow\begin{pmatrix}\mathbb{0}&\mathbb{0}&A\\-A^{T}&\mathbb{1}&\mathbb{0}\\\mathbb{0}&M(t)&N(t)\end{pmatrix}\begin{pmatrix}\overrightarrow{u}\\\overrightarrow{v}\\\overrightarrow{i}\end{pmatrix}=\begin{pmatrix}\overrightarrow{0}\\\overrightarrow{0}\\\overrightarrow{z}\end{pmatrix}\iff T(t)\overrightarrow{w}(t)=\overrightarrow{y}(t)$$
>Questo è definito sistema risolutivo del circuito. La soluzione del circuito è definita come: $$\overrightarrow{w}(t)=T^{-1}(t)\overrightarrow{y}(t)$$
>
>Il teorema di esistenza e unicità afferma che la soluzione del circuito esiste ed è unica se e solo se: $$\det(T(t))\neq0$$


