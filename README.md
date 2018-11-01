# Fitting.jl

<!-- # To do:
- create git repository (done)
- find data (done)
- upload data (done)
- compute all the ne! using YMW16 (done)
- and paramters on notebook, set right units  (done)
- write the likelihood (done)
- produce the mcmc sample (done)
- add a lot of comments in the notebook (done)
- check error on ratio from std (done)
- do plots: strip in the epsilon-m plane (done)
- write readme (introduction done)
- compare exclusion with previous bounds (done)
- include priors (done - prior with better justification? need justificatio of lower bound - 
result is lower bound-dependent - relate mcdm effect with photon mass effect to use photon mass lower bound.
for upper bound look at approximations made)
- write readme (add pictures)

- discuss fit result (more?)
- include other data points?
- write readme (smaller pictures?)

- tag the final commit as "version 1 release"

- add travis (?)
-->

# Signature of millicharged dark matter in pulsar dispersion measure (DM): a Bayesian analysis

The Julia notebook PulsarBayesian was created as part of the Uinversity of Waterloo 2018 Computational Physics course, module II.

In the notebook, we analyze the dispersion measure data from a number of pulsars as a function of their distance. The dispersion measure, which causes a delay between the time of arrival of the pulsar signal in different frequency bands, is usally explained with the presence of ionized plasma in the galactim medium. The standard effect is determined by the density of the electrons integrated along the line of sight. This is what the data looks like for a collection of pulsars from the [ATNF catalogue](http://www.atnf.csiro.au/research/pulsar/psrcat/).

<img src="https://i.imgur.com/AybngWD.png" width="600" height="400">

We make the hypothesis that the dark matter is a particle charged under the electromagnetic field, with charge ![eqn](https://latex.codecogs.com/gif.latex?q=\epsilon&space;e) and mass ![eqn2](https://latex.codecogs.com/gif.latex?m_{\tex{dm}}). The dark matter gives an additional contribution to the dispersion measure. The observational data can thus be used to put constraints on the dark matter parameter space.

We use the emcee Monte Carlo sampler to explore the posterior of the combined data and model. From the sample we obtain constraints at 1, 2 and 3 sigmas, and compare them with other bounds in the literature.

<img src="https://i.imgur.com/WxUYgUn.png" width="500" height="300">

For more information, see the notebook "PulsarBayesian.ipynb". To visualize the notebook online, you can use this [viewer](http://nbviewer.jupyter.org/github/laurasberna/Fitting.jl/blob/master/PulsarBayesian.ipynb). 

# Acknowledgment 

This project was motivited by ongoing research in collaboration with Diego Blas, Andrea Caputo, Miguel Frias, Paolo Pani and Lijing Shao. The ideas detailed here will appear in a future publication.
