# PremiUm CNN: Propagating Uncertainty Towards Robust Convolutional Neural Networks

Introduction: 

Deep neural networks (DNNs) have surpassed human-level accuracy in various learning tasks. However, unlike humans who have a natural cognitive intuition for probabilities, DNNs cannot express their uncertainty in the output decisions. This limits the deployment of DNNs in mission-critical domains, such as warfighter decision-making or medical diagnosis.
Bayesian inference provides a principled approach to reason about model's uncertainty by estimating the posterior distribution of the unknown parameters. The challenge in DNNs remains the multi-layer stages of non-linearities, which make the propagation of high-dimensional distributions mathematically intractable. This paper establishes the theoretical and algorithmic foundations of uncertainty or belief propagation by developing new deep learning models named PremiUm-CNNs (Propagating Uncertainty in Convolutional Neural Networks). 
We introduce a tensor normal distribution as a prior over convolutional kernels and estimate the variational posterior by maximizing the evidence lower bound (ELBO). 
We start by deriving the first-order mean-covariance propagation framework. Later, we develop a framework based on the unscented transformation (correct at least up to the second-order) that propagates \textit{sigma points} of the variational distribution through layers of a CNN. The propagated covariance of the predictive distribution captures uncertainty in the output decision. Comprehensive experiments conducted on diverse benchmark datasets demonstrate: 1) superior robustness against noise and adversarial attacks, 2) self-assessment through predictive uncertainty that increases quickly with increasing levels of noise or attacks, and 3) an ability to detect a targeted attack from ambient noise.


Citation:

If this is useful for your work, please cite our paper:

Dimah Dera, Nidhal C. Bouaynaya, Ghulam Rasool, Roman Shterenberg and Hassan M Fathallah Shaykh, “PremiUm-CNN: Propagating Uncertainty towards Robust Convolutional Neural 
Networks,” IEEE Transactions on Signal Processing, 2021 (under review). 
