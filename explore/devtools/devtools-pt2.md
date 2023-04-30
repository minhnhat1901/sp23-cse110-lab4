**1. What was the bug?**
> First number I enter is 1, and the second number I enter is 2, and the result ends up with 12, which is similar to the way we concatenate a string, which also display in my watchlist of typeof(result) -> string

**2. How would you fix it?**

At the line 11, I will make a conversion for 2 variables of *num1* and *num2* into ***Number*** datatype so that it's in numberic format, then adding 2 numbers together and assign to result. This will provide the final result.

> let result = Number(num1) + Number(num2);