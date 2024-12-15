(1)Calculate the limit of the following functions:
  
(a)$\lim_{x\to0}(\frac1{\ln(1+x)}-\frac1x)$  
**Note: we should use Taylor's Formula on local exponentials to expand and combine the polynominals.**
Notice that on local intervals, $ln(1+x) = x - \frac{x^{2}}{2} + O(x^3)$.
So we could expand the given function as: $\frac1{\ln(1+x)} - \frac1x = \frac1x(\frac1{1-\frac{x}2+O(x^2)}-1)$.
since x is arbitrarily small, we have: $\frac1{\ln(1+x)} - \frac1x = \frac1x(1 + \frac{x}2 + O(x^2)-1)$
Thus, the value of the limit is $\frac1{2}$.

(b) $\lim _{x\to 0} ( \frac {\sin x}x) ^{\frac 1{1- \cos x}}$  
$\begin{gathered}  \begin{aligned}   & \lim_{x\to0}(\frac{\sin x}{x})^{\frac{1}{1-\cos x}} \\   & =(1-\frac{x^{2}}{6}+O(x^{4}))^{\frac{1}{x^{2}}}  \end{aligned} \\  =e(\frac{2}{x^{2}}l_{n}(1-\frac{x^{2}}{6}+O(x^{4}))) \\  =e[\frac{2}{x^{2}}\cdot(-\frac{x^{2}}{6}+O(x^{4}))] \\  =e^{-\frac{1}{3}}  \end{gathered}$

(c)$\lim_{x\to+\infty} x^{\frac1x}$  
$\operatorname*{lim}_{x\rightarrow+\infty}x^{\frac{1}{x}} = e^{x^{-1}\ln x} = e^{0} = 1$.

(d$){lim}_{x\to0}(\frac1{\sin^2x}-\frac1{x^2})$  
$\operatorname*{lim}_{x\rightarrow0}\left(\frac{1}{\sin^{2}x}-\frac{1}{x^{2}}\right) = \frac{1}{x^{2}}\left(\frac{1}{1-\frac{x^{2}}{3}+0(x^{4})}-1\right) = \frac{1}{3}$.
[[Theorem--Taylor's Formula]]

---
(2)Given the coefficient number $h$,set the function $f(x)=\frac h{\sqrt{\pi}}e^{-h^2x^2}$ exists a turning point $x=\pm\sigma$, solve the value of $h$.
**Note: turning point indicates a local maximum or minimum.**
$f^{\prime}(x)=\frac{h}{\sqrt{\pi}}(-2h^{2}x)e^{-h^{2}x^{2}}=-\frac{2h^{3}x}{\sqrt{\pi}}e^{-h^{2}x^{2}}$
So when$x=\pm\sigma,f^{\prime\prime}(x)=-\frac{2h^{3}}{\sqrt{\pi}}e^{-h^{2}x^{2}}(1-2h^{2}x^{2})=0$, the value of h should be $h = \pm\frac{\sqrt2}{2\sigma}$.
[[Definition--Analytic]]

---
(3)Set that funtion $f:(a,b)\to\mathbb{R}$ is differentiable，$[c,d]\subset(a,b)$, and it satisfies that $f^\prime(c)<f^{\prime}(d)$. Prove that $\forall\eta,f^\prime(c)<\eta< f^{\prime}(d)$ ,exists a point $\xi\in(c,d)$, such that $f^\prime(\xi)=\eta.$
$\begin{gathered} g(x)=f(x)-\eta x \\ g^{\prime}(x)=f^{\prime}(x)-y \\ \begin{cases} g(c)<0 \\ g(d)>0 & \end{cases}  \\ g^{\prime}(-\xi)=0\Rightarrow f^{\prime}(\xi)=n \end{gathered}.$
**Maybe we could apply the mean value theorem, but we could not figure out the continuity of the auxiliary function.**
[[Theorem--Lipschitz Continuity]]

___
(4)Given a function $f:(a,b)\to\mathbb{R}$ which satifies $f(x)>0,\forall x\in(a,b)$, set that $\forall c\in\mathbb{R}$,$e^cxf(x)$is the convex function on $(a,b)$，Prove that: $\ln f(x)$ is also a convex function on this field.
Set $g_{c}(x)=e^{cx}f(x)$.
  
Since this function is convex, $g_{c}^{\prime\prime}(x)\geq0$.
  
$g_{c}^{\prime}(x)=(ce^{cx}f(x)+e^{cx}f(x))$  
  
$g_{c}^{\prime\prime}(x)=e^{cx}(c^{2}f(x)+2cf^{\prime}(x)+f^{\prime\prime}(x))\geq0$.
  
Since that $(\ln f(x))^{\prime\prime}=\frac{f^{\prime\prime}(x)f(x)-f^{\prime}(x)^{2}}{f(x)^{2}}$.
  
Given the second order derivative of g , we could get the inequation$4e^{2}f(x)\cdot f^{\prime\prime}(x)\geq4f^{\prime}(x)^{2}c^{2}$. 
  
So$(\ln f(x))^{\prime\prime}\geq0$, proof.
[[Definition--Analytic]]

___
(5) $f: [ 0, 1] \to \mathbb{R}$is a continous function，and $f(0)=0$,Prove that there exists a continous convex function $g:[0,1]\to \mathbb{R}$ such that $g(0)=0$ and $g(x)\geq f(x),\forall x\in[0,1].$  
I have no clue qaq
___

(6) Prove the ineuqlities given below:  
  
$$\begin{aligned}&\:(a\sin^{2}x+b\cos^{2}x)^{2}\leq a^{2}\sin^{2}x+b^{2}\cos^{2}x.
\end{aligned}$$$$\begin{aligned}&\left(1+\frac{c}{a+b}\right)^{m}+\left(1+\frac{b}{a+c}\right)^{m}+\left(1+\frac{a}{b+c}\right)^{m}\geq\frac{3^{m+1}}{2^{m}}, a,b,c,m>0.\end{aligned}$$
(a) :
$\begin{gathered} u=\sin^{2}x \\ (au+b(1-u))^{2}\leq a^{2}u^{2}+b^{2}(1-u)^{2} \\ 2f(a-b)u+(a-b)^{2}u^{2}\leq(a^{2}-b^{2})u \\ 2b+(a-b)u\leq a+b \\ \therefore u\in[-1,1],proof. \end{gathered}$.
(b): firstly set three polyniminals as $x,y,z$ . We could get that their sum is bigger than $\frac3{2}$.
$\begin{gathered} \begin{array}{cc} To\ prove\ that(1+x)^{m}+(1+y)^{m}+(1+z)^{m}\geq\frac{3^{mn+1}}{2^{m}}=3\left(\frac{3}{2}\right)^{m} \\ Construct \\ \frac{(1+x)^{m}+(1+y)^{m}+(1+z)^{m}}{3} \geq\left(1+\frac{x+y+z}{3}\right)^{m}, \\ f(x)=(1+x)^{m} \end{array} \end{gathered}$.
And the constructed inequality below is trivial.
[[Theorem--Inequality Formulae]]