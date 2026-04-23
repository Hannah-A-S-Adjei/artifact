## Included Scenarios

- Scenario 1: Targeted Guessing (`scenario1/`)
- Scenario 2: List-wise / chooser attacker (`scenario2/`)
- Scenario 3: Multi-account attacks (trawling and targeted) (`scenario3/`)
  
---

# Scenario 1 Artifact: Targeted Password Guessing

This repository contains the artifact for **Scenario 1 (Targeted Password Guessing)** from our CCS submission. It enables reproducibility of the evaluation pipeline using a synthetic dataset.

---

## 📌 Description

This artifact provides:

- End-to-end pipeline for targeted password guessing  
- Pretrained models (no retraining required)  
- Precomputed evaluation outputs  

**Privacy Note:**  
The original dataset contains sensitive PII and cannot be shared due to ethical restrictions.  
A small synthetic dataset (4 users) is included to verify execution.

---

## ⚙️ Environment Setup

**Hardware**
- CPU is sufficient (no GPU required)

**Software**
- Python 3.10+
- PyTorch  
- pandas  
- numpy  
- matplotlib  
- scikit-learn  

**Install dependencies**
```bash
pip install -r requirements.txt
```

## Repository Structure
- notebooks/ → Main execution notebook
- data/dummy/ → Synthetic dataset (structure-preserving)
- data/partial_guessing_curves/ → Precomputed evaluation results
- checkpoints/ → Pretrained model checkpoints
- scenario1_pgc_ccs_clean.png/pdf → Final evaluation figures

---

## Notes
- Dummy data is used only to verify pipeline execution
- Models are pretrained and not retrained in this artifact
- No external APIs or internet access required
- CPU execution is sufficient

---

## Results Partial Guessing Curves (PGC) are generated from precomputed result files. These reflect the actual experimental outcomes reported in the paper

---
## Runtime
- Total runtime: ~2–5 minutes on CPU
- No training required (models are pretrained)

## License
- This artifact is provided under the MIT License

