# JavaScript Cheat Sheet

## Math Operations

- Addition
- Subtraction
- Multiplication
- Division
- Modulus (%)
- Exponentiation (**)
- Increment (++)
- Decrement (--)

### Modulus (/ Remainder Operator)

27 % 2 (Output 1. 27/2=13 Rest is 1. Can be used to determine if a number is even or odd.)

### Exponentiation

3**2 (Output 9. 3^2=9.)

### Increment/decrement

3++ same as 3+1
3-- same as 3--

### Assignment operators

3+=2 same as 3+2=
3 **= 2 same as 3^2=
3 %= 2 same as 3 % 2 =

## String Properties and Methods

### String index

stringVar[0]; (Output the 1st letter.)

### String length

stringVar.length; (Output the number of letters in the string.)

### Some string methods
### [thing.method();]

stringVar.toUpperCase(); (Makes the string uppercase.)
stringVar.toLowerCase(); (Makes the string lowercase.)
stringVar.trim(); (Removes spaces from the start/end.)
"   Hello!".trim().toUpperCase(); (Makes the string "HELLO!")

### Some other string methods
### [thing.method(arg);]

**indexOf**

let animal = 'catdog';

animal.indexOf('cat'); (Output 0.)
"catdog"('dog'); (Output 3.)
animal.indexOf('z'); (Output -1. Means: Not found.)

**slice**

str.slice(beginIndex[, endIndex])

const str = 'The quick brown fox jumps over the lazy dog.';
console.log(str.slice(4, 19)); (Output: "quick brown fox")

If we put -x, then it takes the last x letters.

**replace**

const p = 'The quick brown fox jumps over the lazy dog.';

p.replace('dog', 'monkey');
(Output: "The quick brown fox jumps over the lazy monkey.")

**repeat**

"LOL".repeat(3); (Output: LOLLOLLOL)

### String Template Literals
### (Meaning: Strings and variables in the same line)

\`Hello! My name is ${myName.toUpperCase} and I'm ${myAge}.\`
(Output: Hello! My name is DANIEL and I'm 28.)

## Objects

### Math Objects

Math.floor(23.90); (Output: 23. Rounds down.)
Math.ceil(23.20); (Output: 24. Rounds up.)

Math.random(); (Output: Random number between 0 and 1.)
Math.floor(Math.random()*10+1); (Random number between 1 and 10.)

Math.round(4.55) (Output: 5.)
Math.abs(-455) (Output: 455.)
Math.pow(2, 5) (Output: 2^5=32.)

### parseInt

parseInt("99"); (Changes a string to an integer.)

### Prompt

let userInput = prompt("Please enter something.")

userInput will be what the user typed in the popup window.

### Object Literals

**Declaring**

const myWife = {
    name: 'Sara Harka',
    age: 25,
    hairColor: 'red',
    attributes: ['#smart', '#kind', '#important'],
    hot: true
}

**Accessing, editing and adding**

myWife['age']; (Output: '25')
**or**
myWife.age; (Output: '25')

Can be updated:
myWife.age = 99;

New item can be added:
myWife.favAnimal = 'cat';
**or**
myWife['favAnimal'] = 'cat';
(Adds cat to the object.)

## Arrays

let stuff = [true, 69, 'cat', null];

stuff[2]; (Output: "cat".)
stuff.length; (Output: 4. Cuz 4 items.)

**Array actions**

arrayVariable.push('string'); (Pushed the string in the end.)
arrayVariable.pop(); (Pops the last variable from the end.)
arrayVariable.shift(); (Shifts the first variable from start.)
arrayVariable.unshift('string'); (Unshifts a string to start.)

let cats = ['Misty', 'Kitty']
let dogs = ['Barky', 'Doggy']
let animals = cats.concat(dogs);

cats.includes('Misty');
(Checks if array includes a string. Boolean answer.)

dogs.indexOf('Barky');
(Tells position of an array item, like indexOf string.)
(-1 means not found.)

animals.reverse(); (Reverses array order.)

animals.slice(1,3);
(Returns the 2nd and 3rd item. 4th not included.)
(-nums also work.)

months.splice(4, 1, 'May');
(Replaces 1 element at index 4.)
console.log(months);
(Output: Array ["Jan", "Feb", "March", "April", "May"])

**Sort**

const months = ['March', 'Jan', 'Feb', 'Dec'];
months.sort();
console.log(months);
(Output: Array ["Dec", "Feb", "Jan", "March"])

const array1 = [1, 30, 4, 21, 100000];
array1.sort();
console.log(array1);
(Output: Array [1, 100000, 21, 30, 4])


**Functions**

function functionName() {
  console.log("Hello World");
}
functionName();


function testFun(param1, param2) {
  console.log(param1, param2);
}
testFun(param1, param2); 
