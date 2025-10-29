## 📘 **Mutual Fund Plan with Python**

**Analyze Nifty 50 closing prices to create a mutual fund plan based on high ROI and low risk.**

---

### 🧩 **Overview**

This project uses **Python** and **financial analytics** to develop a **data-driven mutual fund strategy**.
By analyzing NIFTY 50 companies' closing prices, it identifies stocks with **high ROI (returns)** and **low volatility (risk)** — ideal for long-term, stable growth.

---

### 🎯 **Objective**

To create a **Mutual Fund Investment Plan** that balances:

* **High ROI (Return on Investment)**
* **Low Volatility (Risk)**

This approach helps investors achieve consistent long-term growth with controlled risk exposure.

---

### 🧹 **Data Preparation**

* Loaded **Nifty 50 closing price data** from CSV.
* Converted the **Date** column to `datetime` format.
* Verified for **missing values** (no nulls found).
* Performed **Exploratory Data Analysis (EDA)** to understand trends.

---

### 📊 **Data Analysis**

1. **Volatility Calculation**

   * Used **Standard Deviation** of stock prices to measure risk.

2. **Growth Rate Calculation**

   * Used **Percentage Change (pct_change)** to compute daily growth rates.

3. **ROI Calculation**

   * ROI = ((Final - Initial) / Initial × 100)

4. **Company Selection Strategy**

   * Selected companies where:

     * ROI > median ROI (high returns)
     * Volatility < median volatility (low risk)

5. **Investment Ratio Allocation**

   * Used **Inverse Volatility Weighting**:

     * Lower volatility → higher investment ratio
     * Ensures stability in returns

---

### 📈 **Visualization**

* **Stock Price Trends** – Line plots for all companies using Plotly.
* **Top 10 Risky Stocks** – Based on volatility ranking.
* **Top 10 Growth Stocks** – Based on average percentage change.
* **ROI Analysis** – Identified companies with the highest return on investment.
* **Investment Ratios** – Displayed recommended allocation percentages.
* **Future Value Simulation** – Projected returns for 1, 3, 5, and 10 years.

---

### 💰 **Mutual Fund Projection**

Assuming:

* ₹5000 monthly SIP
* 10% annual increase in investment
* Compounded monthly
* Based on average mutual fund ROI

|  Period  | Future Value (Approx.) |
| :------: | :--------------------: |
|  1 Year  |         ₹64,000        |
|  3 Years |        ₹4,70,000       |
|  5 Years |       ₹13,00,000+      |
| 10 Years |       ₹72,90,000+      |

💡 *Demonstrates the power of consistent investing and compounding over time.*

---

### 🧠 **Insights**

* High ROI often comes with higher volatility, but filtering by both metrics helps balance risk and reward.
* Companies with **moderate ROI and low volatility** are most suitable for **long-term mutual fund investments**.
* The **inverse volatility strategy** ensures stability while maximizing returns.

---

### ⚙️ **Technologies Used**

* **Python**
* **Pandas**, **NumPy**
* **Plotly** (for interactive visualizations)
* **Matplotlib / Seaborn** (optional for static charts)
* ****Google Colab**

---

### 📂 **Project Structure**

```
📁 Mutual_Fund_Plan_Python/
│
├── nifty50_closing_prices.csv
├── Mutual_Fund_Plan.ipynb
├── README.md


