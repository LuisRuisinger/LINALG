>[!NOTE] Definition
>
>Ein Ring $(K,+,\cdot)$ mit folgenden Eigenschaften heißt $K$-Vektorraum:
>
>1. $K$ ist kommutativ
>2. $\exists$ neutrales Element (hier: Einselement $1$)$:1\cdot\lambda=\lambda=\lambda\cdot 1\hspace{0.5cm}\forall\lambda\in K$
>3. Jedes $\lambda\not =0$ ist invertierbar $\Leftrightarrow K^\times=K\setminus\{0\}$
>
>Für $\lambda,\mu\in K,\ \forall u,v,w\in V:$
>
>- $v+w\in V,\ \lambda\cdot v\in V$
>- $u+(v+w)=(u+v)+w$
>- $\exists 0\in V:0+v=v$
>- $\exists v'\in V:v+v'=0$
>- $u+v=v+u$
>- $\lambda(u+v)=\lambda u+\lambda v$
>- $(\lambda +\mu)v=\lambda u+\mu u$
>- $(\lambda\mu)v=\lambda(\mu v)$
>- $1v=v=v1$

<br>

## Untervektorraum

>[!NOTE] Definition
>
>Sei $V$ ein $K$-Vektorraum. $U\subseteq V$ heißt Untervektorraum, falls $U$ wieder ein Vektorraum ist und alle Elemente innerhalb von $U$ in $V$ liegen:
>
>1. $1\in U$
>2. $u,v\in U\Rightarrow u+v\in U$
>3. $\lambda\in K,\ u\in U\Rightarrow \lambda u\in U$
>
>Automatisch folgt: $|U|\le |V|$

<br>

## Linearkombinationen

>[!NOTE] Definition
>
>- $\{v_1,...,v_n\}\in V$
>- $\{\lambda_1,...,\lambda_n\}\in K$
>
>Es lassen sich lineare Kombinationen aus beiden Mengen bilden. Das Resultat ist der neue $K$-Vektorraum $v\in V$:
>$$v=\sum^n_{i=1}\lambda_iv_i$$


### Erzeugnis

>[!NOTE] Definition
>
>Es ist gegeben $V$ ein $K$-Vektorraum. Wir entnehmen einen Vektorraum $X\subseteq V$. So setze:
>
>$\langle X\rangle =lin(X)$
>$\hspace{0.91cm}=span(X)$
>$\hspace{0.91cm}=\Big\{\sum^n_{i=1}\lambda_iv_i\|\ \lambda_i\in K,\ v_i\in X,\ n\in\mathbb{N}\Big\}$
>$\hspace{0.91cm}=\text{Menge aller endlichen Linearkombinationen von Elementen aus }X$
>$\hspace{0.91cm}=\text{Erzeugnis aus }X$
>$\hspace{0.91cm}=\text{Lineare Hülle von }X$
>
>- nach Definition ist $\langle X\rangle\subseteq V\Leftrightarrow\langle X\rangle$ ist ein Untervektorraum von $V$
>- $X=\emptyset\Rightarrow\langle\emptyset\rangle =\{0\}$

<br>

### Lineare Unabhängigkeit

>[!NOTE] Definition
>
>Es ist gegeben $V$ ein $K-Vektorraum$. $\{v_1,...,v_n\}\in V$ heißen linear unabhängig, falls
>$$\forall v_{\text{chosen}}\in\{v_1,...,v_n\}:\langle v_{\text{chosen}}\rangle\subsetneq\{v_1,...,v_n\}\setminus\{v_{\text{chosen}}\}$$
>
>- dies bedeutet dass kein Vektor ausser der eigene erzeugbar ist durch seinen Span
>- Beweis durch LGS $\Rightarrow\exists_1\text{ Lsg.}\Leftrightarrow v_1,...,v_n$ sind linear unabhängig
>- $rg(V)=\text{Spaltenrang}=\text{Zeilenrang}$

<br>

## Basen

>[!NOTE] Definition
>
>Ist $V$ einer $K$-Vektorraum, so nennt man $B\subseteq V$ eine Basis von $V$, falls
>
>- $B$ ist linear unabhängig (maximal-linear-unabhängige Teilmenge von $V$)
>- $B$ erzeugt $V\Rightarrow\langle B\rangle=V$ (minimales Erzeugendensystem von $V$)

<br>

### Regeln

- jeder $K$-Vektorraum hat mindestens eine Basis
- jede linear unabhängige Menge von $V$ kann man zu einer Basis ergänzen
- jedes Erzeugnendensystem von $V$ kann zu einer Basis verkürzt werden
- jede Basis von $V$ hat die gleiche Mächtigkeit und entspricht $n:=\mathbb{K}^n$
- ist $V$ ein Vektorraum der Dimension $n: dim(V)=n$ sonst $\infty$

<br>

### Folgerungen

$\Rightarrow$ jede linear unabhängige Menge mit $n$ Elementen ist eine Basis
$\Rightarrow$ jedes Erzeugendensystem mit $n$ Elementen ist eine Basis
$\Rightarrow$ mehr als $n$ Vektoren sind immer linear abhängig
$\Rightarrow |U|\le|V|\Leftrightarrow dim(U)\le dim(V)$

<br>

## Kern

>[!NOTE] Definition
>
>Der Kern einer Abbildung dient dazu anzugeben wie stark die Abbildung von der Injektivität abweicht.
>
>- Existenzbeweis des Kerns eines $K$-Vektorraums $V\Leftrightarrow det(V)=0$
>- $dim(Kern(V))=dim(V)-rg(A)$

<br>

### Berechnung

$$V\cdot x=\begin{pmatrix}v_1 & \cdots & v_n\end{pmatrix}\cdot\begin{pmatrix}x_1\\\vdots \\x_m\end{pmatrix}=0\hspace{0.5cm}\Rightarrow\hspace{0.5cm}(V|0)\text{ lösen}\hspace{0.5cm}\Rightarrow\hspace{0.5cm}\text{Kern}(V)$$

<br>

## Bild

>[!NOTE] Definition
>
>Das Bild einer Abbildung beschreibt den möglichen Ergebnisraum dieser Abbildung.
>Gegeben sei ein $K$-Vektorraum $V$. Es gilt:
>$$Bild(V)=\{V\cdot v\ |\ v\in\mathbb{R}^n\}\subseteq\mathbb{R}^m$$

<br>

### Berechnung

$$V\rightarrow V^T\hspace{0.5cm}\Rightarrow\hspace{0.5cm}\text{in ZSF bringen}\hspace{0.5cm}\Rightarrow\hspace{0.5cm}V^T\rightarrow V\hspace{0.5cm}\Rightarrow\hspace{0.5cm}\forall v\in V\setminus\{0_v\}\rightarrow\langle v_1,...,v_n\rangle=:Bild(V)$$

