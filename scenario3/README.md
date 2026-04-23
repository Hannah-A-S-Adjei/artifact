# Scenario 3 Artifact: Multi-Account Attacks (Trawling and Targeted) 

This repository contains the artifact for **Scenario 3 (Multi-Account Attacks: Trawling and Targeted)** from our CCS submission. It enables reproducibility of the evaluation pipeline using a reviewer-safe data.

---

## 📌 Description

This artifact provides:

- Evaluation of multi-account attack strategies:
  - Trawling (untargeted)
  - Targeted attacks
- Comparison across classical models:
  - List-based
  - Markov backoff
  - TarGuess-style
- Generation of evaluation figures:
  - Flatness curves
  - Success plots
  - Partial Guessing Curves



**Privacy Note:**  
Scenario 3 depends on external data derived from user studies and password constructions, making raw data sharing impractical. Therefore, we provide safe outputs that preserve full reproducibility of the reported analysis and figures.

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
 

**Install dependencies**
```bash
pip install -r requirements.txt
```

## Repository Structure
- notebooks/ → Main execution notebook
- csv/ → Reviewer-safe input data files


---

## Notes
- No raw user data or passwords are included
- The artifact focuses on evaluation and visualization only
- CPU execution is sufficient

---
## Results  
Flatness curves, success plots, and Partial Guessing Curves (PGC) are generated from precomputed safe result files.
These reflect the evaluation pipeline and experimental setup used in the paper.

---
## Runtime
- Total runtime: ~1–3 minutes on CPU

## License
- This artifact is provided under the MIT License

