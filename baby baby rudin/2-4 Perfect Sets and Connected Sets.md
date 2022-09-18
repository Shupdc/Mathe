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