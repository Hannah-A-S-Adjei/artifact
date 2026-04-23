# Scenario 2 Artifact: Chooser Attacker (List-wise Ranking) 

This repository contains the artifact for **Scenario 2 (Chooser Attacker (List-wise Ranking)** from our CCS submission. It enables reproducibility of the evaluation pipeline using a reviewer-safe data.

---

## 📌 Description

This artifact provides:

- Offline evaluation of multiple models:
  - GPT-5.4
  - LLaMA-3.3-70B
  - Claude Sonnet 4.6
  - Gemini 2.5 Pro
  - DeepSeek-Chat
  - TarGuess-style baseline
- Per-user ranking outputs
- Partial Guessing Curve (PGC) generation


**Privacy Note:**  
Scenario 2 depends on external model interactions and user-derived data, making raw data sharing impractical. Therefore, we provide safe outputs that preserve full reproducibility of the reported analysis and figure.

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
- Per_user_csv/ → Reviewer-safe per-user ranking files


---

## Notes
- No model queries or API calls are performed in this artifact
- All results are loaded from precomputed safe files
- No external APIs or internet access required
- CPU execution is sufficient

---
## Results  
Partial Guessing Curves (PGC) and comparisons between TT-style and our list construction across attackers are generated from precomputed result files. These reflect the experimental setup and pipeline used in the paper.

---
## Runtime
- Total runtime: ~1–3 minutes on CPU

## License
- This artifact is provided under the MIT License

