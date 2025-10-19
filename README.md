# Modern Portfolio Theory: Efficient Frontier Analysis of Indonesian Banking Stocks

## 📘 Overview
This project applies **Modern Portfolio Theory (MPT)**, a fundamental concept in **Portfolio Management**, to analyze optimal risk-return trade-offs among Indonesian banking stocks. Using Python, we construct and visualize the **Efficient Frontier**, identifying the portfolios with:

- Maximum Sharpe Ratio (optimal risk-adjusted return)
- Minimum Volatility (least total risk)

This analysis demonstrates how data science can be applied to real-world investment management, combining **quantitative finance** with **Python programming**.

---

## 📈 Key Objectives
1. Download and process historical stock price data from Yahoo Finance.
2. Calculate daily returns, expected annual returns, and covariance.
3. Generate 20,000 random portfolios with varying asset weights.
4. Compute expected portfolio return, volatility, and Sharpe ratio.
5. Visualize the **Efficient Frontier** and highlight the **Optimal Portfolios**.
6. Interpret results using concepts: risk, return, diversification, and efficiency.

---

## 💼 Assets Analyzed
The portfolio consists of major **Indonesian banking stocks** listed on IDX:

| Ticker | Company | Description |
|---------|----------|-------------|
| **BBCA.JK** | Bank Central Asia | Large-cap, low-risk defensive bank |
| **BBRI.JK** | Bank Rakyat Indonesia | State-owned, broad retail exposure |
| **BMRI.JK** | Bank Mandiri | Balanced corporate and retail focus |
| **BNGA.JK** | Bank CIMB Niaga | Mid-cap with higher growth potential |
| **BNII.JK** | Bank Maybank Indonesia | Smaller bank, diversification element |

---

## ⚙️ Tools & Libraries
- **Python 3.10+**
- **yfinance** – Downloading historical market data  
- **numpy, pandas** – Financial computations  
- **matplotlib** – Visualization  
- **seaborn** – Correlation heatmaps (optional)

---

## 🧮 Methodology Summary
1. **Data Collection:** Historical prices (2020–2024) pulled from Yahoo Finance.  
2. **Computation:** Daily returns, mean returns, and covariance matrix calculated.  
3. **Simulation:** 20,000 random portfolios generated.  
4. **Optimization:** Identify portfolios with maximum Sharpe ratio and minimum volatility.  
5. **Visualization:** Efficient Frontier plotted with color-coded Sharpe Ratios.  
6. **Interpretation:** Analyze asset weights and diversification implications.

---

## 📊 Key Results

| Portfolio | Expected Return | Volatility | Sharpe Ratio | Main Holdings |
|------------|----------------|-------------|---------------|----------------|
| **Max Sharpe** | ~21.0% | ~25.2% | **0.63** | BNGA, BMRI, BBCA |
| **Min Volatility** | ~16.2% | ~22.1% | **0.51** | BBCA, BNGA, BNII |

- The **Maximum Sharpe Portfolio** delivers the best risk-adjusted return, favoring BNGA and BMRI.  
- The **Minimum Volatility Portfolio** is dominated by BBCA, reflecting its defensive nature.  
- Even within a single sector (banking), diversification reduces total portfolio risk.

---

## 📉 Efficient Frontier Visualization
The Efficient Frontier represents all possible portfolios that offer the **highest expected return for a given level of risk**.

- **Red Dot:** Maximum Sharpe Ratio portfolio (tangency portfolio)
- **Blue Dot:** Minimum Volatility portfolio (global minimum variance)
- **Color Gradient:** Sharpe Ratio intensity

---

## 🧩 Interpretation
> “Diversification allows investors to achieve a more efficient combination of risk and return. The efficient frontier visually represents the benefit of diversification — portfolios below it are inefficient, while portfolios on the curve are optimal.”

This notebook demonstrates how to operationalize that concept using Python.

---

## 🚀 How to Run the Notebook

### 1. Clone this repository
```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/modern_portfolio_theory.git
cd modern_portfolio_theory
```

### 2. Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate    # Mac/Linux
venv\Scripts\activate     # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook
```

Then open `modern_portfolio_theory.ipynb`.

---

## 📦 Suggested `requirements.txt`
```
numpy
pandas
matplotlib
yfinance
seaborn
```
*(optional but recommended: `scipy`, `plotly`, `streamlit`)*

---

## 🧭 Future Enhancements
- Add **Capital Market Line (CML)** visualization  
- Calculate **CAPM alpha/beta** for each stock  
- Include **correlation heatmap**  
- Build a **Streamlit dashboard** for interactivity  
- Extend analysis to multi-sector portfolios

---

## 🧑‍💼 Author
**Cakraningrat Kencana Murti**  
Project Specialist | Banking & Finance | Data Science Enthusiast  

🔗 [GitHub](https://github.com/cakrakencana)  
📧 cakra.kencana.km@gmail.com
---

## 📚 References
- CFA Institute (2025). *CFA Program Curriculum, Level I – Portfolio Management.*  
- Markowitz, H. (1952). *Portfolio Selection.* Journal of Finance.    
