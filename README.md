# P2M2
This is a set of examples that showcase the power of probabilistic programs for model and parameter inference in mechanistic models: ODE,DAE,DDE, PDE etc. It uses PyMC3 as a backend and its powerful implementation of the SMC sampler which is a particle based MCMC method that also gives an estimate of the model marginal likelihood (used for calculating BAyes Factor) and thus can be used to infer the posterior distributions of the parameters as well as Bayesian model selection. 

This gives us the unique abitlty to define any mechanistic model in any language (as long as that model can called in python) and use the powerful PyMC3 library to just press the inference button. This essentially frees the modeller from the task of wrting, debugging and testing bespoke inference algorithms.
