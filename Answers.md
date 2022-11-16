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

## Q11
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1, num2, num3) {
  return num1 + num2 + num3
}

const num1 = 10
const num2 = 1
const num3 = 20

const result = myFunction(1, 1, 1)
```
calls the function `myfunction` which takes three arguments, and returns a value of them added together. `myFunction` is called with (1, 1, 1) the result three will be saved to the variable const result.

Result - we were correct.

### Q12
What will be the value of `result` when this code runs? Why?

```javascript
function getSomeValue() {
  return 2
}

function myFunction(num1) {
  const num2 = getSomeValue()
  return num1 * num2
}

const result = myFunction(5)
```
We called the function `myFunction` with an argument of 5. this then calls the `getSomeValue` function which gives us a value for `num2`. `myfunction` then multiples the `num1` argument with the `num2` variable which returns of value 10.

Result - We were correct.

## Q13
What will be the value of `result` when this code runs? Why?

```javascript

function getSomeValue() {
  return 2
}

function myFunction(num1) {
  const num2 = getSomeValue()
  return num1 * getSomeValue()
}

const result = myFunction(5)
```
We called the function `myFunction` with an argument of 5. `myfunction` multiplies the arguments by the `getSomeValue` function which in this case equals `2`. We will get a result of `10`.

Result - We were correct.

### Q14
What will be the value of `result` when this code runs? Why?

```javascript
function getSomeValue() {
  return 2
}

function myFunction(num1) {
  return getSomeValue() * getSomeValue()
}

const result = myFunction(5)

```
Calling `myfunction` just return `getSomeValue` multiplie `getSomeValue` and doesn't use the inputed argument. The result should be `2*2` which equal `4`.

Result - we were corect.

## Q15
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1) {
  if(true) {
    return -10
  }

  return num1 * 10
}

const result = myFunction(5)
```
Calling `myFunction` only the code up to the first return will run. because the if statment is true, the function `myFunction` will return `-10`.

Result - we were correct.

### Q16
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1) {
  if(false) {
    return -100
  }

  return num1 * 10
}

const result = myFunction(5)
```
Calling `myFunction` with the argument `5`, the if statement is `false` and won't execute, so the code contiounus to the return statement `num1 * 10`. Which will return a value of 50. 

Result - we were correct.

### Q17
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1) {
  return -100

  return num1 * 10
}

const result = myFunction(5)
```
Calling `myFunction` will immediately return `-100` because the return statement is on it's first line.

Result - we were correct.

### Q18
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1) {

  return num1 * 10

  return -100
}

const result = myFunction(5)
```

Calling `myFunction` will immediately return `num1*10` because the return statement is on it's first line. `num1` the argument given which is 5, `myFunction` will return a value of 50 into result variable.

Result - we were correct.

### Q19
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1, num2, num3) {
  return num2
}

const result = myFunction(5, 10, 15)
```
Calling `myfunction` with three arguments, it immediately returns the second argument. The variable result will equal `num2` which is `10`. 

Result - We were correct.

### Q20
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1, num2, num3) {
  return num1 + num3
}

const num1 = 20
const num2 = 200
const num3 = 1000

const result = myFunction(5, 10, num3, 15)
```
`myFunction` takes three arguments. We called it with four arguments, the forth argument will be ignore. `myfunction` will return the first and third arguments added together. the first argument is`5` and the thied argument is `num3` which is saved as a variable with a value of `1000`. So the variable result will equal `5+1000` which is `1005`.

Result - we were correct.

### Q21
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1, num2) {
  const result = num1+num2
  return result
}

const result = myFunction(10, 20)
myFunction(100, 2)
```
`myFunction` takes two arguments and creates a variable named result and added two arguments together. and returns that value. the constant result is in the function scope, so won't effect the constant result on line `355`. `myfunction` is called twice the first time with arguments `10 and 20`, So `30` is saved to the result variable. the second time it is called with `100 and 2` so outputs `102`. 

Result - we were correct but, line `356` did not output it's value visibly. 

### Q22
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1, num2) {
  let result = num1+num2
  return result
}

let result = 0
myFunction(100, 2)
```

`myFunction` takes two arguments and adds them together and returns the result. the result isn't saved anywhere but it's returned anyway with a value of `100+2` which is equal `102`. 

Result - we were correct.

### Q23
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1, num2) {
  result = num1+num2
}

let result = 0
myFunction(100, 2)
```
`myfunction` has no return statement so it will do the calculation of `num1+num2` which equal `100+2` but it will not return any value back to us.

Result - we were correct but the `myfunction` did return a value of undefined.

### Q24
What will be the value of `result` when this code runs? Why?

```javascript
function myFunction(num1, num2) {
  const result = num1+num2
  return 100
}

const result = myFunction(5, 2)
```

`myfunction` takes two arguments adds them together storing them in the result variable within the function but, always return `100`. so the constant variable on line `403` will equal `100`. 

Result - we were correct.

### Q25
What will be the printed out by the console log statements when this code runs? Why?
```javascript
function myFunction(a) {
  let b = 20
  
  console.log("a:", a)
  console.log("b:", b)
  console.log("c:", c)
}

let a = 1
let b = 2
let c = 3

myFunction(100)
```
`myfunction` will log to the console `"a:" 100, "b:" 20, "c:" 3`. 

Result - we were correct. 