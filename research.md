---
layout: single
title: "Publications"
permalink: /research/
author_profile: true
---

### [Statistical Inference under Adaptive Sampling with LinUCB](https://arxiv.org/pdf/2512.00222)
  - **Wei Fan**\*, Kevin Tan\*, Yuting Wei (\* equal contribution)
  - Preprint, 2025  
<details>
  <summary><strong>Abstract</strong></summary>
  Adaptively collected data has become ubiquitous within modern practice. However, even seemingly benign adaptive sampling schemes can introduce severe biases, rendering traditional statistical inference tools inapplicable. This can be mitigated by a property called stability, which states that if the rate at which an algorithm takes actions converges to a deterministic limit, one can expect that certain parameters are asymptotically normal. Building on a recent line of work for the multi-armed bandit setting, we show that the linear upper confidence bound (LinUCB) algorithm for linear bandits satisfies this property. In doing so, we painstakingly characterize the behavior of the eigenvalues and eigenvectors of the random design feature covariance matrix in the setting where the action set is the unit ball, showing that it decomposes into a rank-one direction that locks onto the true parameter and an almost-isotropic bulk that grows at a predictable $\sqrt{T}$ rate. This allows us to establish a central limit theorem for the LinUCB algorithm, establishing asymptotic normality for the limiting distribution of the estimation error where the convergence occurs at a $T^{-1/4}$ rate. The resulting Wald-type confidence sets and hypothesis tests do not depend on the feature covariance matrix and are asymptotically tighter than existing nonasymptotic confidence sets. Numerical simulations corroborate our findings.
</details>



---

### [Actor-Critics Can Achieve Optimal Sample Efficiency](https://arxiv.org/pdf/2505.03710)
  - Kevin Tan\*, **Wei Fan**\*, Yuting Wei (\* equal contribution)
  - In Forty-second International Conference on Machine Learning, 2025 
<details>
  <summary><strong>Abstract</strong></summary>
  Actor-critic algorithms have become a cornerstone in reinforcement learning (RL), leveraging the strengths of both policy-based and value-based methods. Despite recent progress in understanding their statistical efficiency, no existing work has successfully learned an $\epsilon$-optimal policy with a sample complexity of $O(1/\epsilon^2)$ trajectories with general function approximation when strategic exploration is necessary.
  We address this open problem by introducing a novel actor-critic algorithm that attains a sample-complexity of $O(dH^5 \log|\mathcal{A}|/\epsilon^2 + d H^4 \log|\mathcal{F}|/ \epsilon^2)$ trajectories, and accompanying $\sqrt{T}$ regret when the Bellman eluder dimension $d$ does not increase with $T$ at more than a $\log T$ rate.
  Here, $\mathcal{F}$ is the critic function class, $\mathcal{A}$ is the action space, and $H$ is the horizon in the finite horizon MDP setting. Our algorithm integrates optimism, off-policy critic estimation targeting the optimal Q-function, and rare-switching policy resets.
  We extend this to the setting of Hybrid RL, showing that initializing the critic with offline data yields sample efficiency gains compared to purely offline or online RL. Further, utilizing access to offline data, we provide a \textit{non-optimistic} provably efficient actor-critic algorithm that only additionally requires $N_{\text{off}} \geq c_{\text{off}}^*dH^4/\epsilon^2$ in exchange for omitting optimism, where $c_{\text{off}}^*$ is the single-policy concentrability coefficient and $N_{\text{off}}$ is the number of offline samples. This addresses another open problem in the literature. We further provide numerical experiments to support our theoretical findings.
</details>

---

### [Hybrid reinforcement learning breaks sample size barriers in linear MDPs](https://arxiv.org/pdf/2408.04526)
  - Kevin Tan, **Wei Fan**, Yuting Wei
  - In Advances in Neural Information Processing Systems, 2024  
<details>
  <summary><strong>Abstract</strong></summary>
  Hybrid Reinforcement Learning (RL), where an agent learns from both an offline dataset and online explorations in an unknown environment, has garnered significant recent interest. 
    A crucial question posed by \cite{xie2022policy} is whether hybrid RL can improve upon the existing lower bounds established in purely offline and purely online RL without relying on the single-policy concentrability assumption. 
    While \cite{li2023reward} provided an affirmative answer to this question in the tabular PAC RL case, the question remains unsettled for both the regret-minimizing RL case and the non-tabular case. 
    In this work, building upon recent advancements in offline RL and reward-agnostic exploration, we develop computationally efficient algorithms for both PAC and regret-minimizing RL with linear function approximation, without single-policy concentrability. 
    We demonstrate that these algorithms achieve sharper error or regret bounds that are no worse than, and can improve on, the optimal sample complexity in offline RL (the first algorithm, for PAC RL) and online RL (the second algorithm, for regret-minimizing RL) in linear Markov decision processes (MDPs), regardless of the quality of the behavior policy. 
    To our knowledge, this work establishes the tightest theoretical guarantees currently available for hybrid RL in linear MDPs.
</details>

---

### [Approximate message passing from random initialization with applications to $Z_2$ synchronization](https://www.pnas.org/doi/abs/10.1073/pnas.2302930120)
  - Gen Li, Wei Fan, Yuting Wei
  - Proceedings of the National Academy of Sciences, 2023
<details>
  <summary><strong>Abstract</strong></summary>
This paper is concerned with the problem of reconstructing an unknown rank-one matrix with prior structural information from noisy observations. While computing the Bayes optimal estimator is intractable in general due to the requirement of computing high-dimensional integrations/summations, Approximate Message Passing (AMP) emerges as an efficient first-order method to approximate the Bayes optimal estimator. However, the theoretical underpinnings of AMP remain largely unavailable when it starts from random initialization, a scheme of critical practical utility. Focusing on a prototypical model called $Z_2$ synchronization, we characterize the finite-sample dynamics of AMP from random initialization, uncovering its rapid global convergence. Our theory—which is nonasymptotic in nature—in this model unveils the nonnecessity of a careful initialization for the success of AMP.
</details>

---

### [A hyperbolic divergence based nonparametric test for two-sample multivariate distributions](https://onlinelibrary.wiley.com/doi/full/10.1002/cjs.11736)
  - Roulin Wang, Wei Fan, Xueqin Wang
  - Canadian Journal of Statistics, 2022
<details>
  <summary><strong>Abstract</strong></summary>
Two-sample hypothesis testing, as a fundamental problem in statistical inference, seeks to detect the difference between two probability measures and has numerous real-world applications. Current test procedures for multivariate two-sample problems typically rely on angles and lengths in a Euclidean space, or lengths in a unit hypersphere after representing data with the spherical model. This article introduces a hyperbolic divergence based on hyperbolic lengths in hyperbolic geometry, as well as a subsequent nonparametric approach to testing the multivariate two-sample problem. We investigate the properties of our test procedure and discover that our hyperbolic divergence statistic is strongly consistent and consistent against all other alternatives; we also demonstrate that its limit distribution is an infinite mixture of $\chi^2$ distributions under the null hypothesis and a normal distribution under the alternative hypothesis. To calculate the p-value, we employ the permutation method. Furthermore, in numerical studies, we compare our method with several nonparametric procedures under various distributional assumptions and alternatives. We discover that our test procedure has some advantages when the distributions' complex correlation structures differ. Finally, we examine one real data set to show how our method can be used to test two-sample heterogeneity.
</details>

