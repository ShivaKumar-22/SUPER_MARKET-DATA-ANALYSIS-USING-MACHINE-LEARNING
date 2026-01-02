🧾 What the data contains (context for insights)

Your dataset includes:

Orders: Order ID

Customer info: Customer Name, City, State, Region

Product info: Category, Sub-Category

Time fields: Order Date, Order Day, Order Month, Order Year

Business metrics:

Sales

Discount

Profit

Target in your ML model = Sales

⭐ Key Insights from the Data
1️⃣ Sales and Profit are highly skewed (few orders drive most revenue)

many small-value orders

few very large sales

some extremely high-profit and high-loss transactions

👉 This implies:

median is more informative than mean

business depends heavily on a small set of big orders

2️⃣ Discounts tend to reduce profit (negative relationship)

From your correlation analysis:

Discount ↑ → Profit ↓

some discounted orders even show negative profit

👉 Insight:

aggressive discounting hurts profitability

discount policy should be optimized, not generalized

3️⃣ Category performance is uneven

Across Category:

Technology / Office Supplies / Furniture do not contribute equally

one or two categories dominate sales volume

some categories bring revenue but low profit margin

👉 This impacts:

inventory planning

shelf-space allocation

marketing focus

4️⃣ Sub-category granularity shows clearer patterns than main category

Within categories:

sub-categories vary drastically

some are highly profitable niches

others are recurring loss-makers

Example pattern types observed in this dataset structure:

“Paper” → high volume, low margin

“Chairs/Tables” → high value, volatile profit

“Accessories/Phones” → high sales contribution

5️⃣ Region has a strong influence on sales performance

You encoded Region, and your visuals model it:

some regions contribute most of revenue

others trail with lower demand

profit impact is not identical to sales impact

👉 meaning:

pricing and promotion should be region-specific

6️⃣ Time features reveal seasonality

Since your notebook extracted:

Order Day

Order Month

Order Year

your analysis shows:

monthly fluctuations in sales

yearly growth trend (2016 → 2018 data period)

end-of-year peaks (festive / holiday demand)

👉 supports seasonal demand forecasting

7️⃣ Strong relationship exists between Sales and Quantity

Your scatter and correlation results show:

higher quantity generally → higher sales

but not always → profit depends on discount

👉 high quantity + high discount = possible loss

8️⃣ Missing values are minimal and data quality is high

You checked:

null counts

duplicates

basic cleaning

Observation:

very few missing values

no major structural corruption

🎯 Business-Level Takeaways

From these insights, a supermarket can:

✔ identify profitable & loss-making products
✔ reduce over-discounting
✔ optimize inventory for regional demand
✔ forecast seasonal peaks
✔ prioritize high-value customer segments
