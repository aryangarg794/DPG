# Implementation of COPDAQ-Q from [1]
--------------------------------------

The policy it learns is suboptimal (agent attempts to stay still to minimize cost). I suspect this happens due to one of two reasons. 

1. The behaviour policy $\beta(a | s)$ doesn't manage to solve the problem. This results in a suboptimal policy as the only way to maximize the reward is by standing still (or close to it). 
2. The math/implementation is wrong. In the paper they use tile coding for $\phi(s)$, which may prove to be quite important. (To check) Also, the implementation of $\phi(s,a)$ could also be incorrect since I saw differing definitions. 


[1] Silver, D., Lever, G., Heess, N., Degris, T., Wierstra, D., & Riedmiller, M. (2014). Deterministic policy gradient algorithms. In International Conference on Machine Learning (pp. 387-395). PMLR.