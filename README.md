# hw4


### How many lines are drawn each frame? In other words, how often does the for loop run?
There are 38 lines per frame. It runs 38 times.

### What do the first, second, and third appearances of the number 10 do in the code?
The first appearance of 10 sets the first line's x origin at 10. The second appearance is part of the condition of the for loop and subtracts 10 from the width. As long as x is 10 less than the width, the loop will be executed. The third appearance adds 10 to the value of variable x at the end of the iteration of the loop.

### What does a for loop that runs 100 times look like?

for (var i = 0; i < 100; i = i + 1) {
  // Do something.
}

### How many times does the loop body run each frame, once the x and y arrays are full?
6 times.

### What are two ways of increasing the spacing between rings?
increase the Z variable in the following lines of code:

```
  for (var i = 0; i < x.length; i = i + Z) {
    ellipse(x[i], y[i], 1 + Z*(x.length - i));
  }
```

### How can you make the ellipse trail longer?
increase the Z variable in the following lines of code:

```  
  x = x.slice(-Z); // keep the last Z x values
  y = y.slice(-Z); // keep the last Z y values
```
