# Answers for Understanding Functions

## Q1

```javascript
function myFunction(num1, num2) {
  return num1+num2
}
```

The code calls the `myFunction` function and passes two arguments, 5 and 5. The function adds these two numbers together and returns the result (10 in this case). The return value of the function is stored in the variable result - so when this code runs, the value of the result variable will be 10.

Result - I was correct, the code did what I expected.

## Q2

```javascript
function myFunction(num1, num2) {
  num1+num2
}

const result = myFunction(5,5)
console.log(result)
```

The code calls the `myFunction` function and passes two arguments, 5 and 5. The function then adds these two numbers together, but because there is no return, no value will be given outisde the function so nothing will happen. A constant variable named result is made with the value myFunction(5,5) - but as nothing is defined, the variable will be empty.

Result - We were correct - with the addition of the result variable being 'undefined'

## Q3

```javascript
function myFunction(num) {
  return num-1
}

let num = 10
num = myFunction(num)
num = myFunction(num)
```

Calls the function `myFunction` which takes the argument num and returns a value of num-1. In this case num starts off as 10, and will return 9. Then it is saved to the num variable on line 36. Then it is called again on line 37 and would return a value of 8.

Result - we were correct!

## Q4

```javascript
function myFunction(num) {
  return num-1
}

let num = 10
let add = 3
add = myFunction(add)
add = myFunction(add)
```
Calls the function `myFunction` which takes one argument - in this case the variable add. Add on the first call = 3, so the return value would be 3-1 which = 2. On the second call on line 54, add is now equal to 2, so will return 2-1 and set that to the add variable which would equal 1.

Result - we were correct!

## Q5

```javascript
function myFunction(num, num1) {
  console.log(num1)
}

let num = 10
let num1 = 2

myFunction(num)
```

Calls the fution `myFunction` which takes 2 arguments and console.logs the second argument. As the function takes two arguments, and we are only calling the function with one, I believe that it will console.log the value `undefined`. As we have not defined the num1 argument when calling the function.

Result - we were correct!

## Q6

```javascript
function myFunction(num, num1) {
  console.log(num1)
}

let num = 10
let num1 = 2

myFunction(num1, num)
```

Calls the function `myFunction` which takes 2 arguments num and num1 and then console.logs the second argument (num1). We call myFunction with preset variables with the values 10 and 2. So in practise, we are calling the `myFunction(2, 10)` this will then console.log the second argument, which in this case is 10.

Result - We were correct!

## Q7

```javascript
let counter = 1

function myFunction() {
  counter++
  return counter
}

myFunction()
const num = myFunction()
```

Calls the function `myFunction` which takes no arguments. The function increases the counter variable by 1, and returns the value of counter. We then set a constant variable called `num` to = the value of counter. Which by this time would be 3.

Result - We were correct.

## Q8

```javascript
function myFunction(num1, num2) {
  return num1 + num2
}

const num1 = 10
const num2 = 1
const num3 = 4

const result = myFunction(num3, num1)
```

Calls the function `myFunction` which takes two arguments and return a value of them added together. A constant variable named `result` will be created with the value of `num3+num1` which requals `4+10` which equals `14`.

Result - We were correct.

## Q9

```javascript
function myFunction(num1, num2) {
  console.log(num3)
}

const num1 = 10
const num2 = 1
const num3 = 20

myFunction(num3, num1)
```

Calls the function `myFunction` which takes two arguments, and then console.logs the variable named `num3`. Because num3 is set before we call the function, even though we pass the arguments 20 and 10, it should console log the `num3` variables value, which is `20`.

Result - We were correct.

## Q10

```javascript
function myFunction(num1, num2, num3) {
  console.log(num3)
}

const num1 = 10
const num2 = 1
const num3 = 20

myFunction(num3, num1, 100)
```

Calls the function `myFunction` which takes three arguments, and then console logs the third argument given. When `myFunction` is called with `num3, num1, 100` the values entered into the function are `20, 10, 100` so it will console log the third argument which is `100`.

Result - We were correct.