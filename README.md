# Machine Learning for Scientific Research 🔬🤖

Welcome to the official repository for the **Machine Learning for Scientific Research** course. 🧠
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
- **Context**: Machine Learning definition and key milestones.
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
- **Ensemble methods**: classical ensemble methods for classification and regression.
- **Advanced ensemble methods**: stacking.

### [Day 5: advanced architectures](link_to_day5)
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

You will need to use the **command line** for several tasks—not only during software installation, but also in the hands-on activities.
We will be using **Python** for our exercises.
Start by opening a terminal window and typing the following command:

```bash
python -V
```
or
```bash
python --version
```

You should see output similar to:

```bash
Python 3.XX.YY
```

where `XX` and `YY` depend on your installed Python version.
Any recent **Python 3** version should be compatible with the packages we will use.

---

### 1. [VSCodium](https://vscodium.com)

We will use [**VSCodium**](https://vscodium.com) for our programming tasks.
VSCodium is a source code editor designed for programming and software development.
While it is **not technically an Integrated Development Environment (IDE)**, it can behave line one with the right extensions, providing project management, debugging, and testing features.
It is an open-source version of Visual Studio Code (VS Code) that **respects your privacy**—it does not send usage data to Microsoft.

However, if you prefer, you can use [Visual Studio Code](https://code.visualstudio.com).

#### Recommended extensions

After installing VSCodium, open the "Extensions" panel and install the following:
- `Python` (ms-python)
- `Jupyter` (ms-toolsai)
- `Jupyter Notebook Renderers` (ms-toolsai)
- `CSV` (ReprEng)
- `git-autoconfig` (shyykoserhiy)

Other helpful extensions:
- `Todo Tree` (for tags and task tracking)
- `Vim` (for Vim enthusiasts).

### 2. Install [`uv`](https://docs.astral.sh/uv/)

This project uses [`uv`](https://docs.astral.sh/uv/) for Python package and project management.
This ensures that everyone uses the exact same versions of libraries, locked in the `uv.lock` file.

If you haven't installed `uv` yet, run the following:
- **macOS/Linux**:
  ```bash
  curl -LsSf [https://astral.sh/uv/install.sh](https://astral.sh/uv/install.sh) | sh
  ```
- **Windows**:
  ```powershell
  powershell -c "irm [https://astral.sh/uv/install.ps1](https://astral.sh/uv/install.ps1) | iex"
  ```

### 3. Environment setup

Clone the repository and synchronise the environment.
`uv` will automatically create a virtual environment and install all dependencies:
```bash
git clone git@github.com:NunonuN/ml4research.git
cd ml4research
uv sync
```

### 4. Running notebooks

To run the Jupyter notebooks provided in the `notebooks/` directory, open them inside VSCodium or, within the locked environment, run:
```bash
uv run jupyter-lab
```

🚀 **First step**: before the start of the course, please complete the instructions in this section to ensure your local machine is ready.

---

## 📂 Repository Structure

- `notebooks/`: Jupyter notebooks containing lecture code and hands-on exercises.
- `slides/`: PDF interactive presentations for each day.
- `data/`: sample data sets (Diabetes, Iris, California Housing) used in tutorials.
- `pyproject.toml`: project metadata and dependency definitions.
- `uv.lock`: the deterministic lock-file ensuring reproducible set-ups.

🤝 Collaboration
If you find a typo or a better way to implement a robust metric, please feel free to open a Pull Request!

Created by Nuno R. C. Gomes (IEEC/ICE-CSIC) on 2026/05/12 — Promoting Open Science through robust Machine Learning.
