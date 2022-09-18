# Section2 Basic Topology

## FINITE,COUNTABLE,AND UNCOUNTABLE SETS

### 2.1 Definition

Consider two sets ,A and B and a mapping from A to B ,which we may call it 'f'.The 'f' should be some manner,or be said to be a ***function***(mapping).

The elements f(x) for all x in A,are called ***values***.

The set of all values is called the ***range*** of f.

### 2.2 Definition

Clearly,$f(A)$ is the range of f and $f(A) \subseteq B$.

We say that f maps A ***onto*** B when $f(A) = B.$

For each $y \in B$,when $f^{-1}(y)$ covers all the elements of A,f is said to be ***1-1(one to one)*** mapping of A into B.

[^1]: Rudin.Principles of Mathematical Analysis

We may illustrate the definition with these graphs below:

![not mapping](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\not mapping.png)![not onto-1](/bins/not onto-1.png)

![not onto-2](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\not onto-2.png)

![onto(but not 1-1)](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\onto(but not 1-1).png)

![not 1-1](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\not 1-1.png)

![1-1(but not onto)](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\1-1(but not onto).png)

![1-1 and onto](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\1-1 and onto.png)

### 2.3 Definition

Any relation with these properties is called an equivalence relation:

> $$
> \begin{align}
> &reflexive:A \sim A.\\&symmestric:If \ A\sim B,then\ B\sim A.\\
> &transitive:If\ A \sim B\ and\ B \sim C,then\ A\sim C.
> \end{align}
> $$

If there exists a 1-1 mapping of A onto B,we say that A and B are equivalent,that is,$A\sim B$.



### 2.4 Remark

> if $J_m \sim J_n,m=n$.
>
> if $m=n,J_m\sim J_n$.

where $J_n$ is the set whose elements are the integers 1,2, . . . ,n;



### 2.5 Definition

For any set A,we may say:

> a. A is **finite** if $A\sim J_n$ for some n.(empty set $\varnothing$ is considered to be finite)
>
> b. A is **infinite** if A is not finite.
>
> c. A is **countable** if $A\sim J$.
>
> d. A is **uncountable** if A is neither **finite** or **countable**.
>
> e. A is **at most countable**(至多可数) if A is **finite** or **countable**.



### 2.6 Remark

> a.$N\sim Z$
>
> > For :$0,1,2,3,...\rightarrow 0,-1,1,-2,...$
> >
> > We may even find out an explicit formula.
>
> b. $\forall a,b \in R,(a,b)\sim (0,1)$:
>
> > Graphic explanations:
> >
> > ![](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\remark 2.6-1.png)
> >
> > $\forall x $ in (a,b),denoted by N on the axis AB,has some linear pattern corresponding to M in axis 01.
>
> c.$(0,1)\sim R$
>
> > We may even find the explicit function of it:
> >
> > ![remark 2.6-2](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\remark 2.6-2.png)
>
> d. $\forall a,b \in R,(a,b)\sim R$:
>
> > An equivalence relation is transitive,so it is clear.
> >
> > In fact,we could replace the definition of infinite set 2.5.b by the statement below:
> >
> > **A is infinite if A is equivalent to one of its proper subsets.**

### 2.7 Definition

We may sort of order or label the elements in a countable set $A$ in the way of 'sequence in $A$':

$A=\{x_n\},n\in J$.

The elements in the set arranged in this way need not to be distinct.(For example,we may assume:$f(x):=x^2,x_1=(-1)^2=1,x_2=(+1)^2=1,x_1=x_2$,which is valid)



### 2.8 Theorem 

Every infinite subset of a countable set $A$ is countable.

No uncountable set can be a subset of a countable set.

***Proof:***

The key operation is to find out the 'net mapping' of $J_n$,the subset of $J$:

![theorem 2.8-1](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\theorem 2.8-1.png)

In this way we found a mapping function from $J_n$ to $A$ such that $n_k$ is the smallest integer greater than $n_{k-1}$and $x_{n_k}\in E$,where $f(k)=x_{n_{k}}$.

#### 

### 2.9 Theorem

