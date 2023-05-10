### Gruppen

>[!NOTE] Definition
>
>Eine Gruppe $G$ ist eine nichtleere Menge mit innerer Verknüpfung.
>$(G,\cdot)$ heißt Gruppe, wenn:
>
>1. Abgeschlossenheit: $\forall a,b\in G: a\cdot b\in G$
>2. Assoziativ: $\forall a,b,c\in G: (a\cdot b)\cdot c = a\cdot (b\cdot c)$
>3. Neutrales Element: $\forall a\in G:\exists e\in G: a\cdot e= a = e\cdot a$
>4. Inverses Element: $\forall a\in G\exists_1 b\in G: a\cdot b = e = b\cdot a$
>   
>Die Gruppe heißt zudem abelsch, wenn:
>
>5. Kommutativ: $\forall a,b\in G: a\cdot b = b\cdot a$

<br>

### Unterguppen

>[!NOTE] Definition
>
>Sei $(G,\cdot )$ eine Gruppe mit dem neutralen Element $e$, dann gilt $U\subseteq G$ mit
>
>- $e\in U$
>- Abgeschlossenheit: $\forall u,v\in U: u\cdot v\in U$
>- Inverses Element: $\forall u\in U: u^{-1}\in U$
>
>so ist $U$ eine Untergruppe von $G$ und zugleich $|U|\le |G|$

<br>

### Zyklische Gruppen

>[!NOTE] Definition
>
>$\langle a\rangle =\{a^k\ |\ a\in G,\ k\in\mathbb{Z}\}$
>
>- $e\in\langle a\rangle$
>- Abgeschlossenheit: $a^k,a^l\in\langle a\rangle:a_k\cdot a_l=a^{k+l}\in\langle a\rangle$
>- Inverses Element: $a^k\in\langle a\rangle\exists a^{-k}:a^k\cdot a^{-k}=a^0=e=a^{-k}\cdot a^k$

<br>

### Ordnung eines Elements

>[!NOTE] Definition
>
>$O(a)=|\langle a\rangle|\Rightarrow$ kleinste Zahl mit $a^n=e$
>
>Man nehme ein beliebiges Element $e$ aus einer Gruppe $G$. So gilt, falls $e^{\text{Produkte der Teiler von }\varphi (|G|)}\not\equiv_{|G|} 1\Leftrightarrow e$ ist ein Erzeuger.
>
>---
>
>$$\forall a\in (K^{n\times n})^\times:\exists_1 a^{-1}\Rightarrow O(a)=O(a^{-1})=n^2$$

<br>

#### Satz von Lagrange

>[!NOTE] Definition
>
>Sei $G$ eine endliche Gruppe und $U\subseteq G$, dann gilt:
>$$|U|\Big||G|$$
>
>Somit muss die Mächtigkeit einer beliebigen Untergruppe ihre Obergruppe immer teilen.

<br>

#### Eulersche Phi-Funktion

>[!NOTE] Definition
>
>Die eulersche Phi-Funktion gibt an wie viele zu $n$ teilerfremde positive natürliche Zahlen es gibt, die nicht größer als $n$ sind:
>$$\varphi (n):=|\{a\in\mathbb{N}\ |\ 1\le a\le n\wedge ggT(a,n)=1\}|$$
>
>- $\varphi (m\cdot n)=\varphi (m)\cdot\varphi (n)$
>- $\forall p\in\mathbb{P}:\varphi (p)=p-1$
>- $\forall p\in\mathbb{P}:\varphi (p^k)=p^k-p{k-1}$

<br>

### Restklassen

>[!NOTE] Definition
>
>$\overline a=\{a+m\mathbb{Z}\ |\ m\in\mathbb{N}, a\in\mathbb{Z}\}$ beschreibt die Restklasse von $a\text{ mod } m$
>
>Menge der Restklassen: $\mathbb{Z}\Big|n\mathbb{Z}=\mathbb{Z}\Big|n=\mathbb{Z}_n=\{\overline0,...,\overline{n-1}\}\Rightarrow|\mathbb{Z}_n|=n$

