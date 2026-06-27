
# Florence-2 Grasp Point Prediction Security

[![Florence-2](https://img.shields.io/badge/Florence--2-Microsoft-00A4EF?logo=microsoft&logoColor=white)](https://huggingface.co/microsoft/Florence-2-large) [![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/) [![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/) [![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/) [![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)](https://numpy.org/) [![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/) [![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?logo=scipy&logoColor=white)](https://scipy.org/) [![Matplotlib](https://img.shields.io/badge/Matplotlib-ffffff?logo=matplotlib&logoColor=black)](https://matplotlib.org/) [![Pillow](https://img.shields.io/badge/Pillow-945025)](https://pillow.readthedocs.io/) [![JSON](https://img.shields.io/badge/JSON-000000?logo=json&logoColor=white)](https://www.json.org/) [![ReportLab](https://img.shields.io/badge/ReportLab-002F6C)](https://www.reportlab.com/) [![Google Colab](https://img.shields.io/badge/Colab-F9AB00?logo=googlecolab&logoColor=white)](https://colab.research.google.com/) [![Google Drive](https://img.shields.io/badge/Drive-4285F4?logo=googledrive&logoColor=white)](https://drive.google.com/) [![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white)](https://github.com/)

## 🎯 Project Overview
This is my first public repository among a few of my ongoing personal projects to be shared soon. It is an adapted standalone version following the successful completion of our group ENGR 521 Machine Learning course project. It originally presented a comparative study evaluating three state-of-the-art VLM architectures - **CLIP, Grounding DINO, and Florence-2** - on the task of language-guided **grasp-relevant point prediction** (view the [comparative study repository](https://github.com/priyagautham28/grasp-point-prediction)).

What makes this study unique is that it will focus solely on **Microsoft's Florence-2**, including an implementation of its extended capabilities. Additionally, the project's scope will be modified to analyze the model's performance entirely from a **safety and cybersecurity perspective**. Specifically, this involves investigating how data scarcity (particularly concerning small, textureless objects), semantic perturbations, architectural bottlenecks (e.g., centroid extraction flaws), and spatial localization failures translate into physical risks within **cyber-physical systems (CPS)**.

Recognizing the critical need for [epistemic humility](https://arxiv.org/abs/2509.09658) within AI systems - and adopting that same mindset as researchers - we must acknowledge that modern AI possesses emergent properties and unpredictable behaviors. This project is designed for a broad audience, including students, roboticists, machine learning engineers, cybersecurity practitioners, professionals, and curious individuals. Together we will explore the intersection of physical AI and cybersecurity, and I welcome any feedback to help solidify this research.

🚧 Work in Progress: This repository is currently under active development and data preparation.

## 📁 Project Structure

```text
florence-2-grasp-point-prediction-security/
├── .git/                                 # Git version control directory
├── .gitignore                            # Git exclusion rules
├── data/                                 # Raw datasets and threat matrix metadata
│   └── raw/
│       ├── images/             
│       └── metadata_eval.json
├── docs/                                 # Study materials, lab notes, etc. (Local-only)
├── LICENSE                               # MIT License
├── notebooks/                            # Evaluation and pipeline notebooks
│   ├── 00_curate_threat_matrix.ipynb
│   ├── git_commit.ipynb                  # Operational (Local-only)
│   └── setup_and_utils.ipynb             # Operational (Local-only)
├── outputs/                              # Metrics, results, and visualizations
└── README.md                             # Project documentation
```
