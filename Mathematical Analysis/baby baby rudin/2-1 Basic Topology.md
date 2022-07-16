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

![not mapping](E:\全部-自定义\学习\鲁丁 数分\2-1 Basic Topology\bins\not mapping.png)![not onto-1](\bins\not onto-1.png)

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

