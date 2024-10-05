# setTimeout with Closure...

- Example 01:
``` js
function x(){
    var a=30;
    setTimeout(function(){
        console.log(a);
    },5000);
}
x();

```
- Output:
```
Print 30 after 5s.
```
- Problem Statement: Let's assume you have to print 1 after 1 second, 2 after 2 seconds, ...., 10 after 10 seconds using the setTimeout function.
- Example 01:
``` js
  function x(){
  for(var i=1;i<=10;i++){
    setTimeout(function(){
        console.log(i);
    },i*1000);
  }
  console.log("javascript in-depth");
}
x();
}
x();

```
- Output:
```
It won't print as you expected. Because javascript won't wait for anybody when we invoke the function `x()` it goes into the loop but there is a 'setTimeout' function so there will be five copies
of the 'setTimeout' along with var `i` reference. In the meantime 'console.log("javascript in-depth");` this line will be executed and the `var i` value will be `11` along with all references of `var i` and
also `var i` is in the global scope. Therefore, it will print 11 ten times.
```
To overcome the above issues we can just replace `var` with `let`. Because `let` is a block scope, it will create 10 different `i` references with the 'setTimeout' function. Or, using _closure_.


