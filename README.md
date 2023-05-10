#  A Numerical Solution for the Black-Scholes Equation.

This project provides a numerical solution for the Black-Scholes equation, a partial differential equation that describes the price dynamics of European call or put options.

The solution is obtained using the [**finite difference method**](https://en.wikipedia.org/wiki/Finite_difference_method) with an explicit scheme.
This is a method for solving partial differential equations by approximating derivatives using finite differences.

## The Black-Scholes Equation

$$ V_{t}+1/2σ^{2}S^{2}V_{ss}+rsV_{S}-rV = 0, \quad S \in (0, S_{max}), \quad t \in (0, 1) $$

$V$ - is the option price

$S$ - is the underlying asset price

$\sigma$ - is the volatility of the asset

$r$ - is the risk-free interest rate

$t$ - is time


#### Boundary Condition
$$ V(0, t) = 0, \quad t>0 $$

$$ V(S_{max},t) = S_{max}- Ke^{r(1 −t)} \quad t>0$$


#### Initial Condition

$$ V(S,1) = \max(S-K,0) \quad S \in [0,S_{max}] $$ 


&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;

Here below there is a 3D plot that presents an example solution of the Black-Scholes equation:

![](https://github.com/DawOp/Black-Scholes-Equation/blob/main/solution-plot.png)
