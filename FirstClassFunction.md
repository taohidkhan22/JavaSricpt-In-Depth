# First Class Function, Function Statement, Function Expression

## Function statement
```js

a();
function a(){
    console.log("funciton a");
}

```
## Function Expression
```js
c();
var c= function (){
    console.log("function `C`");
    return x;
}

```
_The main difference between `Function Statement` and `Function Expression` is the hoisting problem. That is when `function c` is invoked it is stored as value `undefined` and as for `functionn a` in the Function Statement that was stored as function definition so there would be no hoisting issue._

## Named `Function Expression`
```js
var d= function abc(){
    console.log(abc);
}

d();
```
## First class Function
```js
let s= function xxx(param){
    console.log('First class function');
    console.log(param);
    return xxx;
   
}


const p=s;

p(d);
console.log(p);
```

## Anonymous Function
A function without a name is an anonymous function.
- example:
  ``` js
  function(){
     // statement
  }
  ```

