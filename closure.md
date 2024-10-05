# Closure..
## A Closure is the combination of the function along with its lexical environment/scope.
- Example 01
``` js
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
## Now things will go a little bit tricky with the next two examples 2 and 3.
### Example 2 `function y()` form a closure to the reference `varible a` with outer `function z`.  
- Example 2
``` js
function x() {
    var a=30;
  function z() {
    var a = 55;
    function y() {
      console.log(a);
    }
    y();
  }
  z();
}
x();


```
- Output
```
50
```
### Example 3 `function y()` form a closure to the reference `varible a` with outer `function x`. 
- Example 3
``` js
function x() {
  var a = 39;
  function z() {
    function y() {
      console.log(a);
    }
    y();
  }
  z();
}
x();


```
- Output
```
39
```
#### You can check the Example 02 debugger breakdown.
<img src="./image/Screenshot (249).png">



