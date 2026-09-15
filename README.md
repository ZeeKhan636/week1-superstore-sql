# week1-superstore-sql
Cleaning and analyzing superstore sales data with SQL

1. Which category/sub-category generates the most sales and profit?
2. Which region has high sales but low profit margin?
3. What's the average shipping delay by ship mode?

Now on question 1 my findings are that phones and chars are the bes selleing sub categories. A store manager could focus more on these things inventory and marketing investments and should prioratize customer feedback.

Now on question 2 findings are that West region leads in both total sales (~710K) and order count (1,587), 
followed by East, Central, then South. This could suggest accessibilty or fast transportation but for reL answer we would eed more diging .

On uestion 3 fidings are that Standard Class shipping takes ~5 days to ship, far slower than Same Day (~0 days), 
First Class (~2 days), and Second Class (~3 days). Even though customers chose the cheaper 
option, 5 days feels excessive — reducing this to ~2 days could improve customer satisfaction 
without needing to eliminate the discount option entirely.

Python EDA (Pandas) 

 Found 11 rows with missing Postal Code — all from Burlington, Vermont. 
  Fixed by filling in the correct ZIP code (05401).
 Sales data is right-skewed: average sale is ~$230, but the median is only ~$54. 
  This means a few large purchases are pulling the average up — most orders are actually small.
 The largest individual sales are all Technology purchases (Copiers, Machines) — 
  high-value but infrequent, compared to Phones which sell more often at lower prices.
