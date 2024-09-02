### Connessione in serie di doppi bipoli
>[!note]
>Il collegamento in serie è possibile quando il doppio bipolo ammette base corrente.
>![[Pasted image 20240902163019.png]]
>$$\begin{cases}
>i_{1}'=i_{1}''=i_{1} \\
>i_{2}'=i_{2}''=i_{2}
>\end{cases}\qquad \begin{cases}
>v_{1}=v_{1}'+v_{1}'' \\
>v_{2}=v_{2}'+v_{2}''
>\end{cases}$$
>Quindi: $$\begin{pmatrix}v_{1} \\ v_{2}\end{pmatrix}=(R')\begin{pmatrix}i_{1}' \\ i_{2}'\end{pmatrix}+(R'')\begin{pmatrix}i_{1}'' \\ i_{2}''\end{pmatrix}=\left((R')+(R'')\right)\begin{pmatrix}i_{1} \\ i_{2}\end{pmatrix}$$
> ![[Pasted image 20240902163313.png]]

### Connessione in parallelo di doppi bipoli
>[!note]
>La connessione in parallelo di doppi bipoli è possibile quando ammettono base tensione.
>![[Pasted image 20240902163846.png]]
>$$\begin{cases}
>v_{1}'=v_{1}''=v_{1} \\
>v_{2}'=v_{2}''=v_{2}
>\end{cases}\qquad \begin{cases}
>i_{1}=i_{1}'+i_{1}'' \\
>i_{2}=i_{2}'+i_{2}''
>\end{cases}$$
>Quindi:
>$$\begin{pmatrix}i_{1} \\ i_{2}\end{pmatrix}= \begin{pmatrix}i_{1}' \\ i_{2}'\end{pmatrix}+\begin{pmatrix}i_{1}'' \\ i_{2}''\end{pmatrix}=(G')\begin{pmatrix}v_{1}' \\ v_{2}'\end{pmatrix}+(G'')\begin{pmatrix}v_{1}'' \\ v_{2}''\end{pmatrix}=((G')+(G''))\begin{pmatrix}v_{1} \\ v_{2}\end{pmatrix}$$
>![[Pasted image 20240902164157.png]]

### Connessione in cascata di doppi bipoli
>[!note]
>![[Pasted image 20240902164403.png]]
>$$\begin{cases}
>v_{1}''=v_{2}' \\
>i_{1}''=-i_{2}'
>\end{cases}$$
>Quindi:
>$$\begin{pmatrix}v_{1}' \\ i_{1}'\end{pmatrix}=(T')\begin{pmatrix}v_{2}' \\ -i_{2}'\end{pmatrix}=(T')\begin{pmatrix}v_{1}'' \\ i_{1}''\end{pmatrix}=(T')(T'')\begin{pmatrix}v_{2}'' \\ -i_{2}''\end{pmatrix}$$
>![[Pasted image 20240902164742.png]]



