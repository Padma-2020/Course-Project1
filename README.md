# Course-Project1
Code Academy -Thread Shed
 want to split up daily_sales into a list of individual transactions, we are going to want to split by ,, but first, we need to replace the artifact ;,; to something without a comma, so we don’t split any transactions themselves.

Replace all the instances of ;,; in daily_sales with some other character and save the result to daily_sales_replaced.
Split daily_sales_replaced around commas and save it to a new list daily_transactions
iterate through daily_transactions (remember, this is a list of strings currently), and for each transaction, split the string around whatever character you replaced the ;,; 

Append each of these split strings (which are lists now) to our new list daily_transactions_split.
define an empty list transactions_clean.

Now, Iterate through daily_transactions_split and for each transaction iterate through the different data points and strip off any whitespace.

Add each of these cleaned up transactions to the new list transactions_clean
three empty lists. customers, sales, and thread_sold. We are going to collect the individual data points for each transaction in these lists.
iterate through transactions_clean and for each transaction:

Append the customers name to customers.
Append the amount of the sale to sales.
Append the threads sold to thread_sold
how much Thread Shed made in a day.

First, define a variable called total_sales and set it equal to 0.
consider the list sales. It is a list of strings that we want to sum. In order for us to sum these values, we will have to remove the $, and set them equal to floats.

Iterate through sales and for each item, strip off the $, set it equal to a float, and add it to total_sales
to determine how many of each color thread we sold today. Let’s start with a single color, and then we’ll generalize it.

First, print out thread_sold and inspect it
thread_sold is a list of strings, some are single colors and some are multiple colors separated by the & character.

The end product we want here is a list that contains an item for each color thread sold, so no strings that have multiple colors in them.

First, define an empty list thread_sold_split.
iterate through thread_sold. For each item, check if it is a single color or multiple colors. If it is a single color, append that color to thread_sold_split.

If it is multiple colors, first split the string around the & character and then add each color individually to thread_sold_split
now we have a list thread_sold_split that contains an entry with the color of every thread sold today.

Define a function called color_count that takes one argument, color. The function should iterate through thread_sold_split and count the number of times the item is equal to argument, color. Then, it should return this count.
Define a list called colors that stores all of the colored threads that Thread Shed offers
using the list colors, the string method .format(), and the function color_count, iterate through thread_sold_split and print a sentence that says how many threads of each color were sold today.
