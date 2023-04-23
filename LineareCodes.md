>[!NOTE] Definition
>
>Ein linearer Code besitzt ein Strom an Bits welche Elemente eines endlichdimensionalen Vektorraums $\mathbb{F}^k_2$ über einem endlichen Körper $F_2$ sind
>
>- Bitstrom $x\in K^{k\times 1}$ mit Fehlerwahrscheinlichkeit eines Bits von $P[X]=10^{-6}$
>- Versorgung mit Redundanz $\Rightarrow$ Fehlererkennend / Fehlerkorrigierend
>- Generatormatrix $G\in K^{n\times k}$ schafft Redundanz
>
>Es gilt allgemein
>$$C:=\Big\{G\cdot\begin{pmatrix}x_1\\\vdots \\x_k\end{pmatrix}\ \Big|\ \begin{pmatrix}x_1\\\vdots \\ x_k\end{pmatrix}\in K^k\Big\}\rightarrow\begin{pmatrix}c_1\\\vdots \\ c_n\end{pmatrix}\subseteq K^n,\hspace{0.5cm}k\le n$$
>
>und wird $(n,k)$-Code genannt

<br>

## Eigenschaften

- $n:=$ Länge des Codes
- $n-k=\text{Redundanz}$
- $dim(C)=k$
- $rg(G)=n-k\Leftrightarrow$ voller Rang innerhalb von $G$
- $\frac{k}{n}=\text{Informationsrate}$

<br>

## Besondere Generatormatrizen

### Parity-Check-Matrix

>[!NOTE] Definition
>
>Mithilfe der Parity-Check-Matrix bildet man den Bitstrom $x$ auf einen kodierten Strom $c$ wobei gilt, dass $c_n:=\sum^k_{i=1}x_i$ 
>$$G:=\begin{pmatrix}E_n\\ 1_v\end{pmatrix}:G\cdot x\rightarrow c=\begin{pmatrix}x_1\\\vdots \\ x_k\\ x_1+...+x_k\end{pmatrix}$$
>
>- diese Summe gilt als fehlererkennendender Aspekt eines kodierten Stroms
>- falls Fehler in $c_n$, dann weiß man nichts über die eigentliche Fehlerquelle

<br>

### n-fach Wiederholungscode

>[!NOTE] Definition
>
>Der $n$-fach Wiederholungscode beschreibt die Anzahl an $E_{n'}$ Einheitsmatrizen innerhalb von $G$, sodass man eine möglichst hohe Redudanz und Sicherheit schafft. Jedoch leidet der Informationsfluss dadurch.
>
>$3$-fach Wiederholdungscode $\Rightarrow$ da $P[X]=10^{-6}$ für ein Fehlerbit wissen wir wo der Fehler auftritt $\Leftrightarrow$ wir haben $2$ Stellen wo wir das eigentliche Bit sehen.
>
>$\Rightarrow 1$-fehlererkennender Code
>$\Rightarrow 1$-fehlerkorrigierender Code

<br>

## Dekodieren

>[!NOTE] Definition
>
>Sei $c'$ der kodierte, durch einen Kanal geschickte kodierte Code. Der Empfänger kennt $G$, die Redundanz ist immer unter dem kodierten Code.
>
>Frage: Ist $c'\in C$?
>1. Fall - ja $\hspace{0.525cm}\Rightarrow$ löse $G\cdot x=c'$
>2. Fall - nein $\Rightarrow$  Hammingabstand berechnen und ähnlichstes Codewort berechnen

<br>

### 2. Fall Abfolge

>[!NOTE] Definition
>
>Annahme: Zahl der fehlerhaften Bits ist möglichst klein, also $1$
>$\Rightarrow$ suche $c''\in C$, sodass es sich in möglichst wenig Stellen unterscheidet von $c'$
>
>1. Fall - $\exists_1$ solches $c''\hspace{2.83cm}\Rightarrow$ löse $G\cdot x=c''$
>2. Fall - $\exists_{\ge 1}$ passende Alternativen $\Rightarrow$ Neusendung des Codes

<br>

## Hamminggewicht

>[!INOTE] Definition
>
>Für ein beliebiges $c\in K^n$ gilt:
>$$w(c):=|\{i\in\{1,...,n\}\ |\ c_i\not = 0\}|$$

<br>

## Hammingabstand

>[!NOTE] Definition
>
>Für $2$ beliebige $c,c'\in C$ gilt:
>$$d(c,c'):=|\{i\in\{i,...,n\}\ |\ c_i\not = c'_i\}|=w(c-c')$$
>
>Da Körper des $\mathbb{F}_2$ gelten Addition und Subtraktion der Binärarithmetik
>
>Für ein beliebiges $C\subseteq K^n$ gilt:
>$$d(C)=min\{w(c)\ |\ c\in C\setminus\{0_v\}\}=min\{d(c,c')\ |\ c,c'\in C,\ c\not=c'\}$$
