# Q-PEARL Adapter for Low-Resolution Face Recognition
Q-PEARL-based low-resolution face recognition framework for robust and adaptive recognition under degraded conditions.
# Q-PEARL: Embedding-Space Adaptation for Native Low-Resolution Face Recognition

This repository provides the reproducibility materials for the paper:

**Q-PEARL: Embedding-Space Adaptation with Fusion and Reranking for Native Low-Resolution Face Recognition**

Q-PEARL is a parameter-efficient low-resolution face recognition framework that operates on cached 512-dimensional embeddings extracted from a frozen AdaFace+ARoFace ResNet-100 backbone. The backbone is not modified or fine-tuned. The repository is intended to support evaluation reproducibility, including verification evaluation, TinyFace identity-disjoint split files, hyperparameter configuration, inference settings, and ablation scripts.

## Repository Contents

```text
Q-PEARL/
│
├── README.md
├── requirements.txt
│
├── configs/
│   └── qpearl_final.yaml
│
├── splits/
│   ├── tinyface_dev_identities.txt
│   ├── tinyface_test_identities.txt
│   ├── lfw_pairs.txt
│   └── xqlfw_pairs.txt
│
├── scripts/
│   ├── extract_embeddings.py
│   ├── evaluate_verification.py
│   ├── evaluate_tinyface.py
│   ├── run_hyperparameter_search.py
│   ├── run_ablation.py
│   └── compute_statistics.py
│
├── results/
│   └── expected_results.md
│
└── docs/
    └── reproduction_instructions.md