Let $\{E_n\},n=1,2,3,...$,be a sequence of countable sets,and put
$$
S=\cup^{\infin}_{n=1}E_n
$$
**Then $S$ is countable.**

### 2.10 Remark

Let $A=(0,1)$ and $E_\alpha=(0,\alpha),$then

> $$
> \begin{align}
> &(1)\cup_{\alpha \in A}E_\alpha = (0,1)\\&(2)\cap_{\alpha \in A}E_\alpha = \varnothing.
> \end{align}
> $$

(2) is clear,for:
$$
\forall y>x>0,y\notin E_x.
$$
Hence $\forall y >0,y\notin \cup_{x\in A} E_x$.

To prove (1),we let $M=\cup_{\alpha \in A}E_\alpha$.$\forall x \in M,x \in (0,1),M \subseteq (0,1)$.

Suppose  $\forall \beta \in (0,1)$, $\forall \alpha \in(0,1),\beta \notin E_{\alpha}$,then $\beta>=1$.However $\beta <1$.

Hence,$\forall\  \beta \in (0,1),\exist \alpha \in(0,1),s.t.\beta \in E_{\alpha}$,whereas $(0,1)\subseteq M$.

Since $(0,1) \subseteq M,M \subseteq (0,1),M=\cup_{\alpha \in A}E_\alpha=(0,1)$.



### 2.11 Facts

 A、B are two sets.

> (1)If A has a 1-1 mapping $f$ into B,$\exist\ g:B\rightarrow A,s.t.(gof)=idA$.
>
> (2)If $f$ maps A onto B,$\exist\ g:B\rightarrow A,s.t.(fog)=idB$.



### 2.12 Theorem

Let $\{E_n\},n=1,2,3,...$,be a sequence of countable sets,and put $S=\cup^{\infin}_{n=1}E_n$.Then S is countable.

***Proof:***

Rearrange the order of the terms of the sets $T$ in a sequence $\{x_{nk}\}$:

$x_{11}\rightarrow x_{21}\rightarrow x_{12}\rightarrow x_{31}\rightarrow x_{22}\rightarrow x_{13}\rightarrow ...$

It is valid,because for each element on the specific diagonal

 ,the sum of the indexes ranges from (2) to n+k with step 1.

However,some entries may appear more than once,so what we can assure is that it goes that
$$
S\sim T \subseteq N
$$
Hence S and T are **at most countable**. Since S is infinite,S is countable.



**Corollary**

Suppose A is at most countable,and, for every $\alpha \in A,B_\alpha$is at most countable. Put
$$
T=\cup_{\alpha \in A}B_{\alpha}
$$
Then T is at most countable.

For T is the subset of the at most countable set  $S=\cup^{\infin}_{n=1}E_n$.



### 2.13 Theorem

Let $A$ be a countable set,and let $B_n$ be the set of all n-tuples $(\alpha_1,...,\alpha_n)$,where $\alpha_k \in A(k=1,...,n)$,and the elements $\alpha_1,...,\alpha_n$ need not to be distinct. Then $B_n$ is countable.

***Proof:***

$B_n=\underbrace {A\times...\times A}_{n}$.By induction and Theorem 2.12,we know that $A\times A$ is countable,thus $A\times A\times A$ is countable,...,$B_n$ is countable.



**Corollary**

The set of all **rational numbers** is countable.

That is because $\mathbb{Q} \subset \mathbb{N}\times \mathbb{N}$,$ \mathbb{N}\times \mathbb{N}$ is countable and $\mathbb{Q}$ is at most countable but infinite,and thus countable.



### 2.14 Theorem

Let $A$ be the set of all sequences whose elements are the digits 0 and 1.This set A is uncountable.

***Outline of the proof:***

To prove something wrong is usually hard,so we may try to prove it by contradictions.

We may assign E as a sequence of countless sequences:
$$
E=\{s_1,s_2,s_3,...\}
$$
,where $s_k,k=1,2,...$  is a sequence.

If a set is countable,it can be rearranged to a sequence like that:
$$
\begin{align}
E=\{&\{a_{11},...\},\\
&\{a_{21},a_{22},...\},\\
&\{a_{31},a_{32},a_{33},...\},...\}\\

