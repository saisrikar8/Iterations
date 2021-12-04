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

**Explanation:**

The *loop variable* `i` is initialized to 1, and the termination condition `i < 5` is evaluated. If it is `true` the loop is executed, and then the variable `i` is incremented according to the update statement. As soon as the termination conditiion is `false` (i.e., i>=5), control passes to the first statement following the loop.

*Note:*

1. The loop variable should not have its value changed inside of the loop body.

2. The initializing and the update statements can use any valid constants, variables, or expressions.
3. The scope of the loop variable is restricted to the loop body.

### Enhanced *for* loop (For-each Loop)

This is used to iterate over an array or collection.

```java
for(SomeType element: collection){
	statements
}
```

*Note: *

1. The enhanced *for* loop should be used for accessing elements in the data structure, not for replacing or removing elements.
2. The loop hides the index variable that is used with arrays.

## *While* Loop
Boolean test is performed at the beginning of the loop, if `true`, the loop body is executed, otherwise, we continue.

**Examples**
```java
int mult3 = 3;
while(mult3 < 20){
	System.out.print(mult3+" ");
	mult3 += 3;
}
```

*Note:*

1. It is possible for the body of a `while` loop never to be executed.
2. Beware of infinite loops, which happens when the boolean test is never false. Don't forget to change the loop variable in the body of the loop.


## *do-while* loop
Similar to a `while` loop, however, it checks for the condition *after* executing the loop body;

**Example**
```java
int i = 1;
do{
	System.out.println("Hello World");
	i++;
}
while(i>6);
```

## Nested Loops
You create a *nested loop* when a loop is a statement in the body of another loop.

**Example**
```java
for (int i = 1; i<3; i++){
	for(int j = 1; j <= 4; j++){
		System.out.println("*");
	}
	System.out.println();
}
```

Think:

for each of 3 rows{

	print 4 stars
	go to next line

}
>Output:

>`****`

>`****`

>`****`
