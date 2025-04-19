# Smartphone Retail Sales Analysis

> **Explore • Visualise • Optimise**  
> Understanding smartphone revenue by product tier, quarter & city

---

## 🔍 Project scope
The notebook `smartphone.ipynb` walks through an end‑to‑end exploratory analysis of a public retail dataset from Kaggle. Key questions:

1. **Which product tiers drive the most revenue?**  
2. **How does seasonality affect sales?** (quarterly trends)  
3. **Which cities outperform—or underperform?**  

Import, cleaning, EDA and visualisations are fully contained inside the notebook.

---

## 🗂️ Repository layout
```
│  smartphone.ipynb     # main Jupyter notebook with code & commentary
│  README_smartphone.md # you are reading it 📖
├─ data/                # drop the CSV here (git‑ignored)
├─ images/              # auto‑generated plots (bar, heat‑maps)
└─ models/              # future place for saved models
```

---

## 📦 Dataset
*Source*: [Smartphone Retail Outlet Sales Data](https://www.kaggle.com/datasets/shubham2703/smartphone-retail-outlet-sales-data).

| Column      | Description                                 |
|-------------|---------------------------------------------|
| `Date`      | Transaction date (dd‑mm‑YYYY)               |
| `CITY`      | Outlet location                             |
| `CATEGORY`  | Product tier (Flagship, Mid‑range, etc.)    |
| `REVENUE`   | Sales amount / turnover                     |

> By default the notebook expects the CSV at `./data/SMARTPHONE RETAIL OUTLET SALE DATA.csv`.  
> Running in Google Colab? Just upload the file or mount Drive.

---

## 🚀 Quick start
```bash
# 1 — clone repository
git clone https://github.com/AlidarxD/smartphone_sales_analysis.git
cd smartphone_sales_analysis

# 2 — (optional) create a virtual env
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 3 — install dependencies
pip install -r requirements.txt

# 4 — launch Jupyter
jupyter lab     # or jupyter notebook
```
Open `smartphone.ipynb` and run cells top → bottom.

---

## 🛠️ Dependencies
```text
pandas>=2.0
numpy>=1.24
matplotlib>=3.8
seaborn>=0.13
jupyterlab>=4.0
```

---

## 📊 Key insights
* **Average revenue by quarter** — bar chart shows **Q4 is dominant**, largely driven by flagship models.
* **Heat‑map (City × Category)** — New York stores lead flagship sales, while mid‑range devices are evenly distributed.

Plots are stored in `images/`, or regenerate by running the notebook.

---

## 🚧 Roadmap
* Forecast demand with Prophet / ARIMA.  
* Customer segmentation (RFM) linked to product tiers.  
* Deploy an interactive dashboard via Streamlit.

Pull requests are welcome — fork, create a branch and open an issue/PR.

