# First Class Function, Function Statement, Function Expression

## Function statement{hoisting problem because when c invoke it stored as value undefined}
```js
a();
c();
function a(){
    console.log("funciton a");
}


//Function Expression
var c= function (){
    console.log("function `C`");
    return x;
}
```


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
```


const p=s;

p(d);
console.log(p);
