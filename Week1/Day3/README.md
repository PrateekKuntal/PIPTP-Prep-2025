# Week1 - Day 4

# Problems
## Problem 1

```java
public static int f(int n) {
    if (n == 0) return 0;
    return n + f(n - 1);
}

System.out.println(f(5));
```

*What will be the output?*
- A) 15
- B) 10  
- C) 5
- D) 25

### Solution

**Answer: A) 15**

### Step-by-Step Analysis:

1. **Base Case**: When `n == 0`, the function returns 0
2. **Recursive Case**: For any positive n, the function returns `n + f(n-1)`
3. This creates a chain of recursive calls until it reaches the base case

### Explaination :
1st call: foo(5)=> **Recursive Case**, return 5 + f(4).

2nd call: foo(4)=> **Recursive Case**, return 4 + f(3).

3rd call: foo(3)=> **Recursive Case**, return 3 + f(2).

4rd call: foo(2)=> **Recursive Case**, return 2 + f(1).

5th call: foo(1)=> **Recursive Case**, return 1 + f(0).

6th call: foo(0)=> **Base case**,return 0.

Back To 5th call: as foo(0)=0, **return** 1 + 0 = *1*. 

Back To 4th call: as foo(1)=0, **return** 2 + 1 = *3*. 

Back To 3rd call: as foo(2)=3, **return** 3 + 3 = *6*.

Back To 2nd call: as foo(3)=6, **return** 4 + 6 = *10*. 

Back To 1st call: as foo(4)=10, **return** 5 + 10 = *15*. 


## Problem 2

```java
public static int foo(int n) {
    if (n == 1) return 1;
    if (n % 2 == 0) return 2 * foo(n / 2);
    return 2 * foo((n - 1) / 2) + 1;
}

System.out.println(foo(5));
```

*What will be the output?*

### Solution

**Answer: 5**

### Step-by-Step Analysis:
1. **Base Case**: If `n == 1`, return 1
2. **Even Case**: If n is even, return `2 * foo(n/2)`
3. **Odd Case**: If n is odd, return `2 * foo((n-1)/2) + 1`

### Explaination :
1st call: foo(5)=> **Odd Case**, as 5 is Odd, return (2* foo(2))+1.

2nd call: foo(2)=> **Even case**, as 2 is even, return 2 * foo(1).

3rd call: foo(1)=> **Base case**, **return** *1*.

Back To 2nd call: as foo(1)=1, **return** 2*1= *2*. 

Back To 1st call: as foo(2)=2, **return** (2*2)+1= *5*. 
