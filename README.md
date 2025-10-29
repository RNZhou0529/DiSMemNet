# DiSMemNet: Structure-Aware Distillation and Memory Network for Generalizable Unsupervised Domain Adaptation in EM Segmentation

## Abstract
Deep learning has greatly advanced electron microscopy (EM) segmentation, yet supervised models remain limited by costly voxel annotations and poor generalization across datasets with large domain shifts in contrast, texture, and morphology. These discrepancies distort both appearance and organelle topology, making structure-preserving adaptation essential for reliable EM analysis. To address this challenge, we propose DiSMemNet, a unified framework for unsupervised domain adaptation (UDA) that jointly enhances appearance–structure alignment and cross-domain generalization. The framework consists of two synergistic modules: a gated contrastive translation module that preserves morphological continuity during adversarial alignment, and a distillation–memory synergy module that stabilizes pseudo-label learning via multi-scale distillation and prototype-guided refinement. Through unified optimization of semantic, structural, and appearance consistency, DiSMemNet achieves topology-preserving adaptation and stable convergence across diverse EM domains. Extensive experiments on MitoADWT, SynADWT, and Lucchi datasets demonstrate that DiSMemNet achieves state-of-the-art performance, yielding sharper boundaries, continuous structures, and strong generalization without target annotations. The results highlight its potential as a structure-aware and domain-robust framework for large-scale EM segmentation.
## Keywords
Unsupervised Domain Adaptation, EM Segmentation, Knowledge Distillation, Memory Bank, Contrastive Learning

## Method Highlights
- We propose DiSMemNet, a unified UDA framework that integrates adversarial alignment, memory refinement, and multi-scale distillation for robust EM segmentation without target labels.
- The gate-controlled contrastive loss enhances both appearance and structural alignment through spatial consistency and foreground weighting, suppressing irrelevant regions and preserving topology.
- A memory-assisted refinement module retrieves structure-aware prototypes and works jointly with multi-level knowledge distillation, enabling stable pseudo-label correction and strong cross-domain generalization.

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
