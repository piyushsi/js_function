1. 🎖Write a function named calculateDogAge that:
  * [ ] Takes 1 argument: your puppy's age.
  * [ ] Calculates your dog's age based on the conversion rate of 1 human year to 7 dog years.
  * [ ] Outputs the result to the screen like so: "Your doggie is NN years old in dog years!"
  * [ ] Add an additional argument to the function that takes the conversion rate of human to dog years.
  
 
```js
// your code goes here function calculateDogAge (dogAge) {
  
 function calculateDogAge (puppyAge) {
  dogAge = (puppyAge*7);
  return (`Your doggie is ${dogAge} years old in dog years!`);
  }
```
2. 🎖Write a function named calculateSupply that:
  * [ ] takes 2 arguments: age, amount per day.
  * [ ] calculates the amount consumed for rest of the life (based on a constant max age).
  * [ ] outputs the result to the screen like so: "You will need NN to last you until the ripe old age of X"
  * [ ] Accept floating point values for amount per day, and round the result to a round number.

```js
// your code goes here
function calculateSupply(age,amount){
  const maxAge = age * 365 ;
  totalAmount = (maxAge * amount);
  return (`You will need ${totalAmount}to last you until the ripe old age of ${age}`);

}
```
3. 🎖Create a function called celsiusToFahrenheit:
  * [ ] Store a celsius temperature into a variable.
  * [ ] Convert it to fahrenheit and output "NN°C is NN°F".
  * [ ] Create a function called fahrenheitToCelsius:
  * [ ] Now store a fahrenheit temperature into a variable.
  * [ ] Convert it to celsius and output "NN°F is NN°C."

```js
// your code goes here

function celsiusToFahrenheit(cel) {
  let celTemp = (fah - 32) / 1.8;
    return `${cel}C is ${fah}F`;
}
  function fahrenheitToCelsius(fah) {
    let fahTemp = celsius * 1.8 + 32;
    return `${farenheit}C is ${celsius}F`;
  }
```
4. 🎖The function below returns true if the parameter age is greater than 18. Otherwise it asks for a confirmation and returns its result:

```js
function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    // ...
    return confirm("Did parents allow you?");
  }
}
```
  4.1 🎖Convert the above function using ternary operator.
  ```js
  // your code goes here
  console.log((age > 18)? true : confirm("Did parents allow you?"));

  ```

  4.2 🎖Convert the above function using `||` operator.
  ```js
  // your code goes here

function checkAge(age) {
  return (age > 18) ||  confirm("Did parents allow you?");
}

  // ...
  return confirm("Did parents allow you?");
}
checkAge()
  ```
Will the function work differently if else is removed like below?

```js

```
Is there any difference in the behavior of these two variants? If there is what is that?


5. 🎖 Write a function pow(x,n) that returns x in power n.

  * [ ] Use prompt to take values for x and n, and then shows the result of pow(x,n) using alert.
  * [ ] In this task the function should support only natural values of n: integers greater then 1.

```js
// Your code goes here
function pow(x,n) {
  var x = +prompt("enter an integer");
  var n = +prompt("enter 2nd integer")
  if (n <= 1) {
  alert ("integers less then 1 is not allowed");
  } else {
    return x ** n ;
  }
}
pow()

// After writing code uncomment to check the answer.
// pow(3, 2); // 9
// pow(3, 3); // 27
// pow(1, 100); // 1
// pow(-31, 2); // "The number below 1 is not allowed"
````

6. 🎖Write a program that asks the user for a number n and gives them the possibility to choose between computing the sum and computing the product of 1,…,n. Return the result accordingly.

```js
// your code goes here
function factorial(n) {
    let input = 1;
    for (var i = 1; i <= n; i++) {
      input = i * input;
    }
    return input;
  }
  function chooseOperation() {
    let num = prompt('Enter an integer.');
    let operator = prompt('Enter one of following operator: sum or product');
    switch (operator){
      case "sum": 
      return num*(num+1);
      break;
      case "product": 
      return factorial (num);
      break;
    }
  }
```
6. 🎖Write a program that asks the user for a number n using prompt and prints the sum of the numbers 1 to n

```js
// your code goes here
function sum() {
  let n = +prompt ("enter an integer");
  let sum = 0;
  for (i = 1 ; i <= n ; i=(i+1)) {
    sum += i;
  }
  return sum;
}
```
7. 🎖Modify the previous program such that only multiples of 5 or 7 are considered in the sum, e.g. n = 20 (5,7,10,14,15,20) 71

```js
// your code goes here
function sum() {
  let n = +prompt ("enter an integer");
  let sum = 0;
  for (i = 1 ; i <= n ; i++) {
    sum += i;
  }
  if (n % 5 == 0 || n % 7 == 0) {
  return sum;
  } else {
    return("Enter a valid Number");
  }
  }
```

8. 🎖Write a function `min` that takes two arguments and returns their minimum.

```js
// Your code here.

console.log(min(0, 10));
// → 0
console.log(min(0, -10));
// → -10
function min(x,y) {
  return math.min(x,y);
}
console.log(min(0, 10));
// → 0
console.log(min(0, -10));
// → -10
```