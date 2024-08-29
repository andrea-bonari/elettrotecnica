>[!note]
>Consideriamo un circuito con $n$ nodi e $l$ lati. Consideriamo quindi il numero di incognite $2l+n-1$, le relative equazioni di Tableau: $$\begin{cases}
A\overrightarrow{i}=\overrightarrow{0}&n-1 &\text{KCL} \\
A^{T}\space\overrightarrow{u}-\overrightarrow{V}=\overrightarrow{0}& l & \text{KVL-I}
\end{cases}$$
>Scriviamo le $l$ equazioni costitutive dei componenti nel seguente modo:
>$$M_{j}\overrightarrow{v}_{j}+N_{j}\overrightarrow{i}_{j}=\overrightarrow{z}_{j}$$
>Dove $\overrightarrow{v}$ sono le tensioni descrittive del componente $j$, $\overrightarrow{i}$ sono le correnti descrittive del componente $j$ e $\overrightarrow{z}$ sono i termini noti descrittivi del componente $j$.

>[!example]
>Nel caso del resistore: $$V=Ri\iff V-Ri=0\Longrightarrow$$
>$$(1)V+ (-R)i= (0)$$

>[!example]
>Nel caso del generatore di tensione: $$v(t)=e(t)\Longrightarrow$$
>$$(1)V+(0)i=(e)$$

>[!example]
>Nel caso di un generatore di corrente pilotato in tensione: $$\begin{cases}
i_{1}= gv_{2} \\
i_{2}=0
\end{cases}\Longrightarrow $$
$$\begin{pmatrix}0&-g\\0&0\end{pmatrix}\begin{pmatrix}V_{1} \\ V_{2}\end{pmatrix}+\begin{pmatrix}1&0\\0&1\end{pmatrix}\begin{pmatrix}i_{1} \\ i_{2}\end{pmatrix}=\begin{pmatrix}0\\0\end{pmatrix}$$

