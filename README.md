# PyKet - A Python Framework for Variational Monte-Carlo Simulation based on Tensorflow

PyKet is our framework for running variational Monte-Carlo simulations of quantum many-body systems. It supports any Keras model for representing a parameterized unnormalized wave-function, e.g., Restricted Boltzman Machines and ConvNets, with real or complex-valued parameters. We have implemented a standard Markov-Chain Monte-Carlo (MCMC) energy gradient estimator for this general case, which can be used to approximate the ground state of a quantum system according to a given Hamiltonian. The neural-network-based approach for representing wave-fucntions was shown to be a promising method for solving the many-body problem, often matching or even surpassing the precision of other competing methods.

In addition to an MCMC energy gradient estimator, we have also implemented our novel Neural Autoregressive Quantum State wave-function representation that supports efficient and exact sampling. By overcoming the reliance on MCMC, our models can converge much faster for models of same size, which allows us to scale them to millions of parameters, as opposed to just a few thousands for prior approaches. This leads to better precison and ability to invesitgate larger and more intricated systems. Please read our paper (cited below) for further details on our approach. We hope that users of our library will be able to take our method and apply to a variety of problems. If you use this codebase or apply our method, we would appreciate if you cite us as follows:
```
@article{sharir2019NAQS,
  title = {Deep autoregressive models for the efficient variational simulation of many-body quantum systems},
  author = {Sharir, Or and Levine, Yoav and Wies, Noam and Carleo, Giuseppe and Shashua, Amnon},
  journal = {arXiv preprint arXiv:1902.04057},
  year = "2019",
  month = "Feb"
}
```

## Basic Tutorial

While we are working on writing a proper tutorial on using the framework, we suggest going through the example files.
