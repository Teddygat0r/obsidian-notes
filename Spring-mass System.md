Implements [[Non-Homogeneous ODES]]

Model:
- m: mass > 0
- c: damping constant > 0
- k: spring constant > 0
- x(t): displacement from equillibreum point
- x'(t): velocity of system
- x''(t): acceleration

By Newton's Law: $$F=ma = F_{spring}+F_{damping}$$$$-kx-cx'=mx''$$
$$mx''+cx'+kx=0$$

Damped: $c\neq0$

Undamped model, simple harmonic motion:
$$mx''+kx=0$$$$x(t)=C_1cos(\sqrt{\frac{k}{m}}t) + C_2sin(\sqrt{\frac{k}{m}}t)$$
We will want to rewrite this as $Rcos(\omega t-\phi)$
Use ->
$$cos(A-B)=cos(A)cos(B)+sin(A)sin(B)$$

Example:
$$\frac{1}{2}cos(\omega t)+\frac{\sqrt{3}}{2}sin(\omega t)$$
$$cos(\frac{\pi}{3})*cos(\omega t)+\sin(\frac{\pi}{3})*sin(\omega t)$$
$$cos(\omega t-\frac{\pi}{3})$$
![[Pasted image 20240213181411.png]]


Overdamped Case:
$$c^2-4mk>0$$ Real solutions:
$$x_h=c_1e^{\lambda_1t}+c_2e^{\lambda_2t}$$
Both $\lambda < 0$ so $x_n(t)->0 (t->\inf)$


Critically damped:
$$c^2-4mk=0$$