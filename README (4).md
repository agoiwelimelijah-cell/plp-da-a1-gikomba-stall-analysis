# Gikomba Market Stall Performance Analysis

**Author:** Elijah Agoiwelim  
**Cohort:** PLP Data Analysis Cohort 1  
**Repository:** `plp-da-a1-gikomba-stall-analysis`

---

## 1. Summary of Wanjiku's Business Problem

Wanjiku operates a fresh-produce stall at Nairobi's bustling Gikomba Market, selling staple commodities including tomatoes, onions, sukuma wiki, potatoes, and avocados. Over the past two weeks (14 days), she maintained handwritten notes of daily revenue in a ledger alongside rough estimates of warehouse stock, but lacked the analytical tools to determine whether her business is genuinely growing, when to trigger wholesale vegetable restocks, or how customer buying behaviors shift across trading days. Without systematic data analysis, Wanjiku faced the dual hazard of holding excessive capital in slow-moving items like potatoes while running dangerously low on high-margin, fast-depleting perishables like sukuma wiki and tomatoes ahead of lucrative weekend shopping crowds.

---

## 2. How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/elijahel/plp-da-a1-gikomba-stall-analysis/blob/main/stall_analysis.ipynb)

To run this analysis:
1. Click the **Open In Colab** badge above to launch `stall_analysis.ipynb` directly in your browser.
2. Alternatively, clone this repository and run locally:
   ```bash
   git clone https://github.com/elijahel/plp-da-a1-gikomba-stall-analysis.git
   cd plp-da-a1-gikomba-stall-analysis
   jupyter notebook stall_analysis.ipynb
   ```
3. Run all cells sequentially from top to bottom (**Kernel → Restart & Run All**). The entire codebase uses **Core Python standard library only** (no external libraries like `pandas` or `numpy` are imported or required).

---

## 3. Top Three Findings

1. **Demonstrated Revenue Growth (+10.66% Week-on-Week):** Total 14-day sales amounted to **KES 46,450** with a daily average of **KES 3,317.86**. Revenue expanded from **KES 22,050** in Week 1 to **KES 24,400** in Week 2, registering a positive week-on-week growth rate of **+10.66%**.
2. **Weekend Sales Outperform Weekdays by +82.50%:** Weekend daily sales (Saturdays and Sundays) averaged **KES 4,900.00**, which is **82.50% higher** than the weekday average of **KES 2,685.00** (Mon–Fri). The best trading day across both weeks was Saturday of Week 2 (**KES 5,600**), whereas Tuesday of Week 1 was the lowest (**KES 1,950**).
3. **Imminent Stockouts on Key High-Margin Produce (Sukuma & Tomatoes):** Two out of the five inventory items have dropped to or below their mandatory reorder thresholds: **Sukuma (9 kg remaining vs. 15 kg reorder)** and **Tomatoes (18 kg remaining vs. 25 kg reorder)**. With Sukuma commanding a high **40.00% gross margin** and Avocado yielding **42.86%**, failing to replenish Sukuma before the weekend directly sacrifices high-margin earnings.
