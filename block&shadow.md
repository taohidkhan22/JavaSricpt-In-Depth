# Block Scope 
- Curly braces define the block.
- when multiple statements in the js needs to combine together then the term block comes up.
- `Let` and `const` are block scope 
- `var` in the global scope

``` js
{
  let a = 10;
  var  b = 20;
   const c = 30;
  console.log(a);
  console.log(b);
  console.log(c);
}
console.log(b);
console.log(a);
console.log(c);
```
*Here is the breakdown of the above code:*


<img src="./image/Screenshot (247).png">

# Shadowing
## Legal Shadow
- Example 1:
``` js
let  b=200;
{
   var a = 10;
   let  b = 20;
   const c = 30;
   console.log(a);
   console.log(b);
   console.log(c);
}
console.log(b);
```
**Output 01**
`
   console.log(a):10
   console.log(b):20
   console.log(c):30
   
   console.log(b):200
  
`
- Example 02:
``` js
var  a=200;
{
   var a = 10;
   let  b = 20;
   const c = 30;
   console.log(a);
   console.log(b);
   console.log(c);
}
console.log(b);
```
**Output 02**
```
   console.log(a):10
   console.log(b):20
   console.log(c):30
   
   console.log(b):10

```
## ILlegal Shadow
- Example 1:
  
``` js
let  b=200;
{
   var a = 10;
   console.log(a);
   var  b = 20;
   const c = 30;
  
   console.log(b);
   console.log(c);
}
console.log(b);
```
**Output 01**
```
   console.log(a):10
   console.log(b): Throw a ref error and then stop the execution of the program.

  
```