<br>

#### Satz von Euler

>[!NOTE] Definition
>
>$$a^{\varphi(n)}\equiv_n1\Leftrightarrow ggT(a,n)=1,\hspace{0.5cm}a,n\in\mathbb{N}$$

<br>

#### Kleiner Satz von Fermat

>[!NOTE] Definition
>
>Es sei $p\in\mathbb{P}$. Dann gilt:
>$$\forall a\in\mathbb{Z}:a^p\equiv_pa$$
>
>Weiterhin gilt, falls $ggT(a,p)=1$:
>$$\forall a\in\mathbb{Z}:a^{p-1}\equiv_p1$$

<br>

### Ringe

>[!NOTE] Definition
>
>Eine Menge $R$ mit zwei Verknüpfungen $+$ und $\cdot$ heißt Ringt, wenn:
>
>1. $(R,+)$ ist eine abelsche Gruppe
>2. $\cdot$ ist assoziativ
>3. Distributiv: $\forall a,b,c\in R: a(b+c)=ab+bc$ und $(a+b)c=ac+bc$
>4. Neutrales Element: $forall a\in R: a\cdot e=a=e\cdot a$

<br>

#### Einheitengruppe

>[!NOTE] Definition
>
>Gegeben sei ein Ring $(R,+,\cdot)$. So gilt:
>$$R^\times=\{a\in R\ |\ \forall a\ \exists a^{-1}\in R^\times\}$$
>
>Somit ist $R^\times$ die Einheitengruppe von $R$.

<br>

### Prime Restklassengruppen

>[!NOTE] Definition
>
>Die Restklasse enthält nur die koprimen Reste $\Rightarrow$ alle Elemente der Menge sind teilerfremd zu $n$
>
>$n\in\mathbb{N}\rightarrow\mathbb{Z}^\times_n\hspace{0.5cm}=\hspace{0.5cm}\{\overline a\text{ ist invertierbar}\}$
>$\hspace{3.225cm}=\hspace{0.5cm}\{\overline a\in\mathbb{Z}_n\ |\ \exists j\in\mathbb{Z}_n:\overline aj=1\}$
>$\hspace{3.225cm}=\hspace{0.5cm}\{\overline a\in\mathbb{Z}_n\ |\ ggt(a,n)=1\}$
>

<br>

#### Eigenschaften

- $(\mathbb{Z}_n,+,\cdot)$ ist ein Körper $\Leftrightarrow n\in\mathbb{P}$
- $\overline a$ ist invertierbar

<br>

### Erweiterter Euklidischer Algorithmus

>[!NOTE] Definition
>
>Der EEA dient zur rekursiven Berechnung des ggT zweier Zahlen ohne Kenntnis ihrer Primfaktorzerlegung.
>
>Der $ggT$ von $a$ und $b$ enspricht:
>$$a\cdot\alpha + b\cdot\beta = ggT(a,b)$$

<br>

#### Berechnung

- gegeben $1\le a\le b$ aus $\mathbb{N}$
- falls $(b\ mod\ a)=0$ gib $\alpha =1,\beta =0$ zurück
- sonst berechne rekursiv $\alpha ',\beta '$ mit:
	- $ggT(b\ mod\ a, a)=(b\ mod\ a)\cdot\alpha '+\alpha\cdot\beta '$
	- gebe $\alpha =(\beta '-\lfloor\frac{b}{a}\rfloor\cdot\alpha ')$ und $\beta =\alpha '$ zurück

<br>

>[!EXAMPLE] Beispiel
>
>$a=5, b=911\rightarrow$ gesucht: $ggT(5,911)$
>
>| $a$ | $b$ | $\lfloor\frac{b}{a}\rfloor$ | $\alpha$ | $\beta$ |
>|---:|---:|---:|---:|---:|
>| 5 | 911 | 182 | -182 | 1 |
>| 1 | 5 | - | 1 | 0 |
>
>Somit folgt: $ggT(5,911)=5\cdot (-182)+911\cdot 1$
