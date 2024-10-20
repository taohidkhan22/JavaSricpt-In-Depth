# First Class Function, Function Statement, Function Expression

## Function statement
```js
a();
c();
function a(){
    console.log("funciton a");
}

```
## Function Expression
```js
var c= function (){
    console.log("function `C`");
    return x;
}
c();
```
_{The main difference between `Function Statement` and `Function Expression` the hoisting problem is when `function c` is invoked it is stored as value `undefined`}_

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

