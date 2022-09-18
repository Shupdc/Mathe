# 2-3 Compact Sets

### 2.31 Definition

By an open cover of a set $E$ in a metric space $X$ we mean a collection {$G_\alpha$} of open subsets of $x$ such that $E \subset \cup_\alpha G_\alpha$.



### 2.32 Definition

A subset K of a metric space $X$ is said to be *compact* if every open cover of $K$ contains a *finite* subcover.

More explicitly,the requirement is that if {$G_\alpha$} is an open cover of $K$,then there are finitely many indices $\alpha_1,\alpha_2,...,\alpha_n$ such that $$K\subset G_{\alpha _1}\cup...\cup G_{\alpha_n}$$.



### 2.33 Theorem

Suppose $K\subset Y \sub X$.Then $K$ is *compact relative to $X$ if and only if $K$* is compact to $Y$.

***Proof***

The "if and only if" condition is equivalent to "sufficient and necessary".

(1)Suppose $K$ is compact relative to $X$,We have 
$$
K \sub G_{\alpha_1} \cup G_{\alpha_2} \cup ...\cup G_{\alpha _n} \tag*{(1)}
$$
Let
$$
V_\alpha =Y \cup G_{\alpha}
$$
Then we have
$$
K \sub V_{\alpha_1}\cup V_{\alpha_2} \cup ...\cup V_{\alpha_n} \tag*{(2)}
$$
Thus we prove that $K$ is compact relative to $Y$.

(2)Suppose $K$ is compact relative to $Y$.Similarly Let {$G_n$} be some finite collection of open subsets of $X$ which covers  $K$,and put $V_\alpha = Y \cap G_\alpha$.Then we get (2),which implies (1),and therefore $K$ is compact relative to $X$.



### 2.34 Theorem

Compact subsets of metric spaces are closed.

***Proof***

**这一证明表现出了紧性将局部推广至全局的作用**.

我们等价于证明，“度量空间的紧子集$K$之补集$K^c$为开集”.

我们考虑紧集合中的任意一点$a$和其补集的任意一点$b$.现在为了方便我们不妨固定点$b$,考虑有限个子覆盖(subcover){$A_n$}及点$b$的有限个邻域($B_n$},使得
$$
K \sub \cup_{i=1}^nA_n\\
V=\cap_{i=1}^nB_n
$$
其中，这两个邻域的“中心点”距离记为$d(a_n,b)$.并令所有对应的领域$A_n$与$B_n$满足半径$r_n<\frac{d(a_n,b)}{2}$.

这样就有$V\cap K=\varnothing$.(局部不相交推广至全局不相交).因此对于补集中的任意一点$b$,总能以此法构造领域,使得$N_r(b) \cap K = \varnothing,N_r(b) \sub K^c$.

因此等价命题得证，原命题得证.



### 2.35 Theorem

Closed subsets of compact sets are compact.

***Proof***

Let $K$ be a compact subset of a metric space $X$ and let $F\subseteq K$ be closed(relative to $X$).

Let {$G_n$} be an open cover of $F$,then {$G_\alpha \cap F^c$} is an open cover of $K$.**(Since $F^c$ is open)**



**Corollary**

If $F$ is closed and $K$ is compact,then $F\cap K$ is compact.

The intersection of finite compact sets is compact.

 

### 2.36 Definition

Let {$S_n$} be a collection of subsets of a metric space $X$.We say {$S_n$} satisfies ***finite intersection condition*** if the intersection of every finite subcollection of {$K_\alpha$} is nonempty.



### 2.37 Theorem 

If {$K_\alpha$} is a collection of **compact** subsets of a metric space $X$ such that the intersection of every finite subcollection of {$K_{\alpha}$} is nonempty,then $\cap K_{\alpha}$ is nonempty.

***Proof***

The statement is equivalent to "If $\cap K_\alpha=\varnothing$,then $\cap_{i=1}^n K_i = \varnothing$ ".

We may fix a member $K_1$ such that $K_1 \cap (\cap_{i=2}^\infin K_i)=\varnothing,K_1 \sub (\cap_{i=2}^\infin K_i)^c,K_1 \sub (\cup_{i=2}^\infin K_i^c)$.

Since $K_1$ is compact,$K_1 \sub (\cup_{i=2}^n K_i^c)$,$\cap_{i=1}^n K_i = \varnothing$ .



**Corollary**

If {$K_n$} is a sequence of nonempty compact sets such that $K_n \supset K_{n+1}$.(n=1,2,3,...),then $\cap_1^\infin K_n$ is not empty.



### 2.38 Theorem

If $E$ is a infinite subset of a compact set $K$,then $E$ has a limit point in $K$.

***Proof***

**The key idea is,let I be the k-cell,$\exist x^*\in I$,s.t. if $y \in K_n$, and $K_{n+1} \sub K_n,K_1 \sub I$,then $|y-x^*|$ must be covered by some neighborhood. Namely, $\forall r>0,\exist n\in N,y\in K_n,s.t.|y-x^*|<r$.That is to say,there is always some finite subcollection of {$G_n$} capable of covering $I_n$.Suppose $E' \cap E = \varnothing$.That is to say, $\forall p\in E,\forall \epsilon \in R,N_{\epsilon}p \backslash\{p\}=\varnothing$ .Then there is no finite subcollection of {$V_q$} can cover $E$.Since $E \sub K$,therefore $K$ is not compact. This contradicts the compactness of $K$.**

