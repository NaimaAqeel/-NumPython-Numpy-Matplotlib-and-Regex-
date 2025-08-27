

#  COVID-19 Fictional Data Analysis + RegEx Tasks

##  Project Overview

This project is an **Exploratory Data Analysis (EDA) and Python Practice Notebook** built around fictional COVID-19 data from **3 planets**:

*  **Tatooine**
*  **Naboo**
*  **Alderaan**

The dataset tracks:

* **Daily Cases**
* **Recoveries**
* **Deaths**

for **4 cities on each planet**.

The objective is to practice:

* **NumPy slicing & aggregations**
* **Matplotlib plotting (bar, subplot, scatter plot, bubble chart)**
* **Regular Expressions (RegEx)** for text pattern extraction and validation

---

##  Dataset

The dataset is represented as **Python lists**, later combined into a **3D NumPy array**:

* **Shape of array:** `(3, 4, 3)`

  * `3` → Planets
  * `4` → Cities per planet
  * `3` → Features (Cases, Recoveries, Deaths)

Example:

```
all_data[planet, city, feature]
```

* Feature Index:

  * `0` → Cases
  * `1` → Recoveries
  * `2` → Deaths

---

##  Key Tasks Performed

###  NumPy Operations

* Combine individual planet data into a **3D array**
* Extract **deaths column** for each planet
* Compute:

  * **Total deaths per planet**
  * **Planet with maximum deaths** using `np.argmax`
  * **Average deaths per city** using `np.mean`

---

###  Data Visualization

* **Bar Chart** → COVID-19 cases in Tatooine cities
* **Subplots (3 side-by-side bar charts)** → Cases across Tatooine, Naboo, and Alderaan
* **Scatter Plot (Bubble Chart)**

  * X-axis → GDP per capita
  * Y-axis → Life Expectancy
  * Bubble size → Population
  * Each bubble labeled with **country name**

---

###  Regular Expressions (RegEx) Practice

1. **RGB Hex Code Detection**

   * Match valid hex color codes (`#FF5733`, `#0A0A0A`)
   * Reject invalid codes (`#12345`, `#XYZ123`)

2. **Time Extraction (HH\:MM)**

   * Extract times only if followed by **AM/PM**
   * Use **capturing & non-capturing groups**

3. **String Validator**

   * Function checks if a string contains only **alphabets, digits, and spaces**

4. **Website Detection**

   * Extract valid websites from HTML snippet
   * Capture **whole URL** and **part after `://`** separately

---

##  Example Outputs

* **Highest Death Planet:** Tatooine
* **Average deaths per city:** `[4.5, 3.5, 2.5]`
* **Bar/Subplots:** Show COVID-19 cases per city
* **Bubble Chart:** GDP vs Life Expectancy with population size
* **RegEx Matches:**

  * Hex Codes → `['#FF5733', '#33FF57', '#3357FF', '#0A0A0A', '#FAFAFA']`
  * Times → `['09:45', '05:30', '11:15']`
  * Websites → Extracted full + domain parts

---

##  Technologies Used

* **Python 3**
* **NumPy** → Array manipulation & aggregation
* **Matplotlib** → Visualization (bar, subplot, scatter)
* **RegEx (`re` module)** → Pattern matching

---

##  How to Run

1. Clone this repo:

   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   ```
2. Open the notebook/script in Python or Jupyter
3. Run the cells to see analysis & plots

---

##  Learning Objectives

* Understand **3D NumPy arrays** and indexing
* Perform **aggregations (sum, mean, max, argmax)**
* Create **consistent subplots** for comparative visualization
* Work with **scatter plots and bubble charts**
* Gain hands-on practice with **Regular Expressions** in Python

---

##  Author

**Naima Aqeel**
📧 Email: `naimapnes@gmail.com`
🌐 GitHub: [NaimaAqeel](https://github.com/NaimaAqeel)

---

