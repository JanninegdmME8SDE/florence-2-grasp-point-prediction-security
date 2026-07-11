
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
├── .git/                                           # Git version control directory
├── .gitignore                                      # Git exclusion rules
├── data/                                           # Raw datasets and threat matrix metadata
│   └── raw/
│       ├── images/              
│       └── metadata_eval.json
├── docs/                                           # Study materials, lab notes, etc. (Local-only)
├── LICENSE                                         # MIT License
├── notebooks/                                      # Evaluation and pipeline notebooks
│   ├── 00_curate_threat_matrix.ipynb               # Threat matrix curation
│   ├── 01_florence2_evaluate_threat_matrix.ipynb   # Zero-shot inference
│   ├── git_commit.ipynb                            # Operational (Local-only)
│   └── setup_and_utils.ipynb                       # Operational (Local-only)
├── outputs/                                        # Metrics, results, and visualizations
│   └── threat_eval_results.json                    # Inference coordinates and bounding boxes
└── README.md                                       # Project documentation
```

## 🤝 Acknowledgements

I am grateful to my brilliant professors, teaching assistants, and cohorts, both former and new, for the learning and collaborative experiences during my studies.

I would like to acknowledge the software development and AI/ML skills I have gained through the course materials provided by the University of Washington. These skills served as the primary theoretical and applied basis for the development of this independent project repository, specifically from the following graduate certificate programs:

* [Graduate Certificate in Software Development Engineering](https://www.tacoma.uw.edu/set/programs/certificates/gcsde) (Cohorts 2024-2025)

* [Graduate Certificate in Artificial Intelligence and Machine Learning for Engineering](https://www.engr.washington.edu/admission/professional-masters-certificates/artificial-intelligence-and-machine-learning-certificate) (Cohorts 2025-2026)

## 📚 Bibliography

[1] M. Hickner, *ENGR 521 A SP 26 Machine Learning for Engineering Project*. UW Canvas: Course Materials, 2026.

[2] M. Hickner, *ENGR 510 A AU 25 Foundations Of Machine Learning For Engineering*. UW Canvas: Course Materials, 2025.

[3] S. Fresca, *ENGR 515 A Wi 26 Data-Driven Optimization*. UW Canvas: Course Materials, 2026.

[4] S. Fresca, *ENGR 520 A Sp 26 Physics-Informed Machine Learning*. UW Canvas: Course Materials, 2026.

[5] S. L. Brunton and J. N. Kutz, *Data-Driven Science and Engineering: Machine Learning, Dynamical Systems, and Control*. Cambridge University Press, 2021.

[6] S. L. Brunton, "Optimization: A Bootcamp for Machine Learning, Inverse Problems, and Control." Course Manuscript, University of Washington, 2025.

[7] P. Rajmohan, P. Alam, and J. G. D. MacGormain, "A Comparative Study of CLIP, Grounding DINO, and Florence-2 for Language-Guided Grasp-Relevant Point Prediction," ENGR 521 A SP 26 Machine Learning for Engineering Project, University of Washington, 2026. [Online]. Available: [comparative study repository](https://github.com/priyagautham28/grasp-point-prediction)

[8] AllenAI, "pixmo-points," Hugging Face, 2024. [Online]. Available: [https://huggingface.co/datasets/allenai/pixmo-points](https://huggingface.co/datasets/allenai/pixmo-points)

[9] B. K. Rameshbabu, S. S. Balakrishna, B. Flynn, V. Kapoor, A. Norton, H. Yanco, and B. Calli, "A Benchmarking Study of Vision-based Robotic Grasping Algorithms," *arXiv preprint arXiv:2503.11163*, 2025. [Online]. Available: [https://arxiv.org/abs/2503.11163](https://arxiv.org/abs/2503.11163)

[10] B. Xiao et al., "Florence-2: Advancing a Unified Representation for a Variety of Vision Tasks," *arXiv preprint arXiv:2311.06242*, 2023. [Online]. Available: [https://arxiv.org/abs/2311.06242](https://arxiv.org/abs/2311.06242)

[11] Ultralytics, "How to Run Microsoft Florence-2 with Ultralytics for Visual Reasoning, OCR & Object Detection Tasks," 2025. [Online]. Available: [YouTube Video](https://www.youtube.com/watch?v=ojoYESWLw5Q) | [Colab Notebook](https://colab.research.google.com/github/ultralytics/notebooks/blob/main/notebooks/how-to-use-florence-2-for-object-detection-image-captioning-ocr-and-segmentation.ipynb) | [GitHub Repo](https://github.com/ultralytics/notebooks/blob/main/notebooks/how-to-use-florence-2-for-object-detection-image-captioning-ocr-and-segmentation.ipynb)

[12] A. Deshpande et al., "GraspMoLMo: Language-Guided Grasp Point Selection with Vision-Language Models," *arXiv preprint arXiv:2505.13441*, 2025. [Online]. Available: [https://arxiv.org/abs/2505.13441](https://arxiv.org/abs/2505.13441)

[13] G. Tziafas and H. Kasaei, "Towards Open-World Grasping with Large Vision-Language Models," *arXiv preprint arXiv:2406.18722*, 2024. [Online]. Available: [https://arxiv.org/abs/2406.18722](https://arxiv.org/abs/2406.18722)

[14] E. Griffor, C. Greer, D. Wollman, and M. Burns, "Framework for Cyber-Physical Systems: Volume 1, Overview," National Institute of Standards and Technology, Gaithersburg, MD, Special Publication (NIST SP) 1500-201, 2017. [Online]. Available: [https://www.nist.gov/publications/framework-cyber-physical-systems-volume-1-overview](https://www.nist.gov/publications/framework-cyber-physical-systems-volume-1-overview)

[15] T. Wang et al., "Exploring the Adversarial Vulnerabilities of Vision-Language-Action Models in Robotics," *arXiv preprint arXiv:2411.13587*, 2025. [Online]. Available: [https://arxiv.org/abs/2411.13587](https://arxiv.org/abs/2411.13587)

[16] T. Wang et al., "Adversarial Robustness in Embodied AI: A Closed-Loop Perspective on Attacks and Defenses," *TechRxiv*, 2026. [Online]. Available: [https://www.techrxiv.org/doi/full/10.36227/techrxiv.177100288.88303656/v1](https://www.techrxiv.org/doi/full/10.36227/techrxiv.177100288.88303656/v1)

[17] B. Tong et al., "Measuring Epistemic Humility in Multimodal Large Language Models," *arXiv preprint arXiv:2509.09658*, 2026. [Online]. Available: [https://arxiv.org/abs/2509.09658](https://arxiv.org/abs/2509.09658)

