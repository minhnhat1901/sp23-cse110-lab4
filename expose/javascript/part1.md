# Question 1
For *line 9*, it's printed:
> values added: 20

# Question 2
For *line 13*, it's printed:
> final result: 20

# Question 3
For *line 9*, it's printed:
> values added: 20

# Question 4
For *line 13*, it doesn't print anything since it throws an ReferenceError in Terminal. By definition, declaring a variable with **let** keyword which means we can only access that variable within the block scope {...}. If we call that variable outside the code block, we can't use it.

# Question 5
For *line 9*, it doesn't print anything since it throws an TypeError in Terminal. By definition of **const** keyword, we can't reassign the value after initializing in the first time. Therefore, the code will stop at *line 7* and throws the error.

# Question 6
For *line 13*, it also doesn't print out anything since it's firstly having an error at *line 7*, which conflicts the rule of using **const** keyword. Also, **const** keyword is much similar to **let** keyword when we can't call the variable which is defined within the code block from the outside. Even we pass an error from *line 7*, we still have an ReferenceError.