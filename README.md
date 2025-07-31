**Read me**
**Overview
**This work proposes a hybrid classification framework that integrates handcrafted features (LBP, GLCM, color, wavelet, morphological) and deep learning features (EfficientNet-B0) using a transformer-based attention fusion mechanism, combined with adaptive incremental learning. The framework aims to address robustness and generalizability challenges in histopathological image classification for lung and colon cancers.

**Key Features
✅ Modified EfficientNet-B0 backbone for deep feature extraction
✅ Classical handcrafted feature extraction (GLCM, LBP, color, wavelet, morphological descriptors)
✅ Transformer-based attention mechanism for feature fusion
✅ Adaptive incremental learning to simulate clinical data acquisition
✅ Validation across LC25000, NCT-CRC-HE-100K, and HMU-GC-HE-30K datasets
✅ Comprehensive performance metrics (accuracy, precision, recall, F1, AUC, Kappa)

**Folder Structure**
Transformer-Fusion/
├── Transformer Fusion.ipynb        # Main training and evaluation script
├── feature_extraction.py           # Handcrafted feature extraction utilities
├── transformer_fusion_layer.py     # Custom transformer-based fusion module
├── utils.py                        # Preprocessing, metric computation
├── requirements.txt                # Python dependencies
├── README.md                       # This documentation file
└── datasets/
    ├── LC25000/                    # Preprocessed lung & colon dataset
    ├── NCT-CRC-HE-100K/            # Validation dataset 1
    └── HMU-GC-HE-30K/              # Validation dataset 2
Datasets Used
**1. LC25000 Dataset**
- Description: Lung and colon cancer histopathology dataset (5 classes × 5,000 images)
- Source: https://arxiv.org/abs/1912.12142
- Citation: Borkowski AA, Bui MM, Thomas LB, Wilson CP, DeLand LA, Mastorides SM. "Lung and Colon Cancer Histopathological Image Dataset (LC25000)." arXiv:1912.12142, 2019.
**2. NCT-CRC-HE-100K Dataset**
- Description: 100,000 colorectal cancer tissue patches
- Source: https://doi.org/10.5281/zenodo.1214456
- Citation: Kather JN, Halama N, Marx A. "100,000 Histological Images of Human Colorectal Cancer and Healthy Tissue." Zenodo, 2018. DOI: 10.5281/zenodo.1214456
**3. HMU-GC-HE-30K Dataset**
- Description: 30,000 gastric cancer histopathological images
- Source: https://www.kaggle.com/datasets/monogoku/hmu-gc-he-30k-gastric-cancer-histopathological
- Citation: Khan I. "HMU-GC-HE-30K: Gastric Cancer Histopathological Dataset", Kaggle, 2023.

**Performance Summary**
•	| Dataset           | Accuracy | Precision | Recall | F1-Score | Kappa |
•	| LC25000           | 99.87%   | 0.999     | 0.999  | 0.999    | 0.998  |
•	| NCT-CRC-HE-100K   | 98.67%   | 0.985     | 0.986  | 0.985    | 0.983  |
•	| HMU-GC-HE-30K     | 98.44%   | 0.984     | 0.983  | 0.984    | 0.980  |

**License and Usage Statement**
The code and scripts provided in this repository are shared under the MIT License, permitting free use, modification, and distribution for academic and research purposes, provided appropriate citation is given.
Researchers are encouraged to reference this work in any derived research to acknowledge the original contribution:
Anusha M, et al. Fusion of Classical and Deep Learning Features with Incremental Learning for Improved Classification of Lung and Colon Cancer, 2025. GitHub Repository
The associated datasets (LC25000, NCT-CRC-HE-100K, and HMU-GC-HE-30K) are publicly available under their respective licenses and ethical usage guidelines, and have been appropriately cited in both the manuscript and repository.

**Acknowledgements**
We gratefully acknowledge the public dataset providers and the community for enabling open research.

**Contact**
For queries or collaborations, please contact:
Ms. Anusha Mullakuri
Email:mullakurianusha@gmail.com
Affiliation: JNTUA
