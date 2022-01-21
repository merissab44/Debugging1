# Debug Log

**Explain how you used the the techniques covered (Trace Forward, Trace Backward, Divide & Conquer) to uncover the bugs in each exercise. Be specific!**

In your explanations, you may want to answer:

- What is the expected vs. actual output?
- If there is a stack trace, what useful information does it contain?
- Which technique did you use, on which line numbers?
- What assumptions did you have about each line of code, and which ones were proven to be wrong?

_Example: I noticed that the program should show pizza orders once a new order is made, and that it wasn't showing any. So, I used the trace forward technique starting on line 13. I discovered the bug on line 27 was caused by a typo of 'pzza' instead of 'pizza'._

_Then I noticed another bug ..._

## Exercise 1

I knew that the home page should show the pizza once i submitted an order and it wasn't doing that. I used the divide and conquer method starting at the order route on line 65 and the order.html starting on line 6. I noticed that the name in the html form did not match the route in app.py so I changed it so they matched.

I also decided to add console.log statements to make sure the data was posting and it wasn't grabbing the full list of toppings. After further research, I found the method should've been getlist and not just get. 

Lastly, I noticed in our route that it was adding the pizza but didn't commit it to the database. This would've resulted in not being able to display the data on the page.

## Exercise 2

First, when I ran the application , I expected to retrieve data from the api and display it on the page. I was getting an error on line 52 and so using trace forward from that line I found that the route was using users city but the template was using just city so I changed that. 

Next, I found that there was a typo a couple lines down and instead of 'temperature' it should've just said 'temp'

## Exercise 3

[[Your answer goes here!]]
