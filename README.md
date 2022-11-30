Mess around more with Zotero/Rabbit stuff

# Parallelization Scheme for Modeling Coagulation

## The "Big" Problem

When modeling the time evolution for number densities of particles that experience *coagulation* (or clumping together), this modeling process can be extremely computationally intensive. Right now, the only code that exists for modeling this phenomena is **serial** — often taking up to several days to process on a cluster like USC CARC!

The most famous and relevant equation for describing this number density time evolution of coagulating particles is the **Smoluchowski Coagulation Equation**

$\frac{d}{d t} f_k=\frac{1}{2} \sum_{i+j=k} K(i, j) f_i f_j-\sum_i K(i, k) f_i f_k$

where

* $K$ is…
* $f_i$ is….
* $f_j$ is …

## Importance

Along with modeling coagulation of particles in the atmosphere, this equation is also crucial for aerosols and — most importantly — **interstellar dust**. Because there is no parallelized version for integrated models for this solver, this step has become a bottleneck in the modeling process for coagulation.


## Team Members

* Ziyu Huang
* Kevin Sampson

## Applications

* Interstellar Dust Coagulation


![](https://github.com/DylanUSC/Parallel_Coagulation_Kernel/blob/main/Coagulation_Figure.png)

## Sequential test case: K = 1

K = 1

$N(m, t)=\frac{N_0}{m_0}\left(\frac{2}{N_0 t}\right)^2 \exp \left[\frac{2}{N_0 t}\left(1-\frac{m}{m_0}\right)\right]$

![](https://github.com/DylanUSC/Parallel_Coagulation_Kernel/blob/main/K1_Dustpy.png)


* Cloud condensation in planetary atmospheres



