# Cafe Sales Analysis

This summary follows the findings and recommendations in worksheets `8_Interpret` and `9_Recommend` of [`dashboard/Cafe_Sales_Data_Analysis.xlsx`](../dashboard/Cafe_Sales_Data_Analysis.xlsx). It uses simulated 2025 point-of-sale data for four Metro Manila branches; the results do not describe a real cafe.

## Headline result

The workbook reports **₱394,428 net revenue**. BGC is the largest branch by revenue (₱140,875.50), followed by Makati (₱105,319.25), Ortigas (₱79,713.50), and Quezon City (₱68,520).

## Findings

1. **Revenue is concentrated in two branches.** BGC and Makati account for 62% of revenue. BGC leads in both transaction volume (607) and average order value (₱232). Makati has the second-highest revenue but the lowest AOV (₱214), suggesting its traffic is not being monetized as well.
2. **Drink sales vary by season.** Iced coffee contributes 45% of revenue in the hot, dry months (March–May), but 24% in December–February; its monthly revenue peaks in May (₱19,748). Hot coffee peaks in August, supporting seasonal menu and inventory planning.
3. **Meals have the highest average order value; pastries the lowest.** A meal order averages ₱308.64 versus about ₱163 for a pastry order. Meals make up only 11% of transactions, while iced coffee is the largest revenue category (32%). The workbook suggests testing a drink-and-pastry bundle.
4. **Discounts may not be earning back their cost.** Half of transactions include a discount, and ₱19,112 is given away. Discounted transactions include only 3.1% more units, while matching full-price AOV would require about 13% more. Because product mix differs, this is a signal for testing—not proof of causation.
5. **Demand has three daily peaks.** Morning (07:00–10:00) generates 34% of revenue; lunch and afternoon each contribute about 28%. Noon is the busiest hour (221 transactions). Evening (18:00–20:00) contributes about 10%.
6. **Weekend revenue per day is lower overall.** Weekends average ₱944 per calendar day versus ₱1,135 on weekdays (-17%), with a traffic gap rather than a ticket-size gap. Quezon City has a different pattern and performs more strongly on weekends.
7. **Customer segments have different order values.** Office customers average ₱239.55 per order; students average ₱208.34 among identified groups and already receive a standing 10% discount. Regulars average ₱215.17.
8. **Raw-data quality needs attention.** 73 of 1,836 raw rows (4.0%) were removed during cleaning, and additional records required corrections for spelling, dates, or blanks. Duplicates could inflate revenue and text dates could break monthly analysis.

## Recommended actions

1. Rework discounting: end blanket 15–20% promotions, cap discounts at 10%, and test targeted slow-period or add-on offers.
2. Plan stock and promotions by season: prepare iced drinks for late February–May and emphasize hot drinks in rainy and cooler periods.
3. Test a fixed-price drink-and-pastry bundle; monitor pastry attach rate, units per transaction, and AOV.
4. Match staffing to morning, lunch, and afternoon peaks; review low evening demand.
5. Improve Makati's low AOV with meal suggestions and upsizing at lunch.
6. Test weekend offers at business-district branches and student bundles in Quezon City.
7. Consider corporate or bulk-order options for office customers; review standing student and regular discounts.
8. Improve POS data entry with controlled dropdowns, a fixed date format, and required, bounded quantity values.

The workbook proposes a four-week test of discount and combo changes in two branches, with two control branches. Track AOV and units per transaction.

## Limitations

- All source transactions are simulated; real operating decisions require real POS data.
- Each row is a product line, so the basket-level drink-plus-pastry attach rate cannot be calculated directly from the row-level export.
- Comparisons show association, not cause; discounted orders also differ in product mix.
- Weekday/weekend daily comparisons do not adjust for public holidays.
