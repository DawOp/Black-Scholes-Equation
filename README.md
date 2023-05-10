# The Black-Scholes equation for European options.

$$ V_{t}+1/2σ^{2}S^{2}V_{ss}+rsV_{S}-rV = 0, \quad S \in (0, S_{max}), \quad t \in (0, 1) $$

$V$ - is the option price

$S$ - is the underlying asset price

$\sigma$ - is the volatility of the asset

$r$ - is the risk-free interest rate

$t$ - is time
#### Boundary condition
$$ V(0, t) = 0, \quad t>0 $$

$$ V(S_{max},t) = S_{max}- Ke^{r(1 −t)} \quad t>0$$
#### Initial condition

$$ V(S,1) = \max(S-K,0) \quad S \in [0,S_{max}] $$