我们应当指出，定理2.38可以用于证明**闭区间套**定理。

**更严格的证明如下：**

We prove it by contradiction.

Suppose no point of $K$ is a limit point of a compact set $K$,then for each $q \in K$,$\exist r>0,s.t.N_r(p)\cap E =\varnothing,\{p\}.i.e.$each point in $K$ would have a neighborhood $N_r(p)$ containing at most one point of $E$.

Therefore,$E$ cannot be covered by infinite open sets,and the same is true for $K$,since $E \sub K$,which contradicts the compactness of $K$.



### 2.39 Theorem

If {$I_n$} is a sequence of intervals in $R^1$,such that $I_n \supset I_{n+1}$(n=1,2,3,...),then $\cap^\infin_1 I_n$ is not empty.

***Proof***

令$I_n=[a_n,b_n]$,由于实数集的稠密性，总能找到一个{a_n}的上确界$\alpha$使得$\alpha \in I_n,(n=1,2,3,...)$.故原命题得证.

It is known that $R$ has the least-upper-bound property,and thus has the greatest-lower-bound property. Let {$a_n$} be set of all the lower bounds of each interval $I_n$,and {$b_n$} be the set of all the upper bounds of each interval $I_n$.

It is apparent that:
$$
\exist x\in R,s.t. x=sub\{a_n\}.\\
\forall n \in N^*,a_n<x\leq b_1 \leq b_2 \leq ... \leq b_n
$$
Therefore we find that $\forall n \in N^*,x\in I_n,x\in \cap^{\infin}_1I_n$.



### 2.40 Theorem

Let $k$ be a positive integer. If {$I_n$} is a sequence of k-cells such that $I_n \supset I_n+1$(n=1,2,3,...),then $\cap _1^\infin I_n $ is not empty.

***Proof***

我们对k维的每一维空间都作类似2.39定理的操作即可得证。



### 2.41 Theorem

Every k-cells is compact.

***Proof***

Let I be a k-cell,consisting of all points $x=(x_1,x_2.,...x_n)$ such that $a_j < x_j < b_j(1\le j \le k)$.Put
$$
\delta = \sqrt{\sum _1 ^k (b_j - a_j)^2}
$$
Then $|x-y|\le \delta$,if $x\in I,y\in I$.

To get a contradiction,we suppose that there exists a open cover {$G_n$} of $I$ which contains no finite subcover of $I$.

Put $c_j = \frac{a_j+b_j}{2}$.The intervals will be separated into $2^k$ k-cells of $Q_i$ whose union is $I$.

According the hypothesis,there must be at least one subset cannot be covered by {$G_n$},call it $I_1$.



***Corollary:***

Let $k \in N^*$,If {$I_n$} is a sequence of k-cells such that $I_{n+1}\sub I_n$(n=1,2,3,...),then $\cap ^{\infin} _{1}I_n$ is not empty.

***Proof:***

For each dimension,apply Theorem 2.39.We then obtain $x^*=(x_1^*,x_2^*,...,x^*_k)$.$x^* \in I_n,n=1,2,3...$,which makes the corollary follow.



### 2.42 Theorem(3 个等价命题)

需要指出的是，该定理中(a)与(b)的等价性被称作Heine-Borel theorem（海涅-博雷尔定理）：

If a set E in $R^k$ has one of the following three properties,then it has the other two:

>  (a) E is closed and bounded.
>
>  (b) E is compact.
>
>  (c) Every infinite subset of E has a limit point in E.

***Proof:***

**(a) -> (b):**

$E\sub I$ for some k-cell $I$.Since a closed subset of a compact set is  compact(Theorem 2.35 ) and each k-cell is compact(Theorem 2.40,E is compact.

**(b) -> (c):**

If $E$ is a infinite subset of a compact set $K$,then $E$ has a limit point in $K$.（Theorem 2.38)

That implies (b) to (c).

**(c)  -> (a):**

Suppose $E$ is not bounded,then some subset of $E$(call it $S$) contains points $x_n$ with $|x_n| > n,n\in N^*$.

Thus $S$ clearly has no limit point,contradicting with (c).

Suppose $E$ is not closed,consider a limit point of $E$ but not in $E$.Let $S=\{x_n|x_n \in E,|x_n-x_0|<\frac{1}{n}\}$.

Thus $S$ is infinite, and $S$ has no limit point but $x_0$ in $R^k$.

Let's prove it:

Fix $y\in R^k,y\neq x_0$,then |$x_n - y$|$\geq |x_0- y|+|x_n-x_0|\\ \geq |x_0-y|-\frac{1}{n}\\\geq\frac{1}{2}|x_0-y|$

Therefore $x_0$ is the only limit point of $S$.

Thus S has no limit point in E,contradicting with (c).

Hence it must be closed if (c) holds.



### 2.42 Weierstrass Theorem(魏尔斯特拉斯定理)

Every bounded infinite subset of $R^k$ has a limit point in $R^k$.

***Proof:***

Let the set be $S$.Since it is bounded,there is some k-cell $I_k$ s.t. $S\sub I_k$.$I_k$ is compact,thus $S$ has a limit point in $I_k$.Namely the theorem holds.

