Consider a minimization problem with a feasible region $C$:

$$
p^{\star}=\inf_{x\in C}f(x).
$$

If there exists a two-variable function $F:C\times Y\to[-\infty,+\infty]$ such that $f(x)=\sup_{y\in Y}F(x,y)$, then the minimization problem can be written as

$$
p^{\star}=\inf_{x\in C}f(x)=\inf_{x\in C}\sup_{y\in Y}F(x,y).
$$

By the definition of supremum and infimum, the following holds for all $x'\in C$ and $y'\in Y$:

$$
\inf_{x\in C}F(x,y')\leq F(x',y')\leq \sup_{y\in Y}F(x',y).
$$

The inequality $\inf_{x\in C}F(x,y')\leq \sup_{y\in Y}F(x',y)$ holds for all $x'\in C$ and $y'\in Y$, and thus we can apply $\sup_{y\in Y}$ to the left side and $\inf_{x\in C}$ to the right side. This gives the **max-min inequality**.

$$
\sup_{y\in Y}\inf_{x\in C}F(x,y)\leq\underbrace{\inf_{x\in C}\sup_{y\in Y}F(x,y)}_{=p^{\star}}
$$

Now, what is $\sup_{y\in Y}\inf_{x\in C}F(x,y)$? $\inf_{x\in C}F(x,y)$ is a function in $y$, so let $g(y)=\inf_{x\in C}F(x,y)$. Then the left side itself becomes another maximization problem whose optimal value acts as the lower bound to the optimal value of the original problem $p^{\star}$. If we denote $d^{\star}=\sup_{y\in Y}g(y)$, then the max-min inequality becomes what we call **weak duality**:

$$
\boxed{d^{\star}\leq p^{\star}.}
$$

The original minimization problem $\inf_{x\in C}f(x)$ is called a **primal problem** and the maximization problem derived from it is called a **dual problem**. The gap between the two optimal values $p^{\star}-d^{\star}$ is called a **duality gap** and is greater than or equal to $0$ due to the weak duality. In some cases, $d^{\star}=p^{\star}$ holds (duality gap $0$) and this is called **strong duality**. Note that strong duality only means the supremum and infimum are equal, and this does not guarantee the existence of optimal points.
