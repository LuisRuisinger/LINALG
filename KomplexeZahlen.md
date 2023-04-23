>[!NOTE] Definition
>
>$\mathbb{C}=\{z\ |\ z = a+ib\text{ mit } a,b\in\mathbb{R}\}$
>
>Kann beschrieben werden durch Vektor des $\mathbb{R}^2$:
>- $(a,b)\equiv a+ib$
>- $(a,0)=a,\ (0,b)=b$
>- $(0,1)=i$
>- $(0,1)^2=-1$
>- jeder Vektor des $\mathbb{R}^2$ hat ein multiplikatives Inverses $\Leftrightarrow (a,b)\not =0$
>- $(\mathbb{R},\cdot ,+)$ ist ein Körper

<br>

### Eigenschaften

- $a=Re(z)$
- $b=Im(z)$
- $a=0\Rightarrow z$ ist rein imaginär
- $\overline z$ ist die zu $z$ konjugierte komplexe Zahl:
	- $z=a+ib$
	- $\overline z=a-ib$

<br>

### Rechenoperationen

- $z_1+z_2:=a_1+a_2+i(b_1+b_2)$ analog dazu die Subtraktion
- $z_1\cdot z_2:=a_1b_2-b_1b_2+i(a_1b_2+b_1a_2)$
- $\frac{z_1}{z_2}=\frac{z_1}{z_2}\cdot\frac{z_2}{z_2}=\frac{a_1a_2+b_1b_2+i(b_1a_2-a_1b_2)}{a^2_2+b^2_2}$
- $z\cdot\overline z=a^2+b^2$
- $|z|=\sqrt{a^2+b^2}$
- $\overline{z_1+z_2}=\overline z_1+\overline z_2$ analog dazu alle Rechenoperationen
- $Re(z)=\frac{1}{2}\cdot (z+\overline z)$
- $Im(z)=\frac{1}{2i}\cdot (z-\overline z)$
- Dreiecksgleichung: $|z_1+z_2|\le |z_1|+|z_2|,\ z_1,z_2\in\mathbb{C}$

<br>

### Fundamentalsatz der Algebra

>[!NOTE] Definition
>
>Es sei $P(z)0\sum_{k=0}^na_k\cdot z^k$ ein Polynom vom Grad $deg(P)=:n\in\mathbb{N}$
>
>- nicht konstantes Polynome
>- komplexe Nullstellen $a_k\in\mathbb{C}$
>  
>Das Polynom muss gleich dem Grad Anzahl viele Nullstellen haben. Diese sind komplex. Die komplexen Zahlen sind abgeschlossen.

<br>

### Polarkoordinaten

>[!NOTE] Definition
>
>$z=\{r(cos\varphi +i\cdot cos\varphi )\ |\text{ Radius } r\in\mathbb{R},\varphi\in [-\pi ,\pi]\}$

<br>

#### Umrechnung

- $r:=|z|$
- $\varphi =\begin{cases}arccos\frac{a}{r},\ b\ge 0\\ arccos\frac{a}{r},\text{ sonst}\end{cases}$
- $cos\varphi =\frac{a}{r}$
- $sin\varphi =\frac{b}{r}$

<br>

#### Allg. Rechenoperationen

- Addition und Subtraktion trivial
- $z_1\cdot z_2:=r_1r_2(cos(\varphi_1+\varphi_2)+i\cdot sin(\varphi_1+\varphi_2))$
- $z^n:=r^n(cos(n\cdot\varphi)+i\cdot sin(n\cdot\varphi))$

<br>

#### Rechenoperationen bezogen auf Wurzelziehungen

Allg. $0$-te Wurzel ist nicht definiert

- $\sqrt[n]z\Rightarrow n$ Lösungen
- $z_k:=\sqrt[n]r(cos(\frac{\varphi+2\pi\cdot k}{n})+i\cdot sin(\frac{\varphi+2\pi\cdot k}{n}))$ beschreibt die $k$-te Lösung der Wurzel von $n$ mit $k\in\{0,...,n-1\}$
