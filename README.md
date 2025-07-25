# Concrete Compressive Strength Prediction

This project focuses on predicting **concrete compressive strength (MPa)** based on its composition and curing age using the `Concrete_Data_Yeh.csv` dataset. The analysis and modeling are performed using Python and Jupyter Notebook.

---

## **Project Structure**

```
concrete_strength_prediction/
│
├── Concrete_Data_Yeh.csv
├── Concrete_Data_info.ipynb
├── Concrete_Data_info.txt
└── README.md
```

---

## **Dataset Overview**

**File:** `Concrete_Data_Yeh.csv`

### **Attributes** (from `Concrete_Data_info.txt`):

1. **Cement (component 1):** kg in a m³ mixture (Input Variable)
2. **Blast Furnace Slag (component 2):** kg in a m³ mixture (Input Variable)
3. **Fly Ash (component 3):** kg in a m³ mixture (Input Variable)
4. **Water (component 4):** kg in a m³ mixture (Input Variable)
5. **Superplasticizer (component 5):** kg in a m³ mixture (Input Variable)
6. **Coarse Aggregate (component 6):** kg in a m³ mixture (Input Variable)
7. **Fine Aggregate (component 7):** kg in a m³ mixture (Input Variable)
8. **Age:** Days (1–365) (Input Variable)
9. **Concrete Compressive Strength:** MPa (Output Variable)

---

## **Notebook Overview**

**File:** `Concrete_Data_info.ipynb`

The notebook covers:

* **Data Exploration:** Understanding the structure and summary of the dataset.
* **Feature Analysis:** Investigating the effect of each ingredient on strength.
* **Data Visualization:** Plotting correlations and distributions.
* **Modeling (Optional):** Regression modeling to predict compressive strength.

---

## **Technologies Used**

* **Python 3**
* **Jupyter Notebook**
* **Libraries:**

  * `pandas`
  * `numpy`
  * `matplotlib`
  * `seaborn`
  * `scikit-learn` (if modeling is included)

---

## **How to Run**

1. Clone the repository:

   ```bash
   git clone <your_repo_link>
   cd concrete_strength_prediction
   ```
2. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Open the notebook:

   ```bash
   jupyter notebook Concrete_Data_info.ipynb
   ```

---

## **Results**

The dataset helps in:

* Understanding the role of each component in concrete strength.
* Building predictive models for compressive strength.
* Optimizing concrete mix design for construction.

---

## **Author**

**Adithya Purama**
