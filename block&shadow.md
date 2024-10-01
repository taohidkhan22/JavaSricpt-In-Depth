# Block Scope 
- Curly braces define the block.
- when multiple statement in the js needs to combine together then the term block comes up.
- `Let` and `const` are block scope 
- `var` in the global scope

``` js
{
  let a = 10;
  var  b = 20;
   const c = 30;
  console.log(a);
  console.log(b);
  console.log(c);
}
console.log(b);
console.log(a);
console.log(c);
```
