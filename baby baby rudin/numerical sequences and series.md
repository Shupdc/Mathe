# Chapter 3 NUMERICAL SEQUENCES AND SERIES

## **CONVERGENT SEQUENCES**

### **3.1 Definition**

A sequence {$p_n$} in a metric space X is said to **converge** if $\exist p \in X$,s. t.$\forall \epsilon>0,n\geq N,d(p_n,p)<\epsilon$.
If {$p_n$} is not converge,it is said to diverge.



### **3.2 Theorem**

Let {$p_n$} be s sequence in a metric space $X$.

> ( a ) {$p_n$} converges to $p \sub X$ if and only if each neighborhood of p contains $p_n$ for all but finitely many n.
> ( b )If $p \in X,p' \in X$,and if {$p_n$} converges to p and p',then p' = p.
> ( c )If {$p_n$} converges,then {$p_n$} is bounded.
> ( d )If $E\sub X$ and if p is a limit point of $E$,then there is a sequence {$p_n$} in $E$ such that $p = lim_{n\rightarrow \infin} p_n$.

### **3.3 Theorem**

Suppose {$s_n$},{$t_n$} are complex sequences,and $lim_{n\rightarrow\infin}s_n=s,lim_{n\rightarrow\infin}t_n=t.$Then the four fundamental operations of arithmetric holds.



### **3.4 Theorem**

> (a) Suppose $x_n \in R^k(n=1,2,3,...)$ and $x_n = (\alpha_{1,n},...,\alpha_{k,n})$.Then {$x_n$} converges to $x=(\alpha_1,...,\alpha_k)$ if and only if $lim_{n \rightarrow \infin}\alpha_{j,n}=\alpha_j(1\leq j\leq k)$.
>
> (b) Suppose {$x_n$} ,{$y_n$} are sequences in $R^k$,{$\beta_n$} is a sequence of real numbers,and $x_n \rightarrow x,y_n \rightarrow y,\beta_n \rightarrow \beta$.Then
>
> $lim_{n\rightarrow \infin}(x_n+y_n)=x+y,lim_{n\rightarrow \infin}(x_n \cdot y_n)= x \cdot y, lim_{n\rightarrow \infin}\beta_n x_n = \beta x$.

***Proof***

(a)

If $x_n \rightarrow x$,$|\alpha_{j,n}-\alpha_j| \leq |x_n-x|$,i,e,$\forall \epsilon >0,\exist n \in N^*,s.t. |\alpha_{j,n}-\alpha_j| \leq |x_n-x| <\epsilon$.That is $lim_{n \rightarrow \infin}\alpha_{j,n}=\alpha_j(1\leq j\leq k)$.

Conversely,$\exist N\in N^*,s.t. if \  n\geq N,|\alpha_{j,n}-a{j}|<\frac{\epsilon}{\sqrt{k}}$.

$|x_n-x|=\{\Sigma ^k_{j=1} |\alpha_{j,n} - \alpha_j|^2\}^{1/2} < \epsilon$.So $x_n \rightarrow x$.This prove (a).

(b)

According to Theorem 3.4(a) and Theorem 3.3 we know that (b) holds.



## SUBSEQUENCES

### 3.5 Definition

Given a sequence {$p_n$},consider a sequence {$n_k$} of positive integers,such that $n_1 < n_2 < n_3 < ...$.Then the sequences {$p_{ni}$} is called a subsequence of {$p_n$}.If {$p_n$} converges, the limit is called a subsequential limit of {$p_n$}.



### Remark

{$p_n$} converges to p if and only if every subsequence of {$p_n$} converges to p.

***Proof***

If every subsequence of {$p_n$} converges to p,put $N \in N^*,\forall n>N,p_n \in S_n$,where each $S_n$ converges to p. Thus $\forall \epsilon > 0, |p_n -p|<\epsilon$ .Hence {$p_n$} converges to p.

