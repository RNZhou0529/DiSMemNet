# DiSMemNet: Structure-Aware Distillation and Memory Network for Generalizable Unsupervised Domain Adaptation in EM Segmentation

## Overview
**DiSMemNet** is a unified **unsupervised domain adaptation (UDA)** framework for **electron microscopy (EM) segmentation**, addressing large domain shifts in contrast, texture, and morphology.  
It combines:
- **Gated contrastive translation** → preserves structural topology  
- **Distillation–memory synergy** → refines pseudo labels and stabilizes training

## Method Highlights
- **Gated Patch-wise Contrastive Loss** — Filters ambiguous negatives, preserves morphological topology.  
- **Mean-Teacher Distillation** — Stabilizes representation learning via EMA-based supervision.  
- **Prototype-Guided Memory Bank** — Refines pseudo-labels with structure-aware retrieval.  
- **Unified Optimization** — Jointly enforces appearance, semantic, and structural consistency.  

## Quick Start
```bash
git clone https://github.com/RNZhou0529/DiSMemNet.git
cd DiSMemNet
pip install -r requirements.txt
```

## Citation
If you find this work useful, please cite:
@article{zhou2025dismemnet,
  title={DiSMemNet: Structure-Aware Distillation and Memory Network for Generalizable Unsupervised Domain Adaptation in EM Segmentation},
  author={Zhou, Ruining and Guo, Jinyue and Jiang, Liuyun and Liu, Jing and Han, Hua},
  year={2025},
  institution={Institute of Automation, Chinese Academy of Sciences}
}
