# Closure..
## A Closure is the combination of the function along with its lexical environment/scope.
- Example 01
```js
function x(){
    var a=10;
    function y(){
        console.log(a);
    }
    y();
}
x();
```
- Output
```
10.
```