If {$p_n$} converges to p,$\forall k_n \in N^*,n_i >= n$.Since $\epsilon > 0,\exist N \in N^*,s.t. if\ n > N,|p_n-p|<\epsilon$.Thus $|p_{n_i}-p|<\epsilon$.

Hence  every subsequence of {$p_n$} converges to p.



### 3.6 Theorem

> (a) If {$p_n$} is a sequence in a compact metric space $X$,then some sub-sequence of {$p_n$} converges to a point of $X$.
>
> (b) Every bounded sequence in $R^k$ contains a convergent subsequence.

***Proof***

If there are finitely many points in the sequence,put
$$
p_{n_1}=p_{n_2}=...=p_{n_k}=p
$$
Then {$p_n$} converges to p.

If there are infinitely many points in the sequence,there is a limit point $x_0$ in $X$.Consider a sequence {$x_n$} such that $d(x_n,x_0)<\frac{1}{n}$.Thus {$x_n$} converges to $x_0$.And (a) holds.

Since every bounded sequence in $R^k$ can be covered by a k-cell,apply (a) then (b) follows.



## 3.7 Theorem

The subsequential limits of a sequence {$p_n$} in a metric space $X$ form a closed subset of $X$.

***Proof***

Let $E^*$ be the set of all subsequential limits of {$p_n$} and let q be a limit point of $E^*$.We have to show that $q \in E^*$,i.e. to prove some subsequence converges to q.(连续两次运用极限点定义+度量空间三角不等式)

Choose $n_1$ so that $p_{n_1} \neq q$.(Let $E^*$ has more than one point,otherwise there is nothing left to prove).Put $\delta = d(q,p_{n_1})$.Suppose $n_1,...,n_{i-1}$ are chosen. Since $q$ is a limit point of $E^*$,there is an $x \in E^*$ with $d(x,q) < 2^{-i}\delta$.Since $x \in E^*$,there is an $n_i > n_{i-1}$ such that $d(x,p_{n_i})<2^{-i}\delta,d(q,p_n)\leq d(x,q) + d(x,p_{n_i})<2^{1-i}\delta$ for $i=1,2,3,...$.This says that ${p_{n_i}}$ converges to p.

Thus $q \in E^*$.



## CAUCHY SEQUENCES

### 3.8 Definition

A sequence {$p_n$} in a metric space $X$ is said to be a **Cauchy sequence** if $\forall \epsilon >0$ , $\exist N \in \N^*$ such that $d(p_n,p_m)<\epsilon$ if $n \geq N$ and $m \geq N$.



### 3.9 Definition

Let $E$ be a nonempty subset of a metric space $X$,and let $S$ be the set of all real numbers of the form $d(p,q)$,with $p \in E$ and $q \in E$.The sup of $S$ is called the **diameter** of E.



### Remark

If {$p_n$} is a sequence in $X$ and if $E_N$ consists of the points $P_N,P_{N+1},P_{N+2},...,$it is clear that {$p_n$} is a Cauchy sequence if and only if  $lim_{N\rightarrow \infin}diam(E_n)=0$($\forall \epsilon >0,\exist N \in \N^*,s.t.|E_n|<\epsilon$).



### 3.10 Theorem

> (a) diam $\overline{E}$ = diam $E$.
>
> (b) If $K_n$ is a sequence of **compact** sets in $X$ such that $K_n \supset K_{n+1}$(n=1,2,3,...) and if $lim_{n\rightarrow \infin}diam (K_n) = 0$,then $\cap _1^\infin K_n$ consists of exactly one point.

***Proof***

(a)

It is clear that $diam E \leq diam \overline{E}$,since $E \sub \overline{E}$.

Fix $\epsilon >0,$and choose $p \in \overline{E},q\in \overline{E}$.By the definition of $\overline{E}$,there are points $p',q'$,in $E$ such that $d(p,p')<\epsilon,d(q,q')<\epsilon$.

