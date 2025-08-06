# CIFAR-10 Ambiguous Image Classification – Human vs AI Assisted

## Overview
This project compares two approaches for classifying images from the CIFAR-10 dataset and detecting ambiguous samples:
- **Part A:** Human-guided neural network model (manual CNN design)
- **Part B:** Generative AI-assisted model (architecture & hyperparameter suggestions from AI tools)

The goal is to evaluate model performance and analyze the impact of AI in neural network design, specifically focusing on ambiguity detection.

---

## Repository Structure
```
├── data/                 # Sample data files (small subset for testing)
├── models/               # Saved models (partA_model.h5, partB_model.h5)
├── partA/
│   └── partA.ipynb       # Human-guided model notebook
├── partB/
│   └── partB.ipynb       # AI-assisted model notebook
└── README.md             # Project overview and usage instructions
```

---

## Requirements
Install the required dependencies using:
```bash
pip install -r requirements.txt
```

---

## Usage
### Clone Repository
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

### Running Part A (Human-guided)
Open and run:
```bash
jupyter notebook partA/partA.ipynb
```

### Running Part B (AI-assisted)
Open and run:
```bash
jupyter notebook partB/partB.ipynb
```

Both notebooks will:
- Train models
- Save trained models to `/models/` directory
- Generate results and evaluation metrics

---

## Data
- A small subset of CIFAR-10 is included under `/data/` for demonstration.
- Full CIFAR-10 dataset is automatically downloaded via TensorFlow during training if not already present.

---

## Results Summary
- Human-guided model accuracy: ~73%
- AI-assisted model accuracy: ~82%
- Ambiguity detection methods:
  - Part A: Softmax confidence threshold
  - Part B: Entropy-based uncertainty estimation

---

## Notes
- Model files in `/models/` are excluded from GitHub version control using `.gitignore` (to prevent large file issues).
- Use the included sample data only for quick tests. For full training, rely on the dataset loader.

---

## Author
**Vignesh Sankar**  
Coventry University | Module 7154CEM – Artificial Neural Networks