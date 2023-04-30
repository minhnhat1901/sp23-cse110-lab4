# Question 1
For *line 12*, it's printed: 
> 3

For the for-loop, variable *i* is initialized by **var** keyword, and it iterates until *i* is equal to the length of the *prices* array. We know that at *line 19*, prices array has 3 elements, so the length is 3. Therefore, by break the loop, *i* needs to be 3, as a false condition for comparing with the length of *prices*. Because it's declared by **var**, it will be logged to the console and print out ***3***.

# Question 2
For *line 13*, it's printed: 
> 150

Variable *discountedPrice* is using **var** keyword to declare, and because it's staying inside the for-loop, this means that variable *discountedPrice* keeps declaring and defining everytime the for-loop executed, until the loop breaks. Even though the loop runs 3 times, the value for variable *discountedPrice* got changed until the last time the loop executes. Therefore, we got ***150*** as a final answer.

# Question 3
For *line 14*, it's printed: 
> 150

It's much similar to Question 2, instead of using **var** keyword for declaring the variable inside the for-loop block function, we only need to declare outside the loop, and the value of variable will keep updated when the for-loop is executed. The last time the loop runs, by plugging the value of *discountedPrice* into the equation (300), do the calculation, it returns the value and assign to the *finalPrice*, which then displays to the console by line 14. 

# Question 4
The function *discountPrices* takes two arguments: an array of *prices* and a *discount* value. It runs through the array of *prices*, based on the length of that array, applying the *discount* to each price. Then, it rounds result to two decimal places, and pushes the final price into the *discounted* array, which declared in the function by **var** keyword. Finally, it returns the array of *discounted* prices.

Follow each step of calculation, we will have the result:

```
100 * (1 - 0.5) = 50
200 * (1 - 0.5) = 100
300 * (1 - 0.5) = 150
```

Because the given value is integer, so we don't need to round the value. Therefore, the returned array is [50, 100, 150].

# Question 5
This code will have a ReferenceError because i is declared by **let** keyword. By definition of **let**, it can't be accessed outside the code block {...}, therefore, because it's declared inside the for-loop, it can be used within the loop, not outside. 

# Question 6
Similar to Question 5, *let* keyword restricts the variable to be accessed from the outside of the code block {...}. Therefore, the code causes a ReferenceError which states that *discountedPrice* is not defined, even though it's defined in the code. 

# Question 7
The console will display the value:
> 150

This is different from the Question 5 and 6 because the place where the variable is declared. *finalPrice* is declared outside the for-loop function, but it still guarantees to stay in the same code block {...} with the console.log(...). Therefore, the variable can be found and display in the terminal 