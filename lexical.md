## Scope, Scope Chain, and Lexical Environment
**```Scope``` is an area where the specific variable can be initialized and can also be fetched.** <br>
**```Lexical Environment ``` is the local memory along with the lexical reference to its parent.**


- Example 1:  
``` js
function c() {
  var x = 14;
  b();
  function b() {
    console.log(x);
  }
}
c();

```
This code snippet will print 14 because function b uses lexical references to the parent ```function c``` where variable x is already defined before the function execution call.
- Example2: 
``` js
function c() {
 
  b();
  var x = 14;
  function b() {
    console.log(x);
  }
}
c();

```
This code snippet will print ```undefined``` because function b uses lexical references to the parent function c and ```variable x``` then was in the memory part that means code execution of ```variable x``` didn't occur. So, it was undefined.

-Example 3:
``` js
function c() {
 
  b();

  function b() {
    console.log(x);
  }
}
  var x = 14;
c();
```
 This code snippet will print 14 because function b uses lexical references to the parent ```function c``` and function c then goes into the ```global scope``` 
 where variable x is declared.