\end{align}
$$
Let's DIY a sequence to create the contradiction in the way below:

Consider a sequence $\{b_k\}$ like that:
$$
b_{k}=\left\{
\begin{align}
&1,a_{kk}=0\\
&0,a_{kk}=1
\end{align}
\right.
$$
The sequence $b_k \neq E_{n},\forall n \in N$.However $b_k \in E$.

Thus $A$ is uncountable.



**Corollary**

The set of all real numbers is uncountable.



## METRIC SPACES

### 2.15 Definition

A set X is said to be a metric space if two points a and b in X associate a real number function d(p,q) such that

> $$
> \begin{align}
> &Non-negativity: &d(p,q)>0\ if \ p\neq q,d(p,p)=0;\\
> &Symmetry:&d(p,q)=d(q,p);\\
> &Triangle\ Inequality:&d(p,q) \leq d(p,r)+d(r,q),for\ any\ r \in X.
> \end{align}
> $$

Any function with these three properties is called a distance function,or a metric.



### 2.16 Definition

The **unit ball** is a set defined by
$$
\{\mathbb{x}\in R^n|d(\mathbb{x},\mathbb{0})\leq 1\}
$$


### 2.17 Definition

Let $X$ be a metric space,all points and sets mentioned below are elements and subsets of $X$.

> 1. A **neighborhood** of $p$ is a set $N_r(p)$ consisting of all $q$ such that $d(p,q)<r$,for some $r>0$.The number ***r*** is called the radius of $N_r(p)$.(random r)
> 2. A point p is a ***limit point*** of the set $E$ if *every* neighborhood of p contains a point $q\neq p$ such that $q \in E$.(no one but myself).**$i.e.\forall r>0,N_r(p)\cap E \neq \varnothing$**
> 3. If $p \in E$ and $p$ is not a limit point of $E$,then $p$ is called an ***isolated point*** of $E$.
> 4. A point is an ***interior point*** of E if there is a neighborhood N of p such that $N\subset E$.$i.e.\exist r>0,N_{r}(p)\subseteq E$.
> 5. E is closed if **every limit point** of E is a point of E.
> 6. E is open if every point of E is a **interior point**.$\forall p \in E,\exist r>0,s.t.N_r(p)\subseteq E$.
> 7. The **complement** of E,denoted by $E^c$,is the set of all points $p \in X$ such that $p \notin E$.
> 8. E is ***perfect*** if E is closed and if every point of E is a limit point of E.
> 9. E is ***bounded*** if there is a real number M and a point $q \in X$ such that $d(p,q)<M$ for all $p \in E$.
> 10. E is ***dense*** in X if every point of X is a limit point of E,or a point of E(or both).

Notice that an interior point is not necessarily a limit point.



### 2.18 Facts

Let $X$ be a metric space,all points and sets mentioned below are elements and subsets of $X$.

> 1. If $E$ is open,$E^c$ is closed;
> 2. If $E$ is closed,$E^c$ is open.

***Proof***:

1.We need to show that if p is a limit point of $E^c$ then $p \in E^c$.

Let p be a limit point,$i.e.\forall r>0,N_r(p)\cap E^c \neq \varnothing$.

$\therefore \forall p \in E,\forall r >0,N_r(p)$ dosen't $\subseteq E$.

Therefore p is not an interior point of E. However,every point in E is an interior point.$i.e. p\notin E,p\in E^c$.



2.The statement is equivalent to **"If $E$ is not open,then $E^c$ is not closed"**,which is trivial.

Since E is not open,that is $\exist p \in E,\forall r>0,s.t.N_r(p)\cap E^C \neq \varnothing$.

Therefore $E^c$ is not closed.



### 2.19 Facts

Let $A_n,B_n$ be a open set and a closed set which are both subsets of a metric space X.$(n=1,2,3...)$

> 1. $\cup^{n}_{i=1} A_n$ is open. $\cup^n_{i=1}B_n$is closed.$\cap^n_{i=1}A_n$is open,$\cap_{i=1}^nB_n$is closed.
> 2. $\cup_{i=1}^{\infin}A_n$ is open.$\cup^{\infin}_{i=1}B_n$ is closed.
> 3. $\cap^{\infin}_{i=1}A_n$ may NOT be open.$\cup^{\infin}_{i=1}B_n$ may NOT be closed.



### 2.20 Theorem

If p is a limit point of a set $E$,then every neighbourhood of $p$ contains **infinitely** many points of $E$.

**Corollary**

A finite point set has no limit points.

Hence,a finite set is closed.



### 2.22 Theorem

Let {$E_n$} be a (finite or infinite)collection of sets $E_\alpha$.Then $(\cup_\alpha E_\alpha)^c=\cap_\alpha(E_\alpha^c)$



### 2.23 Definition

If X is a metric space,if $E \subset X$,and if $E'$ denotes the set of all limit points of $E$,then the *closure* of $E$ is the set $\overline{E} = E \cup E'$.



### 2.24 Theorem

If X is a metric space and $E\subset X$,then

> (a) $\overline{E}$ is closed,
>
> (b) $\overline{E}=E$ if and only if E is closed,
>
> (c) $\overline{E} \subset F$ for every closed set $F \subset X$ such that $E \subset F$.



### 2.25 Definition

If $E$ is a metric space and $E$ is a closed set,$E$ is perfect if and only if $E'=E$.



### 2.26 Theorem

Let $E$ be a nonempty set of real numbers which is bounded above. Let $y=sup E$.Then $y \in \overline{E}$.

***Proof***

Assume $y \notin E$.For each $h>0$ there exists a point $x\in E$,such that $y-h<x<y$,otherwise $y-h$ would be the upper bound of $E$.Thus y is a limit point and $y\in \overline{E}$.

**(We omit some new definitions)**



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



### 2.43 Weierstrass Theorem(魏尔斯特拉斯定理)

Every bounded infinite subset of $R^k$ has a limit point in $R^k$.

***Proof:***

Let the set be $S$.Since it is bounded,there is some k-cell $I_k$ s.t. $S\sub I_k$.$I_k$ is compact,thus $S$ has a limit point in $I_k$.Namely the theorem holds.



# 2-4 Perfect Sets and Connected Sets

### 2.44 Definition

A set $E$ is **perfect** if and only if $E'=E$.



### 2.45 Theorem

Let $P$ be a nonempty perfect set in $R^k$.Then $P$ is uncountable.

***Proof***

Suppose $P$ is countable,consider a sequence of neighborhood {$V_n$} of these points $x_1,x_2,x_3,...$.

Since $P'=P,V_n \cap P \neq \varnothing$.We may construct a sequence of {$V_n$} following three properties below:

> 1. $\overline{V}_{n+1} \sub V_n$
> 2. $x_n \notin \overline{V}_{n+1}$
> 3. $V_{n+1} \cap P \neq \varnothing$

Put $K_n=\overline{V_n} \cap P$.Since $\overline{V}_n$ is closed and bounded,it is compact.

By (2),no points in $P$ lies in $\cap^{\infin}_{1} K_n$.$K_n \sub P$,$\cap^{\infin}_{1} K_n=\varnothing.$

But each $K_n$ is nonempty,by (3).

It contradicts the theorem "If {$K_n$} is a sequence of nonempty compact sets such that $K_n \supset K_{n+1}$.(n=1,2,3,...),then $\cap_1^\infin K_n$ is not empty."



#### 2.46 Cantor Set

***Note:***

It is a perfect set in $R^1$ which contains no segment.



### 2.47 Definition

Two subsets $A$ and $B$ of a metric space $X$ are said to be separated if both $A\cap \overline{B}$ and $\overline{A} \cap B$ are empty, i.e.,if no point of $A$ lies in $\overline{B}$ and no points of $B$ lies in $\overline{A}$.

A set $E\sub X$ is said to be connected if $E$ is not a union of two nonempty separated sets.

**If a set is NOT connected,it is a union of two nonempty separated sets.**

Separated sets are disjoint,but disjoint sets need not to be separated.