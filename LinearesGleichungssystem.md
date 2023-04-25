### Lineares Gleichungssystem

#### Schreibweise als Matrix

$\begin{matrix}     a_{11}x_1 & + & \cdots &+ &a_{1n}x_n & = & b_{1}\\     \vdots & + & \ddots &+ &\vdots &= &\vdots\\     a_{m1}x_n & + & \cdots &+ &a_{mn}x_{n} & = & b_{m} \end{matrix}\quad\Rightarrow\quad  \underbrace{\left(\begin{array}{ccc|c}     a_{11} &\cdots &a_{1n} & b_{1}\\     \vdots & \ddots & \vdots & \vdots\\     a_{m1} &\cdots &a_{mn} & b_{m} \end{array}\right)}_{\left(M|b\right)}$

<br>

#### Umformen in Zeilenstufenform

>[!NOTE] Definition elementarer Zeilenumformungen
>
>- Vertauschen zweier Zeilen
>- Multiplikation einer Zeile mit einem Skalar $\lambda\not = 0$
>- Addition des $\lambda$-fachen einer Zeile zu einer anderen 

<br>

$$\underbrace{\left(\begin{array}{cccc|c}     
	* &\cdots & \cdots & \cdots & *\\
	0 & * & \cdots & \cdots & \vdots \\
	0 & 0 & * & \cdots & \vdots \\
	\vdots & \vdots & \vdots & \vdots & \vdots \\
	0 & 0 & 0 & 0 & *
\end{array}\right)}_\text{Zeilenstufenform}$$

Falls die letzte $0$-Zeile für ihr $b\not =0$ ist $\Rightarrow$ LGS unlösbar

<br>

#### Lösen eines LGS

1. in ZSF bringen 
2. rekursives Einsetzen und Lösen der Gleichungen beginnend bei $x_m$ bis $x_1$

Endergebnisse:

- eine Lösung $\Rightarrow$ genaue ZSF ohne Sprünge
- unendlich viele Lösungen $\Rightarrow$ ZSF mit mindestens einem Sprung
- keine Lösung $\Rightarrow$ ZSF Nullreihe muss $b=0$ haben

<br>

### Rang einer Matrix

>[!NOTE] Definition
>
>Matrix auf Zeilenstufenform bringen $\Rightarrow$ Anzahl der nicht $0$-Zeilen = $rg(M)$
>
>- es gibt den Zeilenrang (Rang der Zeile)
>- es gibt den Spaltenrang (Rang der Spalten)

<br>

Das Kriterium der Lösbarkeit:

- LGS lösbar $\Leftrightarrow rg(M)=rg(M|b)$
- das LGS ist lösbar $\Rightarrow$ Anzahl frei wählbarer Variablen $:= \#\text{Variablen}-rg(M)$
- $(M|b)$ eindeutig lösbar $\Leftrightarrow\exists_1\text{ lsg}\Leftrightarrow rg(M)=n$ mit $\mathbb{R}^n$
- falls $\exists{\ge 1}:$
	- anstatt z.B. zu schreiben $x_3=\frac{1}{2}x_4$
	- setzen wir z.B. $\lambda=x_4\Rightarrow x_3=\frac{1}{2}\lambda$


<br>

### Besondere Matrizen

- Spaltenvektor: $m\times 1:S=\begin{pmatrix}S_1\\\vdots \\ S_m\end{pmatrix}$
- Zeilenvektor: $1\times n: Z=\begin{pmatrix}Z_1 & \cdots & Z_n\end{pmatrix}$
- Nullmatrix: Jeder Eintrag ist $0$
- Quadratische Matrix $\Leftrightarrow m=n$
- Einheitsmatrix $E_n,\ n=m$ 
- Diagonalmatrix: $diag(\lambda_1\cdots\lambda_n)=\begin{pmatrix}\lambda_1 & 0 & \cdots  & \cdots\\ 0 & \lambda_2 & \cdots & 0\\\vdots & \vdots & \ddots & \vdots\\ 0 & 0 & \cdots & \lambda_n\end{pmatrix}$
- Obere- und Untere-$\Delta$-Matrix

<br>

#### Permutationsmatrizen

>[!NOTE] Definition
>
>Der Vertausch von Zeilen tritt auf indem man eine Matrix $M$ mit einer Permutationsmatrix $P$ multipliziert.
>
>- jede Zeile der Matrix $P$ kann nur eine $1$ enthalten
>- die Stelle dieser $1$ besagt wohin diese Zeile permutiert / verschoben wird

<br>

### Rechenoperationen

- $A+B:=\forall a_{ij},b_{ij}:(a_{ij}+b_{ij})_{mn}$
- $\lambda A:=\forall a_{ij}:(\lambda a_{ij})_{mn}$

<br>

#### Transponieren

>[!NOTE] Definition
>
$A=\begin{pmatrix}a_{11} & \cdots & a_{1n}\\\vdots & \ddots & \vdots \\ a_{m1} & \cdots & a_{mn}\end{pmatrix}\quad\Rightarrow\quad A^T=\begin{pmatrix}a_{11} & \cdots & a_{m1}\\\vdots & \ddots & \vdots \\ a_{1n} & \cdots & a_{mn}\end{pmatrix}$

<br>

#### Multiplikation

>[!NOTE] Definition
>
>$Z=\begin{pmatrix}Z_1 & \cdots & Z_n\end{pmatrix},\ S=\begin{pmatrix}S_1\\\vdots \\ S_m\end{pmatrix}\quad\Rightarrow\quad Z\cdot S:=\sum_{i=1}^nZ_iS_i$
>
>- $A\cdot B\not =B\cdot A\Rightarrow$ nicht Kommutativ
>- $A^0=E_n$

<br>

#### Invertieren

>[!NOTE] Definition
>
>$(A|E_n)\Rightarrow\text{ durch Zeilenstufenform Umformungen }\Rightarrow (E_n|A^{-1})$
>
>- Eine Matrix ist invertierbar $\Leftrightarrow$ alle Vektoren der Matrix linear unabhängig sind $\Leftrightarrow$ der Rang der Matrix voll ist
>- $A\cdot A^{-1}=E_n=A^{-1}\cdot A$
>- $A-A^{-1}=0$
