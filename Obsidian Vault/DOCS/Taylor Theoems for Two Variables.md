# Taylor Theoems for Two Variables
2023-04-15 | 11:43
{Subject}:[[MTHS 211]]
{Section}:[[14.0 Partial Derivatives]]
{Tags}: #Mathematics #Calculus 
{Related}:

--- 
Single variable Taylor series:
Provided a power series representation for the function $f(x)$ about $x=a$ exists the Taylor Series for $f(x)$ about $x=a$ is:
$$
f(x)=f(a)+\frac{f^{\prime}(a)}{1 !}(x-a)+\frac{f(a)}{2 !}(x-a)^2+\frac{f^{\prime}(a)}{3 !}(x-a)^3+\cdots=\sum_{k=0}^{\infty} \frac{f^{(k)}(a)}{k !}(x-a)^k
$$
The function $f(x)$ should be infinitely differentiable at point $a$
Multi variable Taylor series:
Let $f$ be an infinitely differentiable function in some open neighborhood around $(x, y)=(a, b)$, then:
$$
f(x, y)=f(a, b)+f_x(a, b)(x-a)+f_y(a, b)(y-b)+\frac{1}{2 !} f_{x x}(a, b)(x-a)^2+\frac{1}{2 !} f_{y y}(a, b)(x-b)^2+f_{x y}(a, b)(x-a)(y-b) \ldots
$$
Linear approximation in multiple variables: Take the constant and linear terms from the Taylor series. In a neighborhood of $(x, y)=(a, b)$
$$
f(x, y) \approx f(a, b)+f_x(a, b)(x-a)+f_y(a, b)(y-b)
$$
--- 
{Efundi Lecture Notes}:https://efundi.nwu.ac.za/access/content/group/4c4529f0-7790-4dc7-9390-8f7cd29c9a77/2021/English/Lecture%20Notes/MTHS211%20-%20Lecture%208%20-%20Taylor%E2%80%99s%20Theorem.pdf