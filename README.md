# Quant_IRR — Long-Term Market Strategy (Quant / ML / Hybrid)

This repository contains a Python-based quant research project built to design a **long-term investment strategy** using historical market data and to **generate Buy/Sell signals** based on that strategy. The project was developed in the context of an **inter-hostel competition**, with the **problem statement provided by Beyond IRR**.

We evaluate and compare three approaches:
1. **Quantitative (rule/indicator-based)**
2. **Machine Learning (ML)**
3. **Integrated (Quant + ML hybrid)**

---

## Repository Layout

- `quantitative_approach.py` — Quant-only strategy + signal generation + evaluation
- `ML.py` — ML-based prediction + signal generation + evaluation
- `integrated_approach.py` — Hybrid approach combining Quant + ML + evaluation
- `plot_performance.py` — Plots/visualizations for performance and comparisons
- `performance_stats/` — Stored evaluation metrics and results (per approach)
- `indexes.csv` — Input dataset used for analysis/backtesting
- `PERFORMANCE_AND_ML_REPORT.md` — Project report and summarized results
- `ML_README.md` — ML-specific notes
- `Kriti2026_quant.pdf` — Problem statement document (Beyond IRR)

---

## Setup (Virtual Environment)

### 1) Clone the repository
```bash
git clone https://github.com/Dhruv-Punekar/Quant_IRR.git
cd Quant_IRR
```

### 2) Create and activate a virtual environment

**Windows (PowerShell)**
```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

---

## Execution Commands

> Run scripts from the repository root after activating the virtual environment.

### A) Quantitative approach
Runs the pure quant strategy and saves performance outputs to `performance_stats/`.
```bash
python quantitative_approach.py
```

### B) Machine Learning approach
Runs the ML pipeline (feature engineering + training/inference) and saves results to `performance_stats/`.
```bash
python ML.py
```

### C) Integrated (Quant + ML) approach
Runs the hybrid pipeline and saves results to `performance_stats/`.
```bash
python integrated_approach.py
```

### D) Plot performance / visualize results
Creates plots using the computed results/metrics (commonly read from `performance_stats/`).
```bash
python plot_performance.py
```

---

## Outputs & Where to Find Them

- **Signals / predictions / backtest metrics**: saved inside `performance_stats/`
- **Project write-ups**:
  - `PERFORMANCE_AND_ML_REPORT.md`
  - `ML_README.md`
- **Problem statement**: `Kriti2026_quant.pdf` (Beyond IRR)

---

## Notes / Assumptions

- The dataset `indexes.csv` is assumed to be the main input for all approaches.
- File names reflect which approach is being executed.
- Results are persisted so that `plot_performance.py` can generate charts without re-running everything (depending on implementation).

---

## Disclaimer

This project is intended for educational/research purposes (inter-hostel competition) and does not constitute financial advice. Markets involve risk; past performance does not guarantee future results.
