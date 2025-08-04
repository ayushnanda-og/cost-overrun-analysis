# 🏗️ Cost Overrun Analysis in Construction Projects

This project presents a comprehensive data-driven analysis of cost overrun claims in the construction industry. The study evaluates the causes and risks associated with cost overruns and predicts the likelihood of disputes using statistical methods and a machine learning approach.

## 📊 Project Summary

A detailed analysis was conducted on data collected from **32 real-world construction projects**. The dataset included expert responses rated on a **1 to 5 Likert scale**, reflecting the **frequency and impact of various cost overrun causes**. 

To predict the potential for cost-related disputes, a **Random Forest Genetic Algorithm (RFGA)** machine learning model was trained using these insights.

---

## 📂 Repository Contents

| File/Folder         | Description |
|---------------------|-------------|
| `Prediction.ipynb`  | Jupyter notebook with full data analysis, feature engineering, model training, and evaluation. |
| `Cost_Overrun.csv`  | Dataset containing responses on overrun causes and their frequency. |
| `fig.png`           | Visualization showing key insights from the analysis. |
| `.ipynb_checkpoints`| Auto-saved notebook checkpoints (can be deleted). |

---

## 🔍 Key Methodologies

### 📌 Relative Importance Index (RII)
- Each overrun cause was evaluated for its frequency.
- **RII = ΣW / (A × N)** where:
  - W = weighting assigned to each factor by respondents
  - A = highest weight (5)
  - N = total number of respondents

> **Higher RII** values indicate causes that are more frequent and impactful in cost overrun claims.

### 🤖 RFGA Model for Prediction
- **Binary classification**:
  - 1 = Positive Overrun (Dispute likely)
  - 0 = No Overrun
- Model performance:
  - **Accuracy (Train):** 80%
  - **Accuracy (Test):** 100%

---

## 🧠 Major Findings

- **Top Causes of Cost Overruns:**
  - Price hike of materials
  - Delays due to environmental clearances
  - COVID-19 pandemic impacts
  - Inaccurate project cost estimation
  - Design alterations and analysis delays

- **Top Risk Factors for Conflicts (as per RFGA model):**
  - Inaccurate cost forecasting
  - Faulty equipment-related accidents
  - Poor financial control
  - Time-related uncertainties

---

## 🚀 Impact

- Improves **project cost estimation accuracy**
- Strengthens **dispute risk mitigation**
- Enhances the **economic and reputational standing** of the construction industry
- Supports **project managers** in better planning and resource allocation

---

## ✅ How to Use

## 🧪 Running the Notebook in GitHub Codespaces

You can view and run `Prediction.ipynb` directly inside GitHub Codespaces without any setup on your local machine.

---

### 🚀 Steps to Open Jupyter Notebook in Codespaces

1. **Open this repository in GitHub.**
2. Click the green **`Code`** button → Select the **`Codespaces`** tab.
3. Click **`+ Create codespace on main`** (or your preferred branch).
4. Once the Codespace loads, open a new **terminal** (`Ctrl + \`` or from the top menu).

---

### 🔧 Run Jupyter Notebook from Terminal (Bash Commands)

```bash
# Navigate to your workspace (usually already set)
cd /workspaces/<your-repo-name>  # replace with your repo name if needed

# Optional: Create and activate a virtual environment
python3 -m venv .venv
source .venv/bin/activate

# Upgrade pip and install required packages
pip install --upgrade pip
pip install pandas numpy matplotlib scikit-learn notebook

# Launch Jupyter Notebook server
jupyter notebook --ip=0.0.0.0 --port=8888 --no-browser --allow-root


