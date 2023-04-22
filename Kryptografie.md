## Vorwort

### Sichere Primzahl

>[!NOTE] Definition
>
>Sei $p\in P$, dann gilt:
>$$\frac{p-1}{2}\in P\Rightarrow\text{ sichere Primzahl}$$

<br>

## Pohlig Hellman Verfahren

>[!NOTE] Definition
>
>- $p=(\text{große})\text{ Primzahl}$
>- $N=\text{Klartext mit}\in\mathbb{Z}^\times_p$
>- $e,d=\text{Schlüssel}$
>
>1. Wähle $e\in\mathbb{N}$ mit $ggT(e,p-1)=1$
>
>2. Bestimme $d$ mit:
>
>$$ed\hspace{0.5cm}\equiv\hspace{0.5cm}1\text{ mod }p-1$$
>$$\hspace{0.4cm}ed\hspace{0.5cm}=\hspace{0.5cm}1+r\cdot (p-1)$$
>$$\hspace{0.9cm}1\hspace{0.5cm}=\hspace{0.5cm}ed-r\cdot (p-1)$$
>
>Verschlüsseln:
>$$C=N^e$$
>
>Entschlüsseln:
>$$C^d=(N^e)^d=N^{e\cdot d}=N^{1+r\cdot (p-1)}=N\cdot (N^{p-1})^r=N$$
>
>Für den letzten Schritt wird der Satz von Euler-Fermat verwendet.

<br>

## RSA-Verfahren

>[!NOTE] Definition
>
>Vorbereiten durch den Empfänger. Dieser erzeugt den Schlüssel und teilt ihn öffentlich.
>
>1. wähle große $p,q\in\mathbb{P}:p\not = q$ und $p\pm 1,q\pm 1$ müssen große Primteiler haben
>2. setze $n=p\cdot q$
>3. $|\mathbb{Z}^\times_n|=\varphi(n)=\varphi(p\cdot q)$
>4. wähle $e\in\{1,...,n\}:ggT(e\varphi(n))=1$
>5. berechne $d:e\cdot d\equiv_{\varphi(n)}1$
>6. veröffentliche Schlüssel $(n,e)$
>
>Verschlüsselung des Senders:
>  $$C\equiv_nN^e$$
>  
>Entschlüsselung des Empfängers:
>  $$N\equiv_nC^d$$
