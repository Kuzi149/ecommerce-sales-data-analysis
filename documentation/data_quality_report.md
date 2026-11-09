# Data Quality Report

## 1. Overview
This report summarises the data-quality checks performed on the synthetic e-commerce sales dataset.

The objective was to improve data consistency, identify missing or unmatched records, and prepare the dataset for reliable sales analysis.

## 2. Data Quality Checks

The following checks were performed:

- **SKU standardisation:** Removed unnecessary spaces and standardised SKU formatting.
- **Duplicate SKU checks:** Checked product records for duplicate SKU values.
- **Missing price checks:** Identified products with missing unit prices.
- **SKU matching:** Compared order SKUs against the product reference table.
- **Cost validation:** Checked whether matched order records had available product costs.
- **Revenue validation:** Checked the consistency of gross sales, discounts, net revenue, and estimated gross profit calculations.

## 3. Key Results

| Metric | Result |
|---|---:|
| Matched order lines | 745 |
| Unmatched order lines | 8 |
| Matched order lines affected by missing prices | 23 |
| Matched order lines missing cost | 0 |
| Total net revenue | $24,770.03 |
| Estimated gross profit | $14,005.48 |

## 4. Issues Identified

### Unmatched SKUs
Eight order lines contained SKUs that could not be matched to the product reference table. These records were flagged for review.

### Missing Product Prices
Twenty-three matched order lines were affected by missing product prices. These records require review before their revenue figures can be treated as complete.

### Missing Costs
No matched order lines were identified as missing product cost information.

## 5. Business Analysis Findings

The analysis identified the following findings:

- Social was the highest-revenue sales channel.
- Hoodie was the top product by revenue.
- Electronics was the highest-revenue category.
- December recorded the highest monthly net revenue.
- September recorded the lowest monthly net revenue.

## 6. Limitations

The dataset is synthetic and intended for portfolio demonstration.

Records with unmatched SKUs or missing prices can affect the completeness of revenue analysis. These limitations should be considered when interpreting the results.

## 7. Conclusion

The project demonstrates practical data cleaning, validation, lookup formulas, revenue calculations, and dashboard reporting.

The data-quality checks helped identify records requiring further review and provided a foundation for more reliable business analysis.
