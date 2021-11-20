## Iteration
Java has three different control structures tthat allow the computer to perform iterative tasks: `for` loop, `while` loop, and `do... while`.

### The `for` loop
The general form of a `for` loop is:

```java
for (/*initialization; termination condition; update statement*/){
	//statements(body of loop)
}
```

The termination condition is tested at the top of the loop; the update statement is performed at the bottom.

**Example**

```java
for (int i = 1; i < 5; i++){
	System.out.print(i + " ");
}
// outputs: "1 2 3 4 "
```
