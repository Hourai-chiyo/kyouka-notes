# 03 · 行列式的展开与 Cramer 法则

> 源：`IMG_20261119_103414.jpg`（第 5 页）。
> 原图标题字迹较草（形似「对角方程组」），按内容记为「n 元线性方程组」。
> 缩写处按标准定义补全，不改变原意。

## 例：化三角形计算行列式

$\displaystyle \begin{vmatrix} 1 & 2 & -3 & 4\\ 2 & 3 & -4 & 7\\ -1 & -2 & 5 & -8\\ 1 & 3 & -5 & 10 \end{vmatrix} = \begin{vmatrix} 1 & 2 & -3 & 4\\ 0 & -1 & 2 & -1\\ 0 & 0 & 2 & -4\\ 0 & 1 & -2 & 6 \end{vmatrix} = \begin{vmatrix} 1 & 2 & -3 & 4\\ 0 & -1 & 2 & -1\\ 0 & 0 & 2 & -4\\ 0 & 0 & 0 & 5 \end{vmatrix} =-10.$

## 余子式与代数余子式

把元素 $a_{ij}$ 所在的行和列划去，剩下的行列式 $M_{ij}$ 称为 $a_{ij}$ 的**余子式**；称

$\displaystyle A_{ij}=(-1)^{i+j}M_{ij}$

为 $a_{ij}$ 的**代数余子式**。

**引理**：若第 $i$ 行元素除 $a_{ij}$ 外全为 $0$，则 $D=a_{ij}A_{ij}$。

## 行列式按行（列）展开

$\displaystyle D=a_{i1}A_{i1}+a_{i2}A_{i2}+\cdots+a_{in}A_{in}\qquad (i=1,2,\dots,n),$

$\displaystyle D=a_{1j}A_{1j}+a_{2j}A_{2j}+\cdots+a_{nj}A_{nj}\qquad (j=1,2,\dots,n).$

**定理（异乘为零）**：

$\displaystyle a_{i1}A_{j1}+a_{i2}A_{j2}+\cdots+a_{in}A_{jn}= \begin{cases} D, & i=j,\\ 0, & i\ne j, \end{cases}$

$\displaystyle a_{1i}A_{1j}+a_{2i}A_{2j}+\cdots+a_{ni}A_{nj}= \begin{cases} D, & i=j,\\ 0, & i\ne j. \end{cases}$

## Cramer 法则

$n$ 元线性方程组

$\displaystyle \begin{cases} a_{11}x_1+a_{12}x_2+\cdots+a_{1n}x_n=b_1,\\ a_{21}x_1+a_{22}x_2+\cdots+a_{2n}x_n=b_2,\\ \qquad\vdots\\ a_{n1}x_1+a_{n2}x_2+\cdots+a_{nn}x_n=b_n. \end{cases}$

若系数行列式 $D\ne 0$，则方程组有唯一解

$\displaystyle x_1=\frac{D_1}{D},\quad x_2=\frac{D_2}{D},\quad \cdots,\quad x_n=\frac{D_n}{D},$

其中 $D_j$ 是把 $D$ 的第 $j$ 列换成常数列 $(b_1,b_2,\dots,b_n)^{\mathsf T}$ 得到的行列式。

> **整理者注**：原图只写了 $D_j$ 的记号，没有文字说明；上面的 $D_j$ 定义按标准 Cramer 法则补全。
