# Formula Summary (Extracted from index.html)

This file summarizes the physics formulas used by the interactive calculation using LaTeX blocks.

## 1) Relativistic Factor

$$
\gamma = \frac{1}{\sqrt{1-v^2}}
$$

Here, $v$ is normalized by $c$, so $0 \le v < 1$.

## 2) Lorentz Transform (x-direction)

Forward transform used in code (from $S$ to $S'$):

$$
k_x' = \gamma\left(k_x - v\omega\right),
\qquad
\omega' = \gamma\left(\omega - v k_x\right)
$$

## 3) Drude Dielectric Model (normalized)

$$
\varepsilon(\omega) = 1 - \frac{1}{\omega^2}
$$

The code uses normalized units with $\omega_p = 1$.

## 4) Surface-Plasmon Dispersion Magnitude

$$
k_t(\omega) = |\omega|\,\sqrt{\frac{\varepsilon(\omega)}{1+\varepsilon(\omega)}}
$$

The code limits the branch to $|\omega| < 1/\sqrt{2}$.

## 5) Inverse SP Formula (\omega from k_t)

$$
\omega^2 = \frac{1 + 2k_t^2 - \sqrt{1+4k_t^4}}{2},
\qquad
\omega = \sqrt{\omega^2}
$$

## 6) Bulk-Medium Dispersion Used in the App

2D form:

$$
\omega = \pm\frac{|k_x|}{n}
$$

3D magnitude form:

$$
|\omega| = \frac{k_t}{n},
\qquad
k_t = \sqrt{k_x^2 + k_y^2}
$$

## 7) Emitter Relations

In $S$ frame (line/plane):

$$
\omega = v k_x + \frac{\omega_0}{\gamma}
$$

In $S'$ frame (line/plane):

$$
\omega' = \omega_0
$$

## 8) Intersection Equations Solved Numerically

The app finds roots (bisection) for intersections between emitter relations and medium dispersion.

For SP in $S$ frame, with sign branches $s, s_k \in \{+1,-1\}$:

$$
F(\omega) = v\,\big(s_k\,k_t(\omega)\big) + \frac{\omega_0}{\gamma} - s\,\omega = 0
$$

For SP in $S'$ frame:

$$
F(\omega) = \gamma\Big(s\,\omega - v\,\big(s_k\,k_t(\omega)\big)\Big) - \omega_0 = 0
$$

For bulk mode, analogous branch equations are solved against

$$
\omega = \pm\frac{|k_x|}{n}
$$

## Notes on Normalization

The code is dimensionless. In particular, velocity is $v/c$ and frequencies in SP mode are normalized by $\omega_p$.
