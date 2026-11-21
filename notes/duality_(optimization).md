Consider a minimization problem with a feasible region $C$:

$$
p^{\star}=\inf_{x\in C}f(x).
$$

If there exists a two-variable function $F(x,y)$ such that $f(x)=\sup_{y\in Y}F(x,y)$, then the minimization problem can be written as

$$
p^{\star}=\inf_{x\in C}f(x)=\inf_{x\in C}\sup_{y\in Y}F(x,y).
$$

By the definition of supremum and infimum, the following holds for all $x'\in C$ and $y'\in Y$:

$$
\inf_{x\in C}F(x,y')\leq F(x',y')\leq \sup_{y\in Y}F(x',y).
$$



이 관계는 \inf_{x\in C}F(x,y')에다가 y'에 대한 상한을 취하고 \sup_{y\in Y}F(x',y)에다가 x'에 대한 하한을 취해도 성립하여야 한다. 따라서 아래의 부등식이 성립하며, 이를 최대·최소 부등식이라고 한다.
