### Lexical Environment
-Example1:
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
_Example2:
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
_Example3:
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
