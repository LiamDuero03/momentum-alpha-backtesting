# Equity Momentum Backtesting: From Naive Rules to Sharpe-Optimized Strategies

This project explores **equity momentum strategies** on U.S. stocks, starting with a **naive daily momentum baseline** and iteratively refining it to improve **risk-adjusted returns**.

---

## 📊 What This Project Covers

1. **Naive Daily Momentum**
   - 20/60/120-day lookback windows on a small 5-stock universe
   - Poor baseline performance:
     - **CAGR:** –4.18%
     - **Sharpe Ratio:** –0.09
     - **Max Drawdown:** –73.52%

2. **Weekly Filtering**
   - Weekly rebalancing & simple signal filters to reduce noise
   - Improved results:
     - **CAGR:** +4.82%
     - **Sharpe Ratio:** 0.77
     - **Max Drawdown:** –40.77%

3. **Sharpe-Optimized Momentum**
   - Added **regime filters** (avoiding bear markets)
   - Applied **volatility scaling** (equalizing risk)
   - Best measured performance:
     - **CAGR:** +1.97%
     - **Sharpe Ratio:** **1.42**
     - **Max Drawdown:** –6.03%

4. **Scaling the Universe**
   - Expanded to 25 and 200 large-cap U.S. stocks
   - Introduced **cross-sectional ranking** (weekly top N)
   - Tested **market-neutral long/short momentum**
   - Found that **momentum alpha weakened in U.S. large-caps post-2010**

---

## 🧠 Key Takeaways

- Naive momentum **overtrades and suffers huge drawdowns**.
- Weekly filtering & regime awareness **improves Sharpe ratio and reduces risk**.
- Even well-managed momentum can have **modest raw CAGR but excellent risk-adjusted returns**.
- In **U.S. large-cap equities post-2010**, pure momentum has struggled—highlighting the need for:
  - Longer lookback horizons (6–12 months)
  - Broader universes (global equities, mid-caps, multi-asset)
  - Multi-factor combinations (momentum + value/quality)

> **Lesson learned:** Iterative refinements and robust risk management are essential to turning a naive strategy into something usable—while also understanding when a factor’s edge is regime-dependent.

---

## 🛠 Tech Stack

- **Python**
- **Pandas / NumPy** (data processing)
- **yfinance** (data collection)
- **Matplotlib** (visualizations)

---
