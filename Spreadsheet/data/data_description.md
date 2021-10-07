# Data Description 
Here is a description of the dataset generated for the Excel challenge:

It contains 10,000 "purchases" made in Oct-Nov 2019. For each purchase, the following data is provided:

- Purchase date (value: yyyy-mm-dd; range: October 1st  to November 30th, 2019);
- Whether the date falls into the holiday period (value: ‘holiday’ or ‘non-holiday’; the holiday period is assumed to start on November 20th, about 30% of all purchases occur during the holiday period);
- Sales channel (value: ‘In-store’ or ‘Online’; about 60% of all purchases are ‘In-store’);
- Payment method (value: ‘Cash’, ‘Debit’, ‘Credit’, ‘PPal’, ‘Apay’, ‘Gpay’; about 35%, 15%, 40%, 0%, 3%, and 7%, respectively, for in-store purchases; about 0%, 15%, 70%, 15%, 0%, and 0% for online purchases);
- Product category (values: ‘Clothing’, ‘Shoes’, ‘Accessories’; about 70%, 25%, and 5%, respectively);
- Product type:
-- for category ‘Clothing’: values - ‘Mens top’, ‘Womens top’, ‘Mens jeans’, ‘Womens jeans’   (about 18%, 28%, 22%, and 32%, respectively);
-- for category ‘Shoes’: values - ‘Mens dress shoes’, ‘Womens dress shoes’,   ‘Mens casual shoes’, ‘Womens casual shoes’ (about 24%, 14%, 36%, and 26%, respectively);
-- for category ‘Accessories’: ‘Belt’, ‘Purse’ (about 75% and 25%, respectively).
- Product identifier (values: identifiers for individual products, constructed as a string composed of the first letters of each word in the product type, all lowercase, followed by a 2-digit number; there are 8 men’s tops, 10 women’s tops, 10 men’s jeans, 12 women’s jeans, 5 men’s dress shoes, 6 women’s dress shoes, 8 men’s casual shoes, 11 women’s casual shoes, 4 belts, and 6 purses – 80 different products total);
- Base price (values are in dollars and cents, sampled for each of the 80 products from normal distributions with the following means and standard deviations, and restricted to the following ranges):
-- ‘Mens top’: mean = 35, std = 8, min = 19, max = 45;
-- ‘Womens top’: mean = 38, std = 12, min = 15, max = 50;
-- ‘Mens jeans’: mean = 60, std = 18, min = 30, max = 100;
-- ‘Womens jeans’: mean = 65, std = 25, min = 35, max = 120;
-- ‘Mens dress shoes’: mean = 70, std = 25, min = 40, max = 150;
-- ‘Womens dress shoes’: mean = 60, std = 20, min = 40, max = 120;
-- ‘Mens casual shoes’: mean = 50, std = 20, min = 30, max = 120;
-- ‘Womens casual shoes’: mean = 55, std = 25, min = 30, max = 130;
-- ‘Belts’: mean = 20, std = 7, min = 10, max = 30;
-- ‘Purses’: mean = 50, std = 23, min = 20, max = 100;
- Discount (values are 0, 5, 10, 15, 20, 25, 30, 40, 50, or 75 percent; probabilities of each value outside of the holiday period are 0.5, 0.02, 0.05, 0.03, 0.05, 0.1, 0.05, 0.05, 0.1, and 0.05, respectively; probabilities of each value during the holiday period are 0.2, 0.02, 0.05, 0.03, 0.05, 0.2, 0.05, 0.05, 0.2, and 0.15, respectively);
- Clearance (values: ‘True’ or ‘False’; ‘False’ for all discount values below 50%; ‘True’ for about 30% of items discounted by 50% and 65% of items discounted by 75% outside of the holiday period; ‘True’ for about 15% of items discounted by 50% and 85% of items discounted by 75% during the holiday period);
- Promotion (values: ‘True’ or ‘False’; ‘False’ for all in-store purchases and non-discounted online purchases; ‘True’ for about 90% of online purchases discounted by 5%, 65% - discounted by 10%, 60% - discounted by 15%, 50% - discounted by 20%, 50% - discounted by 25%, 60% - discounted by 30%, 80% - discounted by 40%, 50% - discounted by 50%, 30% - discounted by 75%).
