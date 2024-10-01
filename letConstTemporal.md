# Let Const & Temporal Dead Zone 
## Difference between let and var.
- Well, var can be re-declared but let can't. `let` is introduced in Javascript so that it can only used in the scope whereas `var` can be accessed anywhere in the immediate function.
## Let and Const use Hoisting??
- The answer is yes. However, the hoisting happened in the temporal dead zone, which is the time between declaration and initialization. Both `let` and `const` are stored in the memory but
  not in the typical global memory space, they are stored in the special memory in JVM `script`. That's why `let` and  `const` can't be accessed through window/this object.
# Error
## Reference Error

<p align="center">
  <img src='./image/Screenshot (245).png' alt = "Reference Error">
</p>

## Type Error 

<p align="center">
   <img src='./image/Screenshot (246).png' alt = "Type Error">
</p>

## Syntax Error

<p align="center">
  <img src='./image/Screenshot (244).png' alt = "Syntax Error">
</p>
