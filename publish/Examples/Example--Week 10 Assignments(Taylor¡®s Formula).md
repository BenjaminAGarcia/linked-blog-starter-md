## Assignments for the tenth week  
---  
  
****(1) Calculate the Taylor expression of the following functions：  
  
(a) Expand $\sin(\sin(x))$ at **$x=0$ to $x^3$**  
**To solve this series of questions, we could firstly list the Local Taylor’s Formula of each part of the compound function, then calculate the value by combination.**  
**Since the formula is**  
$$  
\begin{aligned}  
f(x) & =f(x_{0})+\frac{f^{\prime}(x_{0})}{1!}(x-x_{0})+\cdots+\frac{f^{(n)}(x_{0})}{n!}(x-x_{0})^{n}+ \\  
& +o\left((x-x_{0})^{n}\right) \text{ as } x\to x_{0},x\in E,  
\end{aligned}  
$$  
**we could perform the calculation processes.**  
  
The Taylor expansion of $\sin(x)$ at $x = 0$ is:  
$$  
\sin(x) = x - \frac{x^3}{6} + \frac{x^5}{120} - \cdots  
$$  
  
Substitute $y = \sin(x)$, then expand $\sin(y)$ again at $y = 0$:  
$$  
\sin(y) = y - \frac{y^3}{6} + \cdots  
$$  
  
Substitute $y = x - \frac{x^3}{6} + \cdots$:  
$$  
\sin(\sin(x)) = \left(x - \frac{x^3}{6}\right) - \frac{1}{6}\left(x - \frac{x^3}{6}\right)^3 + \cdots  
$$  
  
Simplify up to $x^3$:  
$$  
\sin(\sin(x)) \approx x - \frac{x^3}{3}.  
$$  
  
---  
  
(b) Expand $\sqrt[3]{\sin(x^3)}$ at $x=0$ to include $x^{13}$  
  
Expand $\sin(x^3)$:  
$$  
\sin(x^3) = x^3 - \frac{x^9}{6} + \frac{x^{15}}{120} - \cdots  
$$Compute the cube root:  
$$  
\sqrt[3]{\sin(x^3)} = x \left(1 - \frac{x^6}{6} + \cdots\right)^{1/3}.  
$$  
Using the binomial expansion： $(1 + z)^{1/3}$ where $z = -\frac{x^6}{6}$:  
$$  
\sqrt[3]{\sin(x^3)} = x - \frac{x^7}{18} - \frac{x^{13}}{324} + \cdots.  
$$  
  
---  
  
(c) Expand $\ln\frac{\sin(x)}{x}$ at $x=0$ to include $x^6$  
  
Expand $\frac{\sin(x)}{x}$:  
$$  
\frac{\sin(x)}{x} = 1 - \frac{x^2}{6} + \frac{x^4}{120} - \frac{x^6}{5040} + \cdots.  
$$  
Use the expansion $\ln(1 + z) = z - \frac{z^2}{2} + \frac{z^3}{3} - \cdots$, where $z = -\frac{x^2}{6} + \frac{x^4}{120} - \cdots$:  
$$  
\ln\left(\frac{\sin(x)}{x}\right) = -\frac{x^2}{6} - \frac{x^4}{180} - \frac{x^6}{2835} + \cdots.  
$$  
  
---  
  
(d) Expand $e^{2x} - x^2$ at $x=0$ to include $x^5$  
  
Expand $e^{2x}$:  
$$  
e^{2x} = 1 + 2x + 2x^2 + \frac{4x^3}{3} + \frac{2x^4}{3} + \frac{8x^5}{15} + \cdots.  
$$  
Subtract $x^2$:  
$$  
e^{2x} - x^2 = 1 + 2x + x^2 + \frac{4x^3}{3} + \frac{2x^4}{3} + \frac{8x^5}{15} + \cdots.  
$$  
  
  
---  
****(2) Set $f$ to be two order derivative on the interval $[0,2]$, and $|f(x)|\leq1,|f^{\prime\prime}(x)|\leq1$, prove that    
  
$$  
  
|f'(x)|\leq2,\:\forall x\in[0,2].  
  
$$  
  
**The function is Lipschitz continuous on the interval. After proving this, set a point where the derivative reaches its limit to assume the maximum.**  
**Proof**: The function is Lipschitz continuous on $[0,2]$: since $|f''(x)| \leq 1$. For any $x, y \in [0,2]$:  
$$  
|f'(x) - f'(y)| = \left|\int_y^x f''(t) dt\right| \leq \int_y^x |f''(t)| dt \leq |x - y| \leq 2.  
$$Let $x_0 \in [0,2]$ such that $|f'(x_0)| = \max(|f'(x)|)$. For $f(x)$:  
$$  
|f(x)| \leq 1 \quad \implies \quad |f'(x_0)| \leq \frac{|f(x_0)| + |f(x)|}{|x - x_0|}.  
$$  
  
