# Concrete Compressive Strength Analysis & Visualization

This project analyzes **concrete compressive strength (MPa)** using the `Concrete_Data_Yeh.csv` dataset and provides rich exploratory insights into how mix components and curing age influence strength. A Jupyter Notebook (`Concrete_Data_info.ipynb`) performs data exploration, generates an automated profiling report, and visualizes the top‑20 highest‑strength mixes.

---

## 📁 Project Structure

```
concrete_strength_prediction/
│
├── Concrete_Data_Yeh.csv        # Dataset (1 033 samples × 9 features)
├── Concrete_Data_info.ipynb     # Notebook with EDA & visualizations
├── Concrete_Data_info.txt       # Attribute descriptions
└── README.md                    # Project overview (this file)
```

---

## 📊 Dataset Overview

| Feature                                 | Unit (per m³) | Description                          | Role   |
| --------------------------------------- | ------------- | ------------------------------------ | ------ |
| Cement                                  | kg            | Portland cement                      | Input  |
| Blast Furnace Slag                      | kg            | Ground‑granulated blast‑furnace slag | Input  |
| Fly Ash                                 | kg            | Class F fly ash                      | Input  |
| Water                                   | kg            | Mixing water                         | Input  |
| Superplasticizer                        | kg            | High‑range water‑reducing admixture  | Input  |
| Coarse Aggregate                        | kg            | Gravel/stones                        | Input  |
| Fine Aggregate                          | kg            | Sand                                 | Input  |
| Age                                     | days (1‑365)  | Curing age before testing            | Input  |
| Concrete Compressive Strength (`csMPa`) | MPa           | Target strength                      | Output |

Full attribute details are provided in **`Concrete_Data_info.txt`**.

---

## 📒 Notebook Highlights (`Concrete_Data_info.ipynb`)

| Step                               | Description                                                                                                                                                                                                                                                                                                               |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Data Loading & Checks**       | Uses `pandas` to load CSV, inspect shape/dtypes, and validate null values.                                                                                                                                                                                                                                                |
| **2. Automated Profiling**         | Generates an interactive **YData Profiling** report for quick EDA.                                                                                                                                                                                                                                                        |
| **3. Top‑20 High‑Strength Subset** | Sorts by `csMPa` and selects 20 strongest mixes for focused analysis.                                                                                                                                                                                                                                                     |
| **4. Visualizations**              | <ul><li>**Stacked bar chart** – component quantities across top mixes.</li><li>**Individual pie charts** – composition breakdown per sample.</li><li>**Correlation heatmap** – relationships among numeric features.</li><li>**Scatter & line plots** – each input feature vs. strength, annotated for clarity.</li></ul> |
| **5. (Optional) Modeling**         | Placeholder for regression models (e.g., Linear, Random Forest, XGBoost) to predict `csMPa`.                                                                                                                                                                                                                              |

> **Why focus on the top 20?** Examining high‑performance mixes reveals ingredient combinations that yield exceptional strength, guiding mix‑design optimization.

---

## 🛠️ Technologies & Libraries

* **Python 3**
* **Jupyter Notebook**
* **pandas**, **numpy** – data wrangling
* **matplotlib**, **seaborn** – plotting
* **ydata‑profiling** – automated EDA report
* **scikit‑learn** *(future modeling section)*

---

## 🚀 Getting Started

1. **Clone the repo**

   ```bash
   git clone <your_repo_link>
   cd concrete_strength_prediction
   ```
2. **Install dependencies**

   ```bash
   pip install pandas numpy matplotlib seaborn ydata-profiling scikit-learn
   ```
3. **Launch the notebook**

   ```bash
   jupyter notebook Concrete_Data_info.ipynb
   ```
4. **Explore the profiling report** – It renders inline in the notebook for interactive exploration.

---

## 📈 Results & Insights

* **Ingredient impact:** Cement content shows the strongest positive correlation with strength, while water exhibits a negative trend in high‑strength mixes.
* **Visual takeaways:**

  * Stacked bars highlight mixes rich in cement and slag.
  * Pie charts quickly reveal proportion shifts between fine and coarse aggregates.
  * Correlation heatmap validates known water–cement ratio effects.
* **Actionable outcome:** The visual toolkit aids engineers in tweaking mix proportions to achieve target strengths cost‑effectively.

---

## 👤 Author

**Adithya Purama** — feel free to reach out with suggestions or collaboration ideas!
