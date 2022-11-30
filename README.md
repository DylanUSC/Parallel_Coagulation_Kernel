# Parallel_Coagulation_Kernel

## Smoluchowski Equation


\begin{equation}

\begin{aligned}
\frac{\partial}{\partial t} N(m)=& \int_0^{\infty} \int_0^{m^{\prime}} M\left(m, m^{\prime}, m^{\prime \prime}\right) N\left(m^{\prime}\right) N\left(m^{\prime \prime}\right) K\left(m^{\prime}, m^{\prime \prime}\right) \mathrm{d} m^{\prime \prime} \mathrm{d} m^{\prime} \\
&-N(m) \int_0^{\infty} N\left(m^{\prime}\right) K\left(m, m^{\prime}\right) \mathrm{d} m^{\prime}
\end{aligned}

\end{equation}

## Team Members

* Ziyu Huang
* Kevin Sampson

## Applications

* Interstellar Dust Coagulation

![](https://cdn.mathpix.com/snip/images/Eu4yxLc9s6z63egH3isWv5x9V2HI-d3NQZTiYeQifxU.original.fullsize.png)

## Sequential test case: K = 1

K = 1

$N(m, t)=\frac{N_0}{m_0}\left(\frac{2}{N_0 t}\right)^2 \exp \left[\frac{2}{N_0 t}\left(1-\frac{m}{m_0}\right)\right]$

![](https://github.com/DylanUSC/Parallel_Coagulation_Kernel/blob/main/K1_Dustpy.png)


* Cloud condensation in planetary atmospheres



