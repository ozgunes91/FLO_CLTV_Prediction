> **Note:** This project was developed for educational purposes as part of the Miuul Data Scientist Bootcamp and aims to demonstrate probabilistic CLTV modeling using synthetic retail data.

# 📄 Project Report: FLO CLTV Prediction

## Objective
To predict Customer Lifetime Value (CLTV) using probabilistic models, enabling FLO to optimize marketing strategies and allocate resources based on expected customer value.

## Methodology
- Data Cleaning: Outliers were capped using interquantile thresholds.
- Feature Engineering: Total purchases, total spending, and weekly recency, T, frequency, and monetary values were derived.
- Modeling:
  - BG/NBD model predicted expected purchases in 3 and 6 months.
  - Gamma-Gamma model estimated expected average monetary value.
  - CLTV was calculated for a 6-month horizon.
- Segmentation: Customers were segmented into A–D based on CLTV scores using quartiles.

## Key Findings
- CLTV values vary widely across the customer base.
- The top 5% of customers (CLTV > 424 TL) have an average CLTV of **592.73 TL**, significantly above the population average.
- Segment A customers have an average CLTV of **~385 TL**, high purchase frequency, and above-average spending behavior.

## Strategic Recommendations
- **Segment A:** Launch personalized loyalty campaigns and exclusive offers to retain top customers and increase engagement.
- **Segment B:** Offer targeted promotions to encourage upsell and cross-sell behaviors.
- **Segment C:** Monitor carefully; these customers could churn. Consider limited-time offers or reminders to reactivate them.
- **Segment D:** Low potential value—focus acquisition efforts elsewhere or use cost-effective, automated marketing.

## Conclusion
These insights may help inform more data-driven marketing decisions in similar retail contexts.