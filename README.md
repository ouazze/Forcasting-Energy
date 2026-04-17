#  Energy Demand Forecasting Project

##  Overview

This project focuses on **energy demand analysis and forecasting** using real-world and augmented datasets.
It combines **data exploration, statistical analysis, and deep learning models (LSTM + TFT)** to generate long-term forecasts.

---

##  Project Structure

```
.
├── DataAgumentation.ipynb     # Data augmentation & representative days extraction
├── Owid-enrg.ipynb            # Global energy analysis (OWID dataset)
├── Prevesion.ipynb            # Forecasting model (LSTM + TFT)
├── owid-energy-data.csv       # OWID dataset
├── owid-energy-codebook.csv   # Dataset description
└── README.md
```

---

##  Project Workflow

### 1. Data Augmentation (`DataAgumentation.ipynb`)

* Exploratory Data Analysis (EDA)
* Statistical analysis of energy demand
* Generation of **5 years of synthetic data**
* Extraction of **representative days per season**

---

### 2. Global Energy Analysis (`Owid-enrg.ipynb`)

* Dataset: **Our World in Data (OWID)**
* Steps:

  * Data understanding & cleaning
  * Feature engineering
  * Exploratory Data Analysis
  * Statistical tests
  * Clustering
* Target variable:

  * `primary_energy_consumption` (TWh)

---

### 3. Forecasting Model (`Prevesion.ipynb`)

* Model: **Hybrid LSTM + Temporal Fusion Transformer (TFT)**
* Pipeline:

  * Load augmented data
  * Feature engineering
  * Model training & evaluation
* Target:

  * `Total_Energy_MWh` (hourly)
* Output:

  * **15-year energy demand forecast**

---

##  Model Architecture

* LSTM Encoder (time dependencies)
* Multi-Head Attention (TFT-style)
* Gated Residual Network
* Dense Output Layer

---

##  Key Features

* Time series forecasting
* Data augmentation techniques
* Hybrid deep learning model
* Multi-scale energy analysis (local + global)

---

##  Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow pytorch
```

---

##  How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/energy-forecast.git
cd energy-forecast
```

2. Open notebooks:

```bash
jupyter notebook
```

3. Run in order:

* `DataAgumentation.ipynb`
* `Owid-enrg.ipynb`
* `Prevesion.ipynb`

---

##  Results

* Long-term energy demand forecasting (15 years)
* Synthetic dataset generation for training robustness
* Insights from global energy trends

---

##  Author

Ouazze Moahmed

---

## Notes

* Ensure datasets are in the correct path before running notebooks
* GPU recommended for model training