3. By considering the endpoints, $|x - x_0| \leq 2$, and $|f(x)| \leq 1$, so:  
$$  
|f'(x)| \leq 2.  
$$  
Or using Taylor’s formula:  
𝑓(0) = 𝑓(𝑥1) − 𝑓′(𝑥1) ⋅ 𝑥1 + 𝑓′′(𝜉1)  
2  
2 𝑥1  
𝑓(2) = 𝑓(𝑥1) + 𝑓′(𝑥1) ⋅ (2 − 𝑥1) + 𝑓′′(𝜉1)  
2 (2 − 𝑥1)2  
𝑓(2) − 𝑓(0) = 2𝑓′(𝑥1) + 𝑓′′(𝑥1) ⋅ (2 − 2𝑥1)  
2𝑓′(𝑥1) = 𝑓(2) − 𝑓(0) − 𝑓′′(𝑥1) ⋅ (2 − 𝑥1) ≤ 4  
𝑓′(𝑥1) ≤ 2  
  
---  
**** (3) Prove that $f(x) = \frac{x}{e^x - 1}$ satisfies that the Taylor’s formula at $x=0$ has its coefficient numbers as all rational numbers.  
  
**Proof**: Write $f(x)$ as:  
$$  
f(x) = \frac{x}{x \left(1 + \frac{x}{2} + \frac{x^2}{6} + \cdots\right)} = \frac{1}{1 + \frac{x}{2} + \frac{x^2}{6} + \cdots}.  
$$  
  
Use the series expansion for $\frac{1}{1 + z}$, where:  
$$  
\frac{1}{1 + z} = 1 - z + z^2 - z^3 + \cdots \quad \text{for } |z| < 1.  
$$Here, $z = \frac{x}{2} + \frac{x^2}{6} + \cdots$. Substitute $z$ to get:  
$$  
\frac{1}{1 + \frac{x}{2} + \frac{x^2}{6} + \cdots} = 1 - \left(\frac{x}{2} + \frac{x^2}{6}\right) + \left(\frac{x}{2} + \frac{x^2}{6}\right)^2 - \cdots.  
$$  
  
Each coefficient in the expansion of $f(x)$ is rational because all operations (division, addition, multiplication) involve rational numbers. The factorials in the denominator ensure that the coefficients remain rational.  
Or we could combine the countdown， we could give a combination of a two Taylor’s formulae and the coefficients should all be rational numbers.[[Approach to Analysis - Auxiliary]]  
  
---  
(4)prove that :  
  
$$  
M_1^2 \leq 2M_0 \cdot M_2,  
$$  
  
where:  
- $M_0$ is the maximum value of the function $|f(x)|$,  
- $M_1$ is the maximum value of the first derivative $|f'(x)|$,  
- $M_2$ is the maximum value of the second derivative $|f''(x)|$.  
  
**The proof should be constructed using the relationship between $f'(x)$ and $f''(x)$.**  
  
---  
So introduce the Taylor’s expansion of $f(x+h)andf(x-h)$.By adding two expressions, we could fine the relationship among three coefficients.  
  
---  
**Class quizzes:**  
1, $f^{\prime\prime}(0)exists,f^{\prime}(0)=f(0)=0$.Calculate $\operatorname*{lim}_{x\rightarrow0}\frac{f(x)}{x^{2}}$.  
Set x0 in the neighborhood of zero.  
$f(x_{0})=\frac{f^{\prime\prime}(x_{0})\cdot x_{0}^{2}}{2}$;  
$\frac{f(x_{0})}{x_{0}^{2}}=\frac{f^{\prime\prime}(x_{0})}{2}$.  
DO NOT USE L’HOSPITAL WITHOUT HESITATION  
2,$D\in[a,b],f^{\prime}(\frac{a+b}{2})=0$. Prove that $\exists\xi\in(a,b),|f^{\prime\prime}(\xi)|\geq\frac{4}{(b-a)^{2}}|f(b)-f(a)|$.  
Apply Taylor Expansion of $f(a)andf(b)$ on $\frac{a+b}{2}$.  
3, $D = [a,b],f^{\prime\prime\prime}(x)exists$.Prove that $f(b)-f(a)=f^{\prime}(\frac{a+b}{2})(b-a)+\frac{f^{(3)}(c)(b-a)^{3}}{24}$.  
Applying the similar expansion pattern, we have  
$f(a)-f(b)=f(\cdots+\frac{f^{(3)}(\xi_{1})(b-a)^{3}}{12}+\cdots$  
Or ,we could apply a similar auxiliary thought of the proof of Lagrange’s theorem.  
Set $g(x)=f(x)-f(a)-f^{\prime}(\cdots)-\frac{k}{24}(x-a)^{3}$.  
So $g(a)=g(b)=0$.  
According to Rolle’s theorem, $g^{\prime}(\xi)=f^{\prime}(\xi)-\frac{1}{2}f^{\prime\prime}(\frac{a+\xi}{2})(\xi-a)-\ldots$ equals to zero.  
Set $f^{\prime}(\xi)=f^{\prime}(\frac{a+\xi}{2})+\frac{f^{\prime\prime}(\frac{a+\xi}{2})(\xi-a)}{2}+\ldots$,we could conclude that  
K points to a three order derivative.[[Approach to Analysis - Auxiliary]]