# Machine Learning for Scientific Research 🔬🤖

Welcome to the official repository for the **Machine Learning for Scientific Research** course.
This programme is designed to bridge the gap between "black-box" machine learning (ML) and the demands of the scientific method.

## 🪐 Level
This is an **introductory-level course**, specifically designed for researchers and scientists who are new to the field of Machine Learning.
While we focus on high-level scientific rigour and robustness, no prior expertise in artificial intelligence (AI) or advanced computer science is required to get started.

## 🌟 Course philosophy
In science, a prediction without an explanation or an uncertainty estimate is just a guess.
This course focuses on **robust ML**: moving beyond simple accuracy to prioritise generalisability, interpretability, and reproducibility.

---

## 📅 Programme overview

### [Day 1: Foundations of scientific ML](link_to_day1)
- **Scientific problems**: predictive modelling _vs._ parameter estimation.
- **The workflow**: adapting the ML life cycle to the scientific method.
- **Generalisation**: understanding the tension between **overfitting** and **underfitting**.
- **The bias-variance trade-off**: navigating model complexity _vs._ stability.

### [Day 2: Data wrangling & robustness](link_to_day2)
- **Data taxonomy**: tabular _vs._ non-tabular data (images, graphs, text).
- **EDA**: exploratory data analysis as a tool for hypothesis generation.
- **The cleaning lab**: handling missing data and outliers using **IQR** and **Tukey’s Fences**.
- **Robust metrics**: moving beyond standard deviation to **MAD** and **MedAD**.
- **PCA:** dimensionality reduction and preserving scientific signal.

### [Day 3: model selection & evaluation](link_to_day3)
- **The golden rule**: implementing strict training-testing splits to avoid data leakage.
- **Cross-validation** using **K-Fold** strategies for small, noisy research data sets.
- **Regularisation**: Lasso (L1) for automated feature selection and Ridge (L2) for multicollinearity.
- **Evaluation metrics**: choosing metrics that match scientific goals (e.g., $\text{R}^2$, MSE, F1-score).

### [Day 4: advanced architectures](link_to_day4)
- **Neural networks**: transitioning from classical ML to Deep Learning.
- **Unstructured data**: processing signals and images in a research context.

### [Day 5: robustness, ethics & beyond](link_to_day5)
- **Uncertainty quantification**: confidence intervals and Bayesian approaches.
- **Explainability (XAI)**: opening the black box with **SHAP** values and feature importance.
- **Reproducibility**: version control with Git, environment management, and documentation.
- **Ethics & bias**: identifying algorithmic bias in scientific cohorts.
- **Hands-on capstone** applying the full stack to your own research data.

---

## 🛠️ Getting Started

This project uses [`uv`](https://docs.astral.sh/uv/) for Python package and project management.
This ensures that everyone uses the exact same versions of libraries, locked in the `uv.lock` file.

### 1. Install `uv`
If you haven't installed `uv` yet, run the following:
- **macOS/Linux**:
  ```bash
  curl -LsSf [https://astral.sh/uv/install.sh](https://astral.sh/uv/install.sh) | sh
  ```
- **Windows**:
  ```powershell
  powershell -c "irm [https://astral.sh/uv/install.ps1](https://astral.sh/uv/install.ps1) | iex"
  ```

### 2. Environment setup
Clone the repository and synchronise the environment.
`uv` will automatically create a virtual environment and install all dependencies:
```bash
git clone git@github.com:NunonuN/ml4research.git
cd ml4research
uv sync
```

### 3. Running notebooks
To run the Jupyter notebooks, open them inside VSCodium or, within the locked environment, run:
```bash
uv run jupyter-lab
```

🚀 **First Step**: before Day 1, please complete the instructions in [0+environment-setup.ipynb](./notebooks/0+environment-setup.ipynb) to ensure your local machine is ready.

---

## 📂 Repository Structure

- `/notebooks`: Jupyter notebooks containing lecture code and hands-on exercises.
- `/slides`: PDF interactive presentations for each day.
- `/data`: sample data sets (Diabetes, Iris, California Housing) used in tutorials.
- `pyproject.toml`: project metadata and dependency definitions.
- `uv.lock`: the deterministic lock-file ensuring reproducible set-ups.

🤝 Collaboration
If you find a typo or a better way to implement a robust metric, please feel free to open a Pull Request!

Created by Nuno R. C. Gomes (IEEC/ICE-CSIC) on 2026/05/12 — Promoting Open Science through robust Machine Learning.
