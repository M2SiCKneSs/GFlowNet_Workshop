# Big Data in the Industry: Generative Models & Sampling Workshop

This repository gathers materials—papers, code, slides, and a companion podcast—covering flow‐network generative models (GFlowNets), MCMC and RL–based sampling techniques, and best practices for data‐science project workflows (CRISP-DM). It’s intended as a self-contained workshop bundle and reference library.

## Table of Contents

1. Overview & Themes  
2. Papers & Preprints  
3. Hands-On Code & Notebooks  
4. Slides & Podcast  
5. Getting Started  
6. Citing  

---

## Overview & Themes

- **Generative Flow Networks (GFlowNets):** Learn how to amortize diverse candidate generation via flow-based policies.  
- **Markov Chain & Auxiliary-Variable Sampling:** MCMC methods for discrete and continuous spaces, including local exploration and learned proposals.  
- **Reinforcement-Learning-Driven Sampling:** Off-policy/entropy-regularized RL (PPO, SAC) as samplers.  
- **Project Lifecycle (CRISP-DM):** Standardized template and best practices for end-to-end data science projects.  

---

## Papers & Preprints

| File | Title & Topic |
|:---|:---|
| **9820_flow_network_based_generative_.pdf** | *Flow Network based Generative Models for Non-Iterative Diverse Candidate Generation*<br />Bengio et al. – Introduces GFlowNets for sampling proportional to rewards. |
| **3014_mars_markov_molecular_sampling MCMC3.pdf** | *MARS: Markov Molecular Sampling for Multi-Objective Drug Discovery*<br />Xie et al. – Adaptive fragment-editing MCMC with GNN-based proposals. |
| **grathwohl21a MCMC1.pdf** | *Oops I Took A Gradient: Scalable Sampling for Discrete Distributions*<br />Grathwohl et al. – Gradient-informed Metropolis–Hastings for combinatorial spaces. |
| **NeurIPS-2020-learning-discrete-energy-based-models-via-auxiliary-variable-local-exploration-Paper MCMC2.pdf** | *ALOE: Learning Discrete Energy-based Models via Auxiliary-Variable Local Exploration*<br />Dai et al. – Jointly train an EBM and local-search sampler via a variational power-iteration. |
| **jin18a RL3.pdf** | *Junction Tree Variational Autoencoder for Molecular Graph Generation*<br />Jin et al. – Two-phase VAE: scaffold tree + graph assembly. |
| **1707.06347v2 RL1.pdf** | *Proximal Policy Optimization Algorithms*<br />Schulman et al. – Clip-based PPO for stable on-policy RL. |
| **haarnoja18b RL2.pdf** | *Soft Actor-Critic: Off-Policy Maximum-Entropy Deep Reinforcement Learning with a Stochastic Actor*<br />Haarnoja et al. – Sample-efficient, stable off-policy max-ent RL. |
| **bengio20a (limitation 2).pdf** | *Interference and Generalization in Temporal Difference Learning*<br />Bengio et al. – TD learning’s generalization/interference dynamics. |
| **913_implicit_under_parameterizatio (limitation 1).pdf** | *Implicit Under-Parameterization Inhibits Data-Efficient Deep Reinforcement Learning*<br />Kumar et al. – How rank-collapse in bootstrapped TD degrades sample efficiency. |
| **HW – CRISP-DM Howtodo.pdf** | *How-To Guide: Applying the CRISP-DM Process Model*<br />Step-by-step best practices for business understanding through deployment. |
| **HW1 – Template.docx** | *CRISP-DM Project Template*<br />Editable Word template covering all six CRISP-DM phases.|

---

## Hands-On Code & Notebooks

- **Data_Science_GFN (1).ipynb**  
  - A Jupyter notebook illustrating GFlowNet training on a toy domain.  
  - **Requirements:** Python 3.8+, PyTorch, RDKit, NetworkX.  
  - **Usage:**  
    ```bash
    pip install -r requirements.txt
    jupyter lab Data_Science_GFN\ \(1\).ipynb
    ```  

---

## Slides & Podcast

- **workshop.pptx**  
  - Slide deck summarizing motivation, methods (GFlowNet ● MCMC ● PPO/SAC), and CRISP-DM.  

- **gflownet_podcast.wav**  
  - A 30 min narrated overview of generative flow networks: history, key concepts, and future directions.

---

## Getting Started

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your‐org/big-data‐industry.git
   cd big-data-industry
   ```  
2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   # RDKit, torch, numpy, jupyter, networkx, matplotlib, scipy...
   ```  
3. **Explore the GFlowNet notebook**  
   ```bash
   jupyter lab Data_Science_GFN\ \(1\).ipynb
   ```  
4. **Review slides**  
   Open **workshop.pptx** in PowerPoint or your viewer of choice.  
5. **Listen to the podcast**  
   Any WAV-capable player:  
   ```bash
   afplay gflownet_podcast.wav   # macOS
   play gflownet_podcast.wav     # sox on Linux
   ```  

---

## Citing

If you use any of these materials in your research, please cite the original papers:

```bibtex
@inproceedings{bengio2021gflownet,
  title={Flow Network based Generative Models for Non-Iterative Diverse Candidate Generation},
  author={Bengio, Emmanuel et al.},
  booktitle={NeurIPS},
  year={2021}
}

@inproceedings{xie2021mars,
  title={MARS: Markov Molecular Sampling for Multi-Objective Drug Discovery},
  author={Xie, Yutong et al.},
  booktitle={ICLR},
  year={2021}
}

@article{grathwohl2021oops,
  title={Oops I Took A Gradient: Scalable Sampling for Discrete Distributions},
  author={Grathwohl, Will et al.},
  year={2021}
}

@inproceedings{dai2020aloe,
  title={Learning Discrete Energy-based Models via Auxiliary-Variable Local Exploration},
  author={Dai, Hanjun et al.},
  booktitle={NeurIPS},
  year={2020}
}

@inproceedings{jin2018junction,
  title={Junction Tree Variational Autoencoder for Molecular Graph Generation},
  author={Jin, Wengong et al.},
  booktitle={ICML},
  year={2018}
}

@article{schulman2017ppo,
  title={Proximal Policy Optimization Algorithms},
  author={Schulman, John et al.},
  journal={arXiv preprint arXiv:1707.06347},
  year={2017}
}

@inproceedings{haarnoja2018sac,
  title={Soft Actor-Critic: Off-Policy Maximum Entropy Deep Reinforcement Learning},
  author={Haarnoja, Tuomas et al.},
  booktitle={ICML},
  year={2018}
}

@article{bengio2020interference,
  title={Interference and Generalization in Temporal Difference Learning},
  author={Bengio, Emmanuel et al.},
  journal={ICML},
  year={2020}
}
```
