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

# Question 8
Similar to Question 4, only the different between 2 questions is that now we are using **let** keyword to declare the variable. The function *discountPrices* takes two arguments: an array of *prices* and a *discount* value. It runs through the array of *prices*, based on the length of that array, applying the *discount* to each price. Then, it rounds result to two decimal places, and pushes the final price into the *discounted* array. Finally, it returns the array of *discounted* prices.

Because the given value is integer, so we don't need to round the value. Therefore, the returned array is [50, 100, 150].

# Question 9
The code causes a ReferenceError. This question is similar to Question 5 that we use **let** keyword for the variable type to declare a variable *i* using as an index of array. Because it's declared inside the for-loop function so we can't be able to access from the outside.

# Question 10
The console will display the value:
> 3

By definition of **const** keyword, it's similar to **let** keyword, except we can't reassign after the first time. For this code snippet, the *length* variable is declared by **const** keyword, and assigned by the *prices.length*, which is the fixed number representing the length of an array. How many elements the array have, it will have a correct number of length, therefore, this should be fine for the condition of using **const** keyword. Also, we declare in the same code block so the console can be able to access the variable.

# Question 11
This function will return an array 
>[50, 100, 150]

Even though the variable is declared by **const** keyword, which means we cannot reassign the array with another one. However, the element inside is still fine to reassign or add (Proof: [resource](https://www.w3schools.com/js/js_array_const.asp)).

The function then iterates over the *prices* array using a for loop. In each iteration, it calculates the discounted price by multiplying the original price by (1 - discount), which is 0.5 and pushes the discounted price into the *discounted* array. Finally, the function returns the *discounted* array, which contains a list of discounted prices.

# Question 12
A. Accessing the value of the name property in the student object
> student.name

B. Accessing the value of the Grad Year property in the student object
> student['Grad Year']

C. Calling the function for the greeting property in the student object
> stundent.greeting();

D. Accessing the name property of the object in the Favorite Teacher property in student
> student['Favorite Teacher'].name

E. Access index zero in the array of the courseLoad property of the student object
> student.courseLoad[0]

# Question 13
A. '3' + 2
> 32

Since the string adds to the integer, th integers map to their exact string representation. It ends up with the string `32`.

B. '3' - 2
> 1

For subtraction between a string to an integer, it will convert the string into an integer type and subtract both number together.

C. 3 + null
> 3

Here, null is converted to the number 0 so we add 0 with 3 to become 3.

D. '3' + null
> 3null

For addition between string and numeric, it will concatenate 2 elements together. So we end up with 3null.

E. true + 3
> 4

true maps to 1 in the addition between boolean and integer, so we have the result `4`.

F. false + null
> 0

false maps to 0, and null is converted to 0, therefore the addition will result 0.

G. '3' + undefined
> 3undefined

As an addition with string type, it will convert the other element to string and concatenate to the current string.

H. '3' - undefined
> NaN

For subtraction, it will convert the string into integer and subtract with undefined. It will result NaN - Not A Number, which is a number that is not a legal number.

# Question 14

A. '2' > 1
> true

When doing the comparison between a string and number, the string is automatically converted to a number and do the comparison.

B. '2' < '12'
> false
 
Strings are compared letter-by-letter, which based on ASCII value. Here, it will start comparing '2' with '1', here we know that the value of '1' is smaller than '2', therefore the result is false.


C. 2 == '2'
> true

When comparing values of different types, JavaScript converts the values to numbers. Therefore, '2' is converted to 2, which 2 is equal to 2.

D. 2 === '2'
> false

A strict equality operator === checks the equality without type conversion. Therefore, '2' is in string and and 2 is in number, so the result is false.

E. true == 2
> false

In Javascript, true stands for value of 1 when we convert from Boolean to number. So 1 is not equal to 2.

F. true === Boolean(2)
> true

The conversion [rule](https://javascript.info/type-conversions#boolean-conversion):
- Values that are intuitively "empty", like `0`, an empty string, `null`, `undefined`, and `NaN`, become `false`.
- Other values become `true`.

So we can conclude that for the strict equality, when Boolean(2) is executed, it becomes true, and true is equal to true with the same type.

# Question 15
***Explain the difference between the == and === operators.***

`==`: checks the equality with type conversion. Here, we will convert every type into number and then do comparison.

`===`: checks the equality without type conversion. Here, the variable type must stay at the same variable type. If it's not in the same type, then false. Otherwise, if the value is equal, then true, otherwise, return false.

# Question 16
```js
let statistics = {
    redCars: 21,
    blueCars: 45,
    greenCars: 12,
    raceCars: 5,
    blackCars: 40,
    rareCars: 2
};

for (const property in statistics) {
    let element = statistics[property];
    if (property.startsWith('r') || element % 2 === 1) {
        console.log(element);
    }
}
```

# Question 17
The result of calling *modifyArray([1,2,3], doSomething)* will be a new array *[2, 4, 6]*. At first, the *modifyArray* is called with two arguments: the array *[1, 2, 3]* and the function *doSomething*. Then, inside the *modifyArray* function, we create a new empty array called *newArr*. At line 3, a for loop iterates through each element of the input array *[1, 2, 3]* with the variable *i* representing the index of the array. For each iteration, the *callback* function - *doSomething* is called with the current element of the array as an argument. The *doSomething* function takes a number as an argument and returns the number multiplied by 2. The modified element is then pushed to the *newArr*. After all elements have been processed, the *newArr* is returned.

# Question 18
```js
function printCurrentTime() {
    let d = new Date();
    let time = d.toLocaleTimeString();
    console.log(time);
}

setInterval(printCurrentTime, 1000);
```

# Question 19
> 1
> 4
> 3
> 2




cityslot.json
expose.js
