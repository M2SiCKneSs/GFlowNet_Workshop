# Big Data in the Industry: Generative Models & Sampling Workshop

This repository gathers materials—papers, code, slides, and a companion podcast—covering flow‐network generative models (GFlowNets), MCMC and RL–based sampling techniques, and best practices for data‐science project workflows (CRISP-DM). It’s intended as a self-contained workshop bundle and reference library.

## Table of Contents

1. Overview & Themes  
2. Hands-On Code & Notebooks  
3. Slides & Podcast  
4. Getting Started  
5. Citing  

---

## Overview & Themes

- **Generative Flow Networks (GFlowNets):** Learn how to amortize diverse candidate generation via flow-based policies.  
- **Markov Chain & Auxiliary-Variable Sampling:** MCMC methods for discrete and continuous spaces, including local exploration and learned proposals.  
- **Reinforcement-Learning-Driven Sampling:** Off-policy/entropy-regularized RL (PPO, SAC) as samplers.  
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
  - https://drive.google.com/drive/folders/19gn9aSz9y4OwB8DE_LcSVSgk_z3AULgI?usp=sharing

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
