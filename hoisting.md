## Hoisting 
When a javascript code runs into a machine two components are created **Memory/ Variable Environment** and **Code Execution/ Thread**. So first of all the program goes into the Variable Environment or Memory part where all the 
function and variable is stored. And then comes the code execution by using a call stack. So if someone log the variable before they initialise the value it print ```undefined``` because of that memory part.
- Example:
   

``` js
console.log(s);
console.log(display);
function display(){

}
var s=10;

```
**Output**
```
console.log(s): Undefined.
console.log(display): Display the whole function.

```
