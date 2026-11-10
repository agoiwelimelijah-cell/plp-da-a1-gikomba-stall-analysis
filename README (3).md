# Gikomba Market Stall Performance Analysis

**Author:** Elijah Agoiwelim  
**Cohort:** PLP Data Analysis Cohort 1  
**Repository:** `plp-da-a1-gikomba-stall-analysis`

---

## 1. Summary of Wanjiku's Business Problem

Wanjiku operates a secondhand clothing (*mitumba*) retail and wholesale stall within Nairobi's vibrant Gikomba Market, East Africa's largest trading hub. While her stall experiences robust customer traffic during fresh bale opening days ("camera" high-demand cycles), she contends with sharp daily revenue volatility, escalating operational overheads—such as Nairobi City County cess, secure storage, porterage, and casual labor—and erratic inventory depletion across popular items like denim jeans and winter jackets. Lacking a structured data-driven tracking system and currently co-mingling personal finances with operational cash flow, Wanjiku is unable to verify which trading days truly generate positive economic returns after overheads, nor can she project the working capital required to restock wholesale bales before depleting her fastest-selling merchandise.

---

## 2. How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/elijahel/plp-da-a1-gikomba-stall-analysis/blob/main/stall_analysis.ipynb)

To run this analysis:
1. Click the **Open In Colab** badge above to launch `stall_analysis.ipynb` directly in your browser.
2. Alternatively, clone this repository locally:
   ```bash
   git clone https://github.com/elijahel/plp-da-a1-gikomba-stall-analysis.git
   cd plp-da-a1-gikomba-stall-analysis
   jupyter notebook stall_analysis.ipynb
   ```
3. Run all cells from top to bottom (**Kernel → Restart & Run All**). The entire codebase uses **Core Python standard library only** (no external libraries like `pandas` or `numpy` are imported or required).

---

## 3. Top Three Findings

1. **Revenue Concentration on Bale Days (48.9% of Total Sales):** Saturday (KES 68,200) and Wednesday (KES 45,000) generated KES 113,200 combined, representing 48.9% of total weekly turnover (KES 230,500). Saturday stood out as the single most profitable day, yielding KES 50,800 in net profit at a 74.5% profit margin.
2. **Operational Squeeze on Low-Traffic Days (Tuesday 51.4% Cost Ratio):** Tuesday yielded only KES 14,000 in revenue against KES 7,200 in operating costs, leaving an anemic net profit of KES 6,800. Daily overheads consumed 51.4% of Tuesday's gross takings, demonstrating that fixed operational costs heavily penalize the business when customer volume dips.
3. **Severe Stockout Hazard in High-Margin Categories:** Fast-moving staples—most notably Denim Jeans (18 units remaining vs. 30 unit safety threshold), Heavy Jackets (12 remaining vs. 20 threshold), and Sportswear (8 remaining vs. 20 threshold)—are severely depleted. At current sales velocity, Wanjiku risks losing over KES 38,000 in upcoming weekend demand unless an estimated KES 36,250 restocking order is placed immediately.
