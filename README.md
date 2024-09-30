### Lexical Environment
- Example 1: This code snippet will print 14 because function b uses lexical references to the parent function c where variable x is already defined before the function execution call.
```
function c() {
  var x = 14;
  b();
  function b() {
    console.log(x);
  }
}
c();

```
- Example2: This code snippet will print undefined because function b uses lexical references to the parent function c where variable x is already defined before the function execution call
```
function c() {
 
  b();
  var x = 14;
  function b() {
    console.log(x);
  }
}
c();

```
- Example 3: This code snippet will print 14 because function b uses lexical references to the parent function c where variable x is already defined before the function execution call.
```
function c() {
 
  b();

  function b() {
    console.log(x);
  }
}
  var x = 14;
c();

```
