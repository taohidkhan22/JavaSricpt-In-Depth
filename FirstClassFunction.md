# First Class Function, Function Statement, Function Expression

## First Class Function
A programming language is said to have First-class functions when functions in that language are treated like any other variable. For example, in such a language, a function can be passed as an argument to other functions, can be returned by another function and can be assigned as a value to a variable.
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


## Anonymous Function
A function without a name is an anonymous function.
- example:
  ``` js
  function(){
     // statement
  }
  ```

