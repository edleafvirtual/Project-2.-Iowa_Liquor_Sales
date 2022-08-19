# Project Statement:
In general, when a Licensed Vendor sells alcoholic liquor to a store, this is the one who pays to Iowa State the fee per bottle sold (column 'State Bottle Retail' in our dataset).

There are a few concepts/elements that we should clarify:
- Class E is the license to sell an unopened alcoholic liquor bottle off-premises in Iowa.
- The 'State Bottle Retail' is a fee based on the size of the 'Pack' and the 'Bottle Volume (ml)'.
- The ' Sale (Dollars)' is 'Bottles Sold' times 'State Bottle Retail'. This is the amount the stores pay to the Iowa Alcoholic Beverages Division per bottle sold. It's not the income per sale for store/vendor.
- 'Volume Sold (Gallons)' represents gallons sold by a transaction (row).

The main dataset has 24+ million rows, which includes the sales from January 1st, 2012 to current, making it pretty hard to work with Google Colaboratory.
