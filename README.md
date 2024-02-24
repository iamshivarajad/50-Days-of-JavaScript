# 50-Days-of-JavaScript
Solving interesting challenges to become a better developer 

### Table of Contents

| Day | Problem |
| --- | ------ |
| 1 | [Create a Counter Function](#create-a-counter-function) |

1. ### Create a Counter Function
 
 **Problem:** 
    Build a counter function creator. You are tasked with creating a function that takes an integer n as input and returns another function called a counter. This counter function should initially return the input n and then return 1 more than the previous value every subsequent time it is called (n, n + 1, n + 2, etc).

**Solution:**

```
export function createCounter(n) {
	return () => n++
}

```
Sample Test Cases

```

const counter = createCounter(5)
console.log(counter()) // Output: 5
console.log(counter()) // Output: 6
console.log(counter()) // Output: 7

const secondCounter = createCounter(-3)
console.log(secondCounter()) // Output: -3
console.log(secondCounter()) // Output: -2
console.log(secondCounter()) // Output: -1

const thirdCounter = createCounter(42)
console.log(thirdCounter()) // 42
console.log(thirdCounter()) // 43

```

**[⬆ Back to Top](#table-of-contents)**

