We are interested in a probability distribution $\rho:X \rightarrow \mathbb R_+$, such that

 1.  (Constraints) $ d_i^{-1} (\rho d\mathcal L ) =  \mathbb P_i$, i.e. $\forall B \subseteq \mathbb R $  we have $\int 1_{\{d_i(x) \in B \} }\rho(x) d \mathcal L(x) = \mathbb P_i(B)$. 
 2. (Optimization problem) $\int \rho \log \rho d\mathcal L$ extremal - this expression maximizes entropy under the constraints. This takes account to the fact that less is known about the actual distribution of the probability of presence.
 

To assure positivity we set $\rho = e^\varphi$ and obtain $\rho \log \rho = \varphi e^\varphi$ for the entropy. For simplicity we assume for $\mathbb P_i$ only discrete probabilities $\mathbb P_i = \sum_k p_{i,k} \delta_{x_{i,k}}$

The Gâteaux differential $D^{Gâteaux}$ in direction $\psi$ is given by $\partial_h F(\varphi + h\psi)\mid_{h=0}$

$$ 0 = D^{Gâteaux} \left( \int  -\varphi e^\varphi + \sum_i \lambda_i \sum_k p_{i,k} \delta_{x_{i,k}}\cdot 1_{d_i^{-1} (p_{i,k})} e^\varphi  d\mathcal L \right)(\varphi; \psi) \\
= \partial_h \int -(\varphi + h\psi) e^{\varphi + h\psi} + \sum_{i,k} \lambda_{i,k}' e^{\varphi + h\psi}  \cdot  1_{d_i^{-1} (p_{i,k})}d\mathcal L \\
=-\int \psi e^\varphi \left(1 + \varphi - \sum_{i,k} \lambda_{i,k}' \cdot  1_{d_i^{-1} (p_{i,k})} \right) d\mathcal L \\$$

The last bracket has to be zero (a.e.) because $\psi$ is of arbitrary choice and $e^\varphi \ne 0$.

Absorbing '+1' in the $\lambda$'s leads to the condition

  $$\exists \lambda_{i,k} : \varphi - \sum_{i,k}  \lambda_{i,k}''\cdot  1_{d_i^{-1} (p_{i,k})} = 0$$
