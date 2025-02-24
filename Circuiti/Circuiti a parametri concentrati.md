>[!note]
>In circuito a parametri concentrati, anche detto LUMP Circuit Model, si assume che la propagazione dei segnali è istantanea. È un approssimazione valida se: $$L_{C}<<\lambda$$
>Dove $L_{C}$ è la lunghezza caratteristica del circuito, e $\lambda= \frac{c}{f}$ è la lunghezza d'onda dei segnali presenti nel circuito.

### Componenti
>[!note]
>Definiamo un componente come modello di un sistema fisico. Di seguito la rappresentazione di un componente:
>![[Pasted image 20250224165223.png]]
>><span style="color: lightgreen;">■</span> superficie limite
>><span style="color: yellow;">■</span> morsetto
>><span style="color: aqua;">■</span> terminale
>><span style="color: purple;">■</span> polo (morsetto + terminale)
>
>In base al numero di poli il componente si classifica come $n$-polo.

Utilizziamo tensioni e correnti come variabili descrittive. Per descrivere in maniera esaustiva un $n$-polo sono sufficienti $2\cdot(n-1)$ variabili descrittive ($n-1$ correnti e $n-1$ tensioni), e un legame tra loro, quindi $n-1$ equazioni costitutive.

### Risoluzione di un circuito
>[!note]
>Per risolvere un circuito di $n$ variabili descrittive, sono necessarie $n$ equazioni costitutive. $\frac{n}{2}$ sono date dalle equazioni costitutive dei componenti, mentre $\frac{n}{2}$ equazioni costitutive sono date dalle leggi di Kirchhoff.
>