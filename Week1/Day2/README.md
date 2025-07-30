# Week1 - Day 2

# Problems
## Problem 1
### Code
```
   a, b, c
   Set a=2 b=6 c=8
   a=(10+9)+c
   if((c+b)>(a-c))
        a=b+c
        b=b+b
    End if
    Print a+b+c
```
### Solution : 
**41**
### Explaination :
a = 10 + 9 + 8 = 27, then condition 14(c+b) > 19(a-c) will become false, hence if block will not run.
a+b+c -> 27+6+8=41

## Problem 2
### Code
```
    Integer funn(Integer a, Integer b, Integer c){
        b=7+a
        a=(a+c)+a
        b=(b+b)+c
        c=1+b
        return a+b+c
    }
```
*Output if a=0 b=2 and c=10*
### Solution : 
**59**
### Explaination :
Initial values will be updated as per the order of statements. Like in Line (statement) no. 3: variable ‘b’ will be updated with a value of (7+a) which means 7+0=7. Then, in line 4, variable ‘a’ will be updated with value (a+c)+a which is (0+10)+0=10. Now, in line 5 ‘b’ will be reupdated with (b+b)+c. Keep remember “Precedence of Operators” while assigning the values in ‘b’. First it will execute parenthesis () and will retrieve the current value of b which has updated from line 3 then it will add with value of ‘c’. After execution of line 5 variable ‘b’ will be updated with value (7+7)+10=24. Then, in line 6, the value of variable ‘c’ will be updated with 1+b. Last value of b is 24 so
variable ‘c’ will be updated with 1+24=25. Now, from line 7 updated values of variable a, b and c will be added together and return from the function. So the final (return) value will be a+b+c => 10+24+25=59.


## Problem 1
### Code
```
   Integer pp, qq, rr
   Set 
   a=(10+9)+c
   if((c+b)>(a-c))
        a=b+c
        b=b+b
    End if
    Print a+b+c
```
### Solution : 
**41**
### Explaination :
a = 10 + 9 + 8 = 27, then condition 14(c+b) > 19(a-c) will become false, hence if block will not run.

a+b+c -> 27+6+8=41