# Takeaway Restaurant - Synchronous Code Review Exercise 1

## Prompt

I am a business analyst who'd like to get a system built up for us. 
The restaurant would like to keep track of the orders as they are 
delivered to the correct customer. A customer is identified with 
a name they give the till operator. Each order may be a breakfast, 
a snack or the chef's special each with their respective pricing. 
Each customer orders a single menu item per order. When the customers 
queue up, the till operator will use the program to take the orders for the cook. Delivery will be dealt with 
by another program. The cook will see the orders from a screen with 
the same view that the till operator has. The program must in the end provide clear user-friendly error messages
when invalid is entered.

## Illustration

### Taking an order

Current orders:
1. Customer 8 - Snack
2. Customer 9 - Chef's special
3. Customer 10 - Snack

Meal types:
1. Breakfast
2. Snack
3. Chef's special

Please enter the next order's number or 0 to indicate Customer 8's order is ready:

#### User input

1

### Order entered and indicating that the top order is ready

Current orders:
1. Customer 8 - Snack
2. Customer 9 - Chef's special
3. Customer 10 - Snack
4. Customer 11 - Breakfast

Meal types:
1. Breakfast
2. Snack
3. Chef's special

Please enter the next order's number or 0 to indicate Customer 8's order is ready:

#### User input

0

### Order served and top order becomes Customer 9's

Current orders:
1. Customer 8 - Snack
2. Customer 9 - Chef's special
3. Customer 10 - Snack
4. Customer 11 - Breakfast

Meal types:
1. Breakfast
2. Snack
3. Chef's special

Please enter the next order's number or 0 to indicate Customer 9's order is ready:

### Empty queue.

The last order was customer 11's order. There are no orders in the queue.

Meal types:
1. Breakfast
2. Snack
3. Chef's special

Please enter the next order's number:

#### User input

12

### Error screen

The customer is either unrecognised or already serviced. 

Meal types:
1. Breakfast
2. Snack
3. Chef's special

Please enter the next order's number:

#### User input

1

#### Taking an order after clearing

Current orders:
1. Customer 12 - Breakfast

Meal types:
1. Breakfast
2. Snack
3. Chef's special

Please enter the next order's number or 0 to indicate Customer 12's order is ready: