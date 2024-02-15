Given a Homogeneous [[Linear ODEs]]:
$$y^n(x)+a_{n-1}y^{n-1}x+...+a_1y'(x)+ay(x)=0$$
Solve with $y=e^{\lambda x}$ and treat like normal equation
e.g.
$$y''+y'-42y=0$$
$$\lambda^2 + \lambda - 42=0$$
$$(\lambda - 6)(\lambda+7) = 0$$
$$\{C_1e^{-7x}+C_2e^{6x}\}$$
Guideline: Guess the solution $y=e^{\lambda x}$, then solve for $\{\lambda_1, \lambda_2, ...\}$

This works if all $\lambda$ are unique. If they are, then use $e^{\lambda x}$

Otherwise, if $\lambda_1=\lambda_k$, then $y_1(x) = e^{\lambda_1 x}$ , $y_2(x)=xe^{\lambda_1x}$, $y_k(x)=x^{k-1}e^{\lambda_1x}$ 

ex:
$$y^5-8y^3+16y'=0$$
$$\lambda^5-8\lambda^3+16\lambda$$
$$\lambda(\lambda^4-8\lambda^2+16)$$
$$\lambda(\lambda^2-4)^2$$
$$\{0, 2, -2, 2, -2\}$$
$$y=C_1e+C_2e^{2x}+C_2xe^{(2x)}+C_3e^{(-2x)}+C_4xe^{(-2x)}$$
If we have complex roots: $\lambda_1=a+bi$ that are distinct: just uses the complex roots. It is correct.
![[Pasted image 20240202141132.png]]
![[Pasted image 20240202141209.png]]
Afterwards, should rewrite the solution using trig.

Solution will be in the form:
$$C_3e^{ax}cos(bx)+C_4e^{ax}sin(bx)$$

To summarize: solve the polynomial for each $\lambda_n$, allowing for complex solutions.
Write $y_1$ to $y_n$ using $\lambda_1$ to $\lambda_n$ with:
1. Distinct real: $y_1=e^{\lambda_1x}$ 
2. Repeated Real: $y_1=e^{\lambda_1x}$ and $y_2=xe^{\lambda_2x}$
3. Distinct complex: $y_1=e^{ax}cos(bx)$ and $y_2=e^{ax}sin(bx)$ 
4. Repeated complex: $y_1=e^{ax}cos(bx)$ and $y_2=e^{ax}sin(bx)$ and$y_3=xe^{ax}cos(bx)$ and $y_4=xe^{ax}sin(bx)$ 