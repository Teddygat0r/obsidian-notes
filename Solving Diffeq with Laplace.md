Given $f^{(n)}$ is a piecewise continuous function, we can define:
$$L\{f^{(n)}\}=s^nF(s)-s^{n-1}f(0)-s^{n-2}f'(0)-...-sf^{n-2}(0)-f^{(n-1)}(0)$$
For second order differentials:
$$L\{y'\}=sY(s)-y(0)$$
$$L\{y^{''}\}=s^2Y(s)-sy(0)-y'(0)$$
We need initial conditions at t=0

To solve a non-homogeneous differential equation:
$$y''-10y'+9y=5t, y(0)=-1, y'(0)=2$$
1. Take the laplace transform of everything. 
2. Plug in the initial conditions for everything
3. Solve for $Y(s)$
4. Perform reverse laplace transform, usually with partial fraction decomposition.
$$s^2Y(s)-sy(0)-y'(0)-10sY(s)+10y(0)+9Y(s)=\frac{5}{s^2}$$
$$s^2Y(s)+s-2-10sY(s)-10+9Y(s)=\frac{5}{s^2}$$
$$(s^2-10+9)Y(s)+s-12=\frac{5}{s^2}$$
$$(s^2-10+9)Y(s)=\frac{5}{s^2}-s+12$$
$$Y(s)=\frac{-s^3+12s^2+5}{s^4-10s^3+9s^2}$$
$$s^4-10s^3+9s^2=s^2(s-9)(s-1)$$
$$\frac{-s^3+12s^2+5}{s^4-10s^3+9s^2}=\frac{As+B}{s^2}+\frac{C}{s-9}+\frac{D}{s-1}$$
$$-s^3+12s^2+5=(As+B)(s-9)(s-1)+C(s^2)(s-1)+D(s^2)(s-9)$$
If $s=0$
$$5=(B)(-9)(-1)$$
$$B=\frac{5}{9}$$
If $s=1$
$$16=D(-8)$$
$$D=-2$$
If $s=9$
$$-729+12*81+5=248=C(81)(8)$$
$$C=\frac{31}{81}$$
$$A+C+D=-1$$
$$A=\frac{50}{81}$$
$$Y(s)=\frac{\frac{50}{81}s+\frac{5}{9}}{s^2}+\frac{\frac{31}{81}}{s-9}+\frac{-2}{s-1}$$
$$y(t)=\frac{50}{81}+\frac{5}{9}t+\frac{31}{81}e^{9t}-2e^{-t}$$