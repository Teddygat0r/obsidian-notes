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