$d(p,q)\leq d(p,p')+d(q,q')+d(p',q')<2\epsilon + d(p',q')\leq 2\epsilon + diam(E)$.

It follows that $diam \overline{E}\leq diamE+2\epsilon$,i.e.$diam\overline{E} \leq diamE$.

Therefore,$diam E=diam \overline{E}$,(a) is proved.

 (b)

Put $K=\cap^\infin_1 K_n$.Therefore $K$ is not empty.If $K$ has more than one point,then $diam(K)>0$(diam,short for diameter,is the sup of the distance set).Since  $K_n \supset K_{n+1}$,$K_n \supset K, lim_{n\rightarrow \infin}diam (K_n) > 0$,contradicting to the assumption that $diam(K_n) \rightarrow 0$.



### 3.11 Theorem

> (a) In any metric space $X$ ,every **convergent** sequence is a Cauchy sequence.
>
> (b) If X is a **compact** metric space and if {$p_n$} is a Cauchy sequence in $X$,then {$p_n$} **converges** to some point of $X$.
>
> (c) In $R^k$,every Cauchy sequence **converges**.



### Note

收敛的定义和柯西序列的定义的差别在于前者有极限概念显式地参与，后者则没有。

3.11(b)能让我们不知道具体收敛值的情况下判断一个序列是否收敛。

结合3.11(a)与3.11(c)，我们会发现在欧式空间里，柯西序列和收敛序列是**等价**的。这一事实被称为**柯西收敛准则**(Cauchy criterion for convergence).



***Proof***

(a)

If $p_n \rightarrow p$ and if $\epsilon > 0,\exist N \in \N^*,s.t. d(p,p_n) <\epsilon,n \ge N.$Hence $d(p_n,p_m) \leq d(p_n,p)+d(q_m,p) < 2\epsilon$, as soon as $min\{n,m\} \geq N$.Thus {$p_n$} is a Cauchy sequence.



(b)

Let {$p_n$} be a Cauchy sequence in the compact space $X$.Then $lim_{N\rightarrow \infin}diam \overline{E_N}=0$.

Notice that $E_N \supset E_{N+1}$,therefore $\exist p \in X$ lies in every $\overline{E_N}$.

Since the limit of $diam\overline{E_N}$ is zero,it follows that $\exist N \in \N^*,s.t.$ if $n > N,\forall \epsilon >0$,$diam(\overline{E_n})<\epsilon$,i.e.$\forall q \in \overline{E_N}$,$d(p,q)<\epsilon$.

In other words,$d(p,p_n)<\epsilon$.That is $p_n\rightarrow p$.



(c)

Consider a Cauchy sequence {$x_n$},it is obvious that it is bounded and closed.**(*)**

Therefore it is compact.(c) follows from (b).

**(*)**:It is closed cause there is only one limit point in a Cauchy sequence.



### 3.12 Definition

A metric space in which every Cauchy sequence converges is said to be **complete**.



### 3.13 Definition

A sequence {$s_n$} of real numbers is said to be

> (a) monotonically increasing if $s_n \leq s_{n+1} (n=1,2,3,...)$
>
> (b) monotonically decreasing if $s_n \geq s_{n+1}(n=1,2,3,...)$



### 3.14 Theorem

Suppose {$s_n$} is monotonic. Then {$s_n$} converges if and only if it is bounded.



## UPPER AND LOWER LIMITS

### 3.15 Definition

Let {$s_n$} be a sequence of real numbers with the following property:

For every real $M$ there is an integer $N$ such that $n\geq N$ implies $s_n \geq M$.We then write
$$
s_n\rightarrow +\infin.
$$
Similarly,if for every real $M$ there is an integer $N$ such that $n>N$ implies $s_n \leq M$,we write
$$
s_n\rightarrow -\infin.
$$


### 3.16 Definiton

Let {$s_n$} be a sequence of real numbers.Let $E$ be the set of numbers $x$(in the extended real number system) such that $s_{n_k} \rightarrow x$ for some subsequence {$ s_{n_k}$}.This set $E$ contains all subsequential limits as defined in **Definition 3.5** ,plus possibly the numbers $+\infin,-\infin.$



### 3.17 Definition

Let {$s_n$} be a sequence of real numbers.Let $E$ and $s^*$ have the same meaning as in **Definition 3.16**.Then $s^*$ has the following two properties:

> (a) $s^* \in E$.
>
> (b) If $x>s*$,there is an integer $N$ such that $n\geq N$ implies $s_n < x$.

Moreover,$s^*$ is the **only** number with the properties (a) and (b).



### 3.18 Examples



### 3.19 Theorem

If $s_n \leq t_n$ for $n\geq N$,where $N$ is fixed,then

> $lim_{n\rightarrow \infin} inf \ $$s_n$ $\leq$ $lim_{n\rightarrow \infin} inf\ t_n$,
>
> $lim_{n\rightarrow \infin} sup \ s_n\leq lim_{n\rightarrow \infin}sup\ t_n$.



### SOME SPECIAL SEQUENCES

### 3.20 Theorem

> 1. If $p>0$,then $lim_{n\rightarrow \infin}\frac{1}{n^p} = 0$.
> 2. If $p>0,$then $lim_{n\rightarrow \infin} \sqrt[n]{p}=1$.
> 3. $lim_{n\rightarrow \infin} \sqrt[n]{n} = 1$
> 4. If $p > 0$ and $\alpha$ is real,then $lim_{n\rightarrow \infin}\frac{n^\alpha}{(1+p)^n}=0$.
> 5. If $|x| < 1$,then $lim_{n\rightarrow \infin}x^n=0$.



### SERIES

### 3.21 Definition

Given a sequence {$a_n$}, we use the notation
$$
\sum_{n=p}^q a_n
$$
to denote the sum.

With {$a_n$} we denote a sequence {$s_n$},where 
$$
s_n = \sum^n_{k=1}a_k.
$$
For {$s_n$},we use the symbolic expression:
$$
\sum ^{\infin}_{n=1}a_n \tag{1}
$$
The symbol (1) we call an infinite series,or just a series.The numbers $s_n$ are called the **partial sums**  of the series. If {$s_n$} converges to $s$,we say that the series converges,and write
$$
\sum^{\infin}_{n-1}a_n = s.
$$
The number $s$ is called the sum of the series;but it should be clearly understood that $s$ is the **limit** of a sequence of sums,and is **not obtained simply by additions.**



### 3.22 Theorem

$\sum a_n$ converges if and only if for **every** $\epsilon >0$ there is an integer $N$ such that
$$
|\sum^m_{k=n} a_k|\leq \epsilon \tag{2}
$$
if $m\ge n \ge N$.

In particular,by taking $m=n$,(2) becomes
$$
|a_n|\leq \epsilon(n \geq N).
$$


### 3.23 Theorem

If $\sum a_n$ converges,then $lim_{n\rightarrow \infin} a_n = 0$.



### 3.24 Theorem

A series of nonnegative terms converges if and only if its partial sums form a bounded sequence.



### 3.25 Theorem

> $$
> If \ |a_n| \leq c_n\ for\ n\geq N_0,where \ N_0\ is\ some\ fixed\ integer,and\ if\ \sum{c_n}\ converges,then \sum a_n \ converges.\\
> If \ a_n \geq d_n \geq 0 \ for\ n \geq N_0,and\ if\ \sum d_n\ diverges,then \sum a_n\ diverges.
> $$



## SERIES OF NONNEGATIVE TERMS

### 3.26 Theorem

If $0\leq x < 1$,then
$$
\sum^{\infin}_{n=0}x^n=\frac{1}{1-x}
$$
If $x \geq 1$,the series diverges.



### 3.27 Theorem

Suppose $a_1 \ge a_2 \ge a_3 \geq...\geq 0$.Then the series $\sum^{\infin}_{n=1}a_n$ converges if and only if the series
$$
\sum^{\infin}_{k=0}2^k\cdot a_{2^k} = a_1 +2a_2+4a_4+8a_8+...
$$
converges.



### 3.28 Theorem

$\sum \frac{1}{n^p}$ converges if $p>1$ and diverges if $p \leq 1$.



### 3.29 Theorem

If $p>1$,
$$
\sum^{\infin}_{n=2}\frac{1}{n(log\ n)^p}
$$
converges;If $p>1$,the series diverges.



## THE NUMBER e

### 3.30 Definition

$e=\sum^{\infin}_{n=0}\frac{1}{n!}$.



### 3.31 Theorem

$lim(1+\frac{1}{n})^n=e$.



### 3.32 Theorem

$e$ is **irrational**.



### THE ROOTS AND RATIO TESTS

### 3.33 Theorem(Root Test)

Given $\sum a_n$,put $\alpha = lim_{n\rightarrow \infin} sup(\sqrt[n]{|a_n|})$.

Then

> $$
> If\ \alpha <1,\sum a_n\ converges;\\
> If\ \alpha >1,\sum a_n\ diverges;\\
> If\ \alpha =1,the\ test\ gives\ no\ information.
> $$



### 3.34 Theorem(Ratio Test)

The series $\sum a_n$

> $$
> (1)\ converges\ if\ lim_{n\rightarrow \infin}sup|\frac{a_{n+1}}{a_n}|<1,\\
> (2)\ diverges\ if\ |\frac{a_{n+1}}{a_n}| \geq 1\ for\ all\ n\geq n_0,where\ n_0\ is\ some\ fixed\ integer.
> $$



### 3.35 Examples



### 3.36 Remarks



### 3.37 Theorem

For any sequence {$c_n$} of positive numbers,

> $$
> lim_{n\rightarrow \infin} inf(\frac{c_{n+1}}{c_m})\leq lim_{n\rightarrow \infin}inf(\sqrt[n]{c_n}),\\
> lim_{n\rightarrow \infin} sup(\sqrt[n]{c_n})\leq lim_{n\rightarrow \infin}sup\frac{c_{n+1}}{c_n}.
> $$



## POWER SERIES

### 3.38 Definition

Given a sequence {$c_n$} of complex numbers,the series
$$
\sum ^{\infin}_{n=0}c_nz^n
$$
is called a **power series**. The numbers $c_n$ are called the coefficients of the series;$z$ is a complex number.



### 3.39 Theorem

Given the power series $\sum c_n z_n$,put $\alpha = lim_{n\rightarrow \infin}sup(\sqrt[n]{|c_n|}),R=\frac{1}{\alpha}.(If\ \alpha = 0, R = + \infin;if\ \alpha = +\infin,R = 0.)$Then $\sum c_n z^n\ converges\ if\ |z| < R,and \ diverges \ if\ |z|>R.$



### 3.40 Examples



## SUMMATION BY PARTS

### 3.41 Theorem

Given two sequences $\{a_n\},\{b_n\}$,put 
$$
A_n = \sum ^n_{k=0}a_k
$$
$if\ n\geq0;put\ A_{-1}=0.Then,if\ 0\leq p \leq q,we\ have$
$$
\sum^{q}_{n=p}a_nb_n=\sum^{q-1}_{n=p}A_n(b_n-b_{n+1})+A_qb_q-A_{p-1}b_p.
$$


### 3.42 Theorem

Suppose

> 1.  the partial sums $A_n$ of $\sum a_n$ form a bounded sequence;
> 2.  $b_0\geq b_1 \geq b_2 \geq ...$;
> 3.  $lim_{n\rightarrow \infin}b_n = 0$.

Then $\sum a_nb_n$ converges.



### 3.43 Theorem

Suppose

> 1. $|c_1|\geq |c_2| \geq ...$;
> 2. $c_{2m-1}\geq 0,c_{2m}\geq 0\ (m=1,2,3,...)$;
> 3. $lim_{n\rightarrow \infin} c_n = 0$.

Then $\sum c_n$ converges.



### 3.44 Theorem

Suppose the radius of convergence of $\sum c_n z^n$ is 1,and suppose $c_0 \geq c_1 \geq c_2 \geq...$,$lim_{n\rightarrow \infin}c_n = 0$.Then $\sum c_nz^n$ converges at every point on the circle $|z|=1$,except possibly at $z=1$.



### ABSOLUTE CONVERGENCE

The series $\sum a_n$ is said to converge absolutely if the series $\sum|a_n|$ converges.



### 3.45 Theorem

If $\sum a_n$ converges absolutely,then $\sum a_n$converges.



### 3.46 Remarks

If $\sum a_n$ converges,but $\sum |a_n|$ diverges,we say that $\sum a_n$ converges **nonabsolutely**.

For instance,the series
$$
\sum \frac{(-1)^n}{n}
$$
converges nonabsolutely.

The comparison test,as well as the root and ratio tests,is really a test for absolute convergence,and therefore c**annot give any information about nonabsolutely convergent series**. Summation by parts can sometimes be used to handle the latter. In particular,power series converge absolutely in the interior of the circle of convergence.

We shall see that we may operate with absolutely convergent series very much as with finite sums. We may multiply them term  by term and we may change the order in which the additions are carried out,**without affecting the sum of the series.** But for nonabsolutely convergent series this is no longer true,and more care has to be taken when dealing with them.



## ADDITION AND MULTIPLICATION OF SERIES	

### 3.47 Theorem

If $\sum a_n = A,and\ \sum b_n = B,then \sum(a_n+b_n) = A+B$, and $\sum c a_n = cA$,for any fixed c.



### 3.38 Definiton

Given $\sum a_n$ and $\sum b_n$,we put
$$
c_n = \sum^n_{k=0}a_kb_{n-k} (n=0,1,2,...)
$$
and call $\sum c_n$ the product of the two given series.



### 3.49 Example



### 3.50 Theorem

Suppose

> $$
> \begin{aligned}
> &(1) \sum^{\infin}_{n=0} a_0 \ converges\ absolutely,\\
> &(2) \sum^{\infin}_{n=0} a_n =  A,\\
> &(3) \sum^{\infin}_{n=0} b_n =  B,\\
> &(4) c_n =\sum^{n}_{k=0}a_kb_{n-k} (n=0,1,2,...).\\
> \end{aligned}
> $$

Then 
$$
\sum^{\infin}_{n=0}c_n = AB
$$


## REARRANGEMENTS

### 3.52 Definition

Let {$k_n$},n=1,2,3,... be a sequence in which every positive integer appears once and only once(that is ,$\{k_n\}$ is a 1-1 function from $J$ onto $J$.)Putting
$$
a'_n = a_{k_n} (n=1,2,3,...),
$$
we say that $\sum a'_n$ is a rearrangement of $\sum a_n$.



### 3.53 Example



### 3.54 Theorem

Let $\sum a_n$ be  a series of real numbers which converges,but not absolutely.Suppose
$$
-\infin\leq \alpha \leq\beta\leq \infin.
$$
Them there exists a rearrangement $\sum a_n'$ with partial sums $s'n$ such that
$$
lim_{n\rightarrow \infin} inf(s'_n)= \alpha,lim_{n\rightarrow \infin}sup(s'_n)=\beta.
$$


### 3.55 Theorem

If $\sum a_n$ is a series of complex numbers which converges absolutely,then every rearrangement of $\sum a_n$ converges,and they all converge to the same sum. 