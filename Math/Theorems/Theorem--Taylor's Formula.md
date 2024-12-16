---  
### 3, Taylor’s Formula  
  
From the amount of differential calculus that has been explained up to this point, one may obtain the correct impression that the more derivatives of two functions coincide (inclusive of zeroth order) at a point, the better these functions approximate each other in a neighborhood of that point.  
  
An algebraic polynomial can be expressed as:  
$$  
P_n(x) = P_n(x_0) + \frac{P_n^{(1)}(x_0)}{1!}(x - x_0) + \ldots + \frac{P_n^{(n)}(x_0)}{n!}(x - x_0)^n,  
$$  
where $c_k = \frac{P_n^{(k)}(x_0)}{k!}$.  
  **Note: If you want to check the higher order derivatives of Pn s in single and complicated forms, refer to [[Definition--Derivative Calculation]].**
#### **Definition**  
The algebraic polynomial given by:  
$$  
P_n(x_0; x) = P_n(x_0) + \frac{P_n^{(1)}(x_0)}{1!}(x - x_0) + \ldots + \frac{P_n^{(n)}(x_0)}{n!}(x - x_0)^n,  
$$  
is called the **Taylor polynomial of order $n$** of $f(x)$ at $x_0$.  
  
  
**Theorem**:  
If the function $f(x)$ is continuous on the closed interval with endpoints $x_0$ and $x$, and it has a derivative of order $n+1$ at the interior points of this interval, then for any function $\varphi$ that is continuous on this closed interval and has a nonzero derivative at its interior points, there exists a point $\xi$ between $x_0$ and $x$ such that:  
$$  
r_n(x_0; x) = \frac{\varphi(x) - \varphi(x_0)}{\varphi'(\xi)} \cdot \frac{f^{(n+1)}(\xi)}{n!}(x - \xi)^n.  
$$  
---  
**Auxiliary Function \( F(t) \)**  
  
To analyze the behavior of the remainder in Taylor's theorem, we introduce an auxiliary function \( F(t) \), which helps derive expressions for the error term in Taylor series expansions.  
  
  
**Let**:  
$$  
F(t) = f(x) - \left[ f(x_0) + \frac{f^{(1)}(x_0)}{1!}(x - x_0) + \frac{f^{(2)}(x_0)}{2!}(x - x_0)^2 + \cdots + \frac{f^{(n)}(x_0)}{n!}(x - x_0)^n \right].  
$$  
  
Equivalently, \( F(t) \) can be written as:  
$$  
F(t) = f(x) - \sum_{k=0}^n \frac{f^{(k)}(x_0)}{k!}(x - x_0)^k.  
$$  
  
Here, \( F(t) \) represents the difference between the actual function value \( f(x) \) and the Taylor polynomial $P_n(x_0; x)$ of degree $n$ at $x_0$.  
  
---  
  
**Purpose of \( F(t) \):**  
The function \( F(t) \) is constructed to isolate the error term in Taylor expansions. By analyzing \( F(t) \), we can precisely determine the behavior of the remainder term $r_n(x_0; x)$, which quantifies the difference between \( f(x) \) and its Taylor polynomial approximation.  
  
**Expression for \( F(t) \) Including the Remainder:**  
Rewriting \( F(t) \) to explicitly include the remainder term:  
$$  
F(t) = r_n(x_0; x),  
$$  
where:  
$$  
r_n(x_0; x) = f(x) - P_n(x_0; x).  
$$  
  
Using the remainder formula, we can express \( F(t) \) in terms of the higher-order derivatives of \( f(x) \).  
  
---  
  
**Analysis of \( F(t) \) Using Cauchy’s Theorem:**  
Using Cauchy’s finite-increment theorem, we can write the remainder in terms of \( F(t) \) and analyze its behavior:  
1. \( F(t) \) satisfies the conditions of continuity and differentiability in the interval $[x_0, x]$.  
2. The derivative \( F'(t) \) includes higher-order terms, which we analyze to deduce properties of the remainder.  
  
The critical property derived from \( F(t) \) is:  
$$  
F'(t) = f^{(n+1)}(\xi) \cdot \frac{(x - \xi)^n}{n!},  
$$  
where $\xi \in [x_0, x]$. This leads to the **Cauchy form** and **Lagrange form** of the Taylor series remainder.  
**Cauchy form**：$r_{n}(x_{0};x)=\frac{1}{n!}f^{n+1}(\xi)(x-\xi)^{n}(x-x_{0})$；  
**Lagrange form**：$r_{n}(x_{0};x)=\frac{1}{(n+1)!}f^{n+1}(\xi)(x-x_{0})^{n+1}$.  
  
---  
#### Specific Examples and convergence of Taylor series  
**Example 1**:$$e^{x}=1+\frac{1}{1!}x+\frac{1}{2!}x^{2}+\ldots+\frac{1}{n!}x_{n}+r_{n}(x)$$ and the remainder is $$r_{n}(0;x)=\frac{1}{(n+1)!}e^{\xi}\cdot x^{n+1}\rightarrow0$$which indicates that in the sum of series the remainder could be omitted.  
  
---  
**Example 2**:  
Given that $$f(x)=\sin x,f^{n}(x)=\sin(x+\frac{\pi}{2}n)$$ we could estimate the remainder of the sine function as$$r_{n}(0;x)=\frac{1}{(n+1)!}\sin(\xi+\frac{\pi}{2}n+1)x^{n+1}.$$Which also tends to zero.  
  
---  
**Example 3:**$$\ln(1+x)=x-\frac{1}{2}x^{2}+\ldots+\frac{(-1)^{n-1}}{n}x^{n}$$In this Taylor formula ,the remainder should be $$r_{n}(0;x)=\frac{1}{n!}\frac{(-1)^{n}n!}{(1+\xi)^{n}}\cdot(x-\xi)^{n}x$$thus, while the absolute value of x is lower than 1, then$$|\frac{x-\xi}{1+\xi}|\leq\frac{|x|-|\xi|}{1-|\xi|}\leq x$$,and the remainder would converge to zero.  
If not, then the remainder would not be convergent, meaning that the approximation of Taylor’s formula is inaccurate.  
  
---  
#### Taylor’s formula in local intervals  

  Let E be a closed interval having x0 ∈ R as an endpoint. If the function f : E → R has derivatives  $f^{\prime}(x_0)$, ... ,$f^{n}(x_0)$ up to order n inclusive at the point x0, then the following representation holds:
  $f(x) = f(x_{0})+ \frac{f^{\prime}(x0)}{1!} (x-x_{0})+ ... + \frac{f^{n}(x0)}{n!} (x-x_{0})^{n} + o((x-x_0)^{n})$
  So the remainder here should be theinfinitesimal bounded polynominals.
  See [[Definition--infinitesimal&Ultimate bounded (o and O)]].
  
---
We would like to give some simple examples about common functions:

$e^{x}= 1+\frac1{1!}x+\frac1{2!}x^{2}+...+\frac1{n!}x^{n}+O(x^{n+1}) \ or\  o(x^n).$
cosx
coshx
ln(1+x)
(1+x)^\alpha





