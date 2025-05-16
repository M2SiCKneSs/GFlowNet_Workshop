# Big Data in the Industry: Generative Models & Sampling Workshop

This repository gathers materials—papers, code, slides, and a companion podcast—covering flow‐network generative models (GFlowNets), MCMC and RL–based sampling techniques, and best practices for data‐science project workflows (CRISP-DM). It’s intended as a self-contained workshop bundle and reference library.

## Table of Contents

1. Overview & Themes  
2. Hands-On Code & Notebooks  
3. Slides & Podcast  
4. Getting Started  

---

## Overview & Themes

- **Generative Flow Networks (GFlowNets):** Learn how to amortize diverse candidate generation via flow-based policies.  
- **Markov Chain & Auxiliary-Variable Sampling:** MCMC methods for discrete and continuous spaces, including local exploration and learned proposals.  
- **Reinforcement-Learning-Driven Sampling:** Off-policy/entropy-regularized RL (PPO, SAC) as samplers.  
---

## Hands-On Code & Notebooks

- **GFlowNet_tutorial_oct_2022.ipynb**  
  - A Jupyter notebook of a tutorial for a toy enviroment of a smiley face.
  - Link: https://colab.research.google.com/drive/1fUMwgu2OhYpQagpzU5mhe9_Esib3Q2VR 

- **Data_Science_GFN_workshop.ipynb**  
  - A Jupyter notebook illustrating GFlowNet training on a toy domain.  
  - **Requirements:** Python 3.8+, PyTorch, RDKit, NetworkX.
  - Link: https://colab.research.google.com/drive/1jDlLOemfQJEr2kUHbdR2zkV6wvpkWzyB?authuser=1
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

### Citing
If you use any of these materials in your research, please cite the original paper.
```
