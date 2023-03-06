# Receipts-for-Lovely-Loveseats

We’ve decided to pursue the dream of small-business ownership and open up a furniture store called Lovely Loveseats for Neat Suites on Fleet Street. With our newfound knowledge of Python programming, we’re going to build a system to help speed up the process of creating receipts for your customers.

In this project, we will be storing the names and prices of a furniture store’s catalog in variables. You will then process the total price and item list of customers, printing them to the output terminal.


------------

	1.
Let’s add in our first item, the Lovely Loveseat that is the store’s namesake. Create a variable called lovely_loveseat_descriptionand assign to it the following string:

```
Lovely Loveseat. Tufted polyester blend on wood. 32 inches high x 40 inches wide x 30 inches deep. Red or white.
```
	Hint
Recall string assignment syntax:

```
variable_name = "This is a string"
```
	2.
Great, now let’s create a price for the loveseat. Create a variable lovely_loveseat_priceand set it equal to 254.00.
	Hint
Assign the variable same as the string before, but leave out the quotes since we’re storing a number:

```
numeric_variable = 10.00
```
	3.
Let’s extend our inventory with another characteristic piece of furniture! Create a variable called stylish_settee_descriptionand assign to it the following string:

```
Stylish Settee. Faux leather on birch. 29.50 inches high x 54.75 inches wide x 28 inches deep. Black.
```
	4.
Now let’s set the price for our Stylish Settee. Create a variable stylish_settee_priceand assign it the value of 180.50.
	5.
Fantastic, we just need one more item before we’re ready for business. Create a new variable called luxurious_lamp_descriptionand assign it the following:

```
Luxurious Lamp. Glass and iron. 36 inches tall. Brown with cream shade.
```
	6.
Let’s set the price for this item. Create a variable called luxurious_lamp_priceand set it equal to 52.15.
	7.
In order to be a business, we should also be calculating sales tax. Let’s store that in a variable as well.

Define the variable sales_taxand set it equal to .088. That’s 8.8%.

Our First Customer

	8.
Our first customer is making their purchase! Let’s keep a running tally of their expenses by defining a variable called customer_one_total. Since they haven’t purchased anything yet, let’s set that variable equal to 0for now.
	9.
We should also keep a list of the descriptions of things they’re purchasing. Create a variable called customer_one_itemizationand set that equal to the empty string "". We’ll tack on the descriptions to this as they make their purchases.
	Hint
An empty string is a string without any characters in it. Assign it just like any other variable:

```
empty_string = ""
```
	10.
Our customer has decided they are going to purchase our Lovely Loveseat! Add the price to customer_one_total.
	Hint
The price for the loveseat is saved in lovely_loveseat_price. Add it to the total like so:

```
customer_one_total += lovely_loveseat_price
```
	11.
Let’s start keeping track of the items our customer purchased. Add the description of the Lovely Loveseat to customer_one_itemization.
	Hint
The description is in the lovely_loveseat_descriptionvariable. Recall you can use the plus-equals operator to add strings to an existing variable.

```
customer_one_itemization += lovely_loveseat_description
```
	12.
Our customer has also decided to purchase the Luxurious Lamp! Let’s add the price to the customer’s total.
	Hint

Add luxurious_lamp_priceto customer_one_total.

	13.
Let’s keep the itemization up-to-date and add the description of the Luxurious Lamp to our itemization.
	14.
They’re ready to check out! Let’s begin by calculating sales tax. Create a variable called customer_one_taxand set it equal to customer_one_totaltimes sales_tax.
	Stuck? Get a hint
	15.
Add the sales tax to the customer’s total cost.
	Hint

Update the variable customer_one_totalby adding customer_one_taxto it.

	16.
Let’s start printing up their receipt! Begin by printing out the heading for their itemization. Print the phrase "Customer One Items:".
	Hint
Use the print()function and pass in the string to print, like so:

```
print("Your phrase here")
```
	17.
Print customer_one_itemization.
	Hint
Use the print()function to print the variable like so:

```
print(customer_one_itemization)
```
	18.
Now add a heading for their total cost: Print out "Customer One Total:"
	19.
Now print out their total! Our first customer now has a receipt for the things they purchased.
	20.
  
  
  ------------------
  
  # Furniture items for sale and their prices
lovely_loveseat_description = '''Lovely Loveseat. Tufted polyester blend on wood. 32 inches high x 40 inches wide x 30 inches deep. Red or white.'''
lovely_loveseat_price = 254.00
stylish_settee_description = '''Stylish Settee. Faux leather on birch. 29.50 inches high x 54.75 inches wide x 28 inches deep. Black.'''
stylish_settee_price = 180.50
luxurious_lamp_description = '''Luxurious Lamp. Glass and iron. 36 inches tall. Brown with cream shade.'''
luxurious_lamp_price = 52.15
#sales tax ------
sales_tax = .088

# customers and transactions------
customer_one_total = 0 
customer_one_itemization = ''
# updated customer one price 
customer_one_total += lovely_loveseat_price
customer_one_itemization += '''Lovely Loveseat. Tufted polyester blend on wood. 32 inches high x 40 inches wide x 30 inches deep. Red or white.'''
#customer added the lamp to their total checkout price
customer_one_total += luxurious_lamp_price
customer_one_itemization += '''Luxurious Lamp. Glass and iron. 36 inches tall. Brown with cream shade.
'''

# Calculate the sales tax here
customer_one_tax = customer_one_total * sales_tax
#add the sales tax to the customer's total cost 
customer_one_total += customer_one_tax 
print('Customer One Items:')
print('')
print(customer_one_itemization)
print('')
print('Customer One Total:')
print(customer_one_total)
