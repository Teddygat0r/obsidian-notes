Solutions to other odes [[Linear ODEs]]

Given a non-homogeneous ODE:
$$a_ny^n(x)+a_{n-1}y^{n-1}(x)+...+a_0y(x)=f(x)$$

By Theorem 2 [[Linear ODEs]]:
There must be a solution such:
$$C_1y_1+C_2y_2+...C_ny_n+y_p$$
Mostly similar to the homogeneous ODE, with $y_p$ from the non-homogeneous part.

How to find $y_p$?
- Guess $y_p$ from f(x) with undefined coefficients.
- Plug in and solve for $y_p$

How to guess number very good professional :thumbsup:

| $f(x)$ | $y_p(x)$ |
| ---- | ---- |
| Polynomial of size n | $a_nx^n+...a_1x+a_0$ |
| $ke^{\alpha x}$ | $Ae^{\alpha x}$ |
| $k_1cos(\beta x)+k_2sin(\beta x)$ | $Acos(\beta x)+Bsin(\beta x)$ |
| $f_1(x) * f_2(x)$ | $y_{p1}(x)*y_{p2}(x)$ |
| If $y_p$ has a common term with $y_n$ | Reguess $y_{pnew}=y_p*x^n$  |
| If $f(x)=f_1(x)+f_2(x)$ | $y_{p_1new}(x)+y_{p_2new}(x)$ |
![[Pasted image 20240205204741.png]]