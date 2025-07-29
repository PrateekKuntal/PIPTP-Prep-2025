# Week1 - Day 1
# Problems
## Problem 1
### Code
```
void fun(Integer w, Integer x){
     Integer y =0;
    if(x % w == 0 || w%x == 0){
        y = y+1;
    }else{
        y = y+10;
    }
    print(y);
}
fun(40, 4); 
```

### Solution :
**1**

### Explaination :
w % x == 0 is true. since 40 % 4 == 0. hence, y = y + 1 => 1

## Problem 2:
### Code

```
Integer a = 1;
while(a<5){
    a=a+2;
}
print(a);
```

_How many times loop will run?_
### Solution :
**2**

### Explaination :
1st : a = 1 + 2 = 3, now condintion is checked a < 5 -> true since a == 3. 

2nd : a = 3 + 2 = 5 now condition is checked, a < 5, since a == 5 -> loops terminates .

## Problem 3:

### Code
```
Integer funn(Integer a, Integer b){
    if(a && b && a+b > 0){
        return a + funn(a-2, b-2) + b;
    }
    return a ^ b
}
```
_Output of code when a=8 and b=8?_

### Solution :
**40**

### Explaination :
a=8 b=8 -> condition true -> 8 + 8 + funn(6, 6)

a=6 b=6 -> condition true -> 6 + 6 + funn(4, 4)

a=4 b=4 -> condition true -> 4 + 4 + funn(2, 2)

a=2 b=2 -> condition true -> 2 + 2 + funn(0, 0)

a=0 b=0 -> condition false -> returns 0 ^ 0 = 0

***Final answer =***  8 + 8 + 6 + 6 + 4 + 4 + 2 + 2 + 0 = ***40***

## Problem 4:
### code
```
Integer a, b
Set a = 3, b = 3
a = b
if(1^1){
    a=1
}else{
    b=2
}
print(a+b)
```

_What is the output of the pseudocode?_

### output :
**5**

### Explaination :
Since 1 ^ 1 = 0, then condition is false then else block is executed, that will make b = 2, then a + b => 3 + 2 = 5

## Problem 5:
### code
```
Integer funn(Integer a, Integer b){
    Integer c
    for(each c from 2 to 4){
        if(a mod 2 < b mod 3){
            a = 4 mod 3
        }else{
            if(5 mod 3 > b){
                a = b
            }
            b = 1
        }
    }
    return a + b
}
```
*What function will return for a=7 and b=5?*

### output :
**6**

### Explaination :
1st : a=7 b=5, now condintion is checked 7%2 < 5%3 -> true since 7%2 = 1 and 5%3 = 2, then a is set to, a = 4%3 = 1.

1st : a=7 b=5, now condintion is checked 7%2 < 5%3 -> true since 7%2 = 1 and 5%3 = 2, then a is set to, a = 4%3 = 1.