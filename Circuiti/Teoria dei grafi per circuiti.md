>[!note]
>Un grafo è un insieme di nodi e lati. Se i lati sono orientati, si parla di grafo orientato, viceversa di grafo non orientato.

>[!example]
>![[Pasted image 20250225092001.png]]
>><span style="color: yellow;">■</span> Percorso: insieme di lati che collega 2 nodi
>><span style="color: lightgreen;">■</span> Maglia: percorso chiuso
>><span style="color: pink;">■</span> Sottografo: un sottoinsieme di nodi e lati
>><span style="color: aqua;">■</span> Taglio: insieme di lati che, se rimossi, separa il grafo in due sottografi non connessi
>><span style="color: red;">■</span>Albero: percorso non chiuso che collega tutti i nodi del grafo

Ad ogni componente è associato un grafo. Il grafo complessivo di un circuito sarà dato dall'unione dei grafi di tutti i componenti.

### Grafo di un componente
>[!note] 
>Il grafo di un componente si distingue in grafo a stella e non a stella: 
>- Grafo a stella: ha un nodo di riferimento
>- Grafo non a stella: non ha un nodo di riferimento
>  
>Inoltre in base all'orientamento di corrente e tensione, se il grafo è a stella, si possono utilizzare la convenzione degli utilizzatori o dei generatori:
>- Convenzione degli utilizzatori: tensione e corrente in senso discorde
>- Convenzione dei generatori: tensione e corrente in senso concorde

La scelta della convenzione da utilizzare è arbitraria, tuttavia è importante mantenere coerenza. Non è obbligatorio utilizzare la stessa convenzione per tutto il circuito.
