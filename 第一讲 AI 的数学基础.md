### 随机变量

#### 定义：随机变量

设 $\Omega$ 为试验 $E$ 的样本空间，$X: \Omega \to \mathbb{R}$ 为一个实值函数，若 $\forall x \in \mathbb{R}, \{\omega \mid X(\omega) \le x\}$ 为一个随机事件，则称 $X$ 为随机变量。

- 通常用大写字母表示随机变量。

#### 定义：分布函数

设 $X$ 为随机变量，称：

$$
\begin{aligned}
F : \mathbb{R} &\to [0, 1] \\
x &\mapsto \Pr [X \leq x]
\end{aligned}
$$

为 $X$ 的分布函数，则有：

$$
\forall x_1 < x_2, \Pr[x_1 < X \leq x_2] = F(x_2) - F(x_1)
$$

故分布函数可完整描述随机变量取值概率的规律。

#### 定义：概率密度函数

设一维连续型随机变量 $X$ 的分布函数为 $F$，若在 $\mathbb{R}$ 上可积的非负函数 $f$ 使得 $F(x) = \displaystyle\int_{-\infty}^x f(t) \text{d} t$，则称 $f$ 为 $X$ 的概率密度函数。

#### 定义：数学期望

- 设离散型随机变量 $X$ 的分布列为 $P(X = x_k) = p_k \quad (k \in \mathbb{N}_+)$，若级数 $\displaystyle\sum_{k = 1}^{+\infty} x_k p_k$ 绝对收敛，则称之为 $X$ 的数学期望，记作 $E(X)$。
- 设一维连续型随机变量 $X$ 的概率密度函数为 $f$，若广义积分 $\displaystyle\int_{-\infty}^{+\infty} x f(x) \text{d} x$ 绝对收敛，则称之为 $X$ 的数学期望，同样记作 $E(X)$。

#### 定义：协方差

- _Motivation：考察两个随机变量的相关性，则需引入同时与两者有关的项。_

若随机变量 $X, Y$ 的期望存在，称：

$$
\text{Cov}(X, Y) = E[(X - E(X))(Y - E(Y))]
$$

为 $X, Y$ 的协方差，则有：

- $\text{Cov}(X, X) = D(X), \text{Cov}(X, Y) = \text{Cov}(Y, X)$。
- $\text{Cov}(X, Y) = E(XY) - E(X) E(Y)$。

### 定义：相关系数

若随机变量 $X, Y$ 的方差存在，且 $D(X), D(Y) > 0$，称：

$$
\rho_{X, Y} = \frac{\text{Cov}(X, Y)}{\sqrt{D(X)} \cdot \sqrt{D(Y)}} \in [-1, 1]
$$

为 $X, Y$ 的相关系数。
