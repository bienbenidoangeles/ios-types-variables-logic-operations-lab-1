# Types Variables Logic and Operations Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit

## 1. Which of the following variables/constants are declared correctly?  Select all that apply.

```swift
a. let nameOfPrincipal: Character = "Mrs. Watkins"

b. var temperatureOutside: Int = 90.7

c. var isSummer: String = false

d. let whiteHouseAddress: Int + String = 1600 + "Pennsylvania Ave"

e. var peopleAtParty: Double = "95"
```

Choice d

***
## 2. Which of the following expressions evaluate to true?

```swift
a. !(4 + 3 < 2 * 4)
    f
b. !(1 + 1 != 2) && !(3 >= 3)
    f
c. (3 < 2 || (0 < 1 && 3 >= 3)) && true
    t
d. !!(!!true && !!false)
    f
e. true && (true && (true && (true || false)))
    t
```

Choices c and d

***

## 3. You are given two variables a and b, compute their sum and store it in another variable named sum then print the result.

```swift

Example 1
Input:
var a = 1
var b = 2

Expected values:
sum = 3

Output: 
3

Example 2
Input:
var a = 13
var b = 22

Expected values: 
sum = 35

Output:
35
```
In example 1: include the following code under line 55:
```swift
var sum = a + b 
print(sum)
```

In example 2: include the following code under line 66:
```swift
var sum1 = a +b
print(sum)
```
***
## 4.Determine the number of seconds in a year and store the number in a variable named secondsInAYear.

```swift
Hint:
The number of seconds in a year is 365 times the number of seconds in a day.
The number of seconds in a day is 24 times the number of seconds in a hour.
The number of seconds in a hour is 60 times the number of seconds in a minute, which is 60.
```
```swift
var secMin = 60
var secHour = 60 * secMin 
var secDay = secHour * 24
var secondsInAYear =  365 * secDay
```

***
## 5. Your are given the width and height of a screen in pixels. Calculate the total number of pixels on the screen and store the result in a variable named numberOfPixels.

```swift
var width = 1920 
var height = 1080

Example 1
Input: 
var width = 4
var height = 3

Expected values:
numberOfPixels = 12

Example 2
Input:
var width = 1920
var height = 1080

Expected values:
numberOfPixels = 2073600

Hint:
Consider a 5x3 screen like this:
*****
*****
*****

The number of pixels on this screen is 5+5+5 = 5*3
```

In example 1, include the following code under line 107:
```swift
var numberOfPixels = width * height
```
In example 2, include the following code under line 115:
```swift
var numberOfPixels = width * height
```
***
## 6. You are given the sum and the difference of two numbers. Find out the values of the original numbers and store them in variables a and b.

```swift
let sum = 16 // a + b 
let diff = 4 // a - b

Example 1
Input: 
var sum = 16 
var dif = 4

Expected values:
a = 10
b = 6

Example 2
Input:
var sum = 2 
var dif = 0

Expected values:
a = 1
b = 1

Hint:
sum + diff = a + a + b - b
sum + diff = 2 * a
```

In examples 1 and 2 include the following code under lines 140 and 154 respectively:
```swift
var a = (sum+dif) /2
var b = sum - a
```

***
## 7. Given two variable a and b, swap their values. That is the new value of a will become the old value of b and vice versa.

```swift
var a = 1
var b = 2

Example 1
Input: 
a = 2
b = 1

Hint:
Just assigning a to the value of b and b to the value of a will not work.

var a = 1
var b = 2

a = b // a will have the value 2. The original value of a is lost
b = a // b will remain the same
```
```swift
var c = a
var a = b
var b = c
```

***
## 8. You are given a number a. Print the last digit of a.

```swift
var a = 123

Example 1
Input: 
var a = 123

Output:
3

Example 2
Input: 
var a = 337

Output:
7

Hint:
Use the remainder % operator.
Remember that a = k * (a / k) + a % k
Can you think of a value for k that gives the last digit?

```
In examples 1 and 2, insert the following code under lines 202 and 209 respectively:
```swift
var remainder = a % 10
print(remainder)
```
***
## 9. You are given Rocky’s age in dog years. Print Rocky’s age in human years. You know that 1 human year is 7 dog years.

```swift

Example 1
Input: 
var rockysAge = 50

Output:
7

```
In example 1, insert the following code under line 231:
```swift
var rockyHumAge = rockysAge / 7
print(rockyHumAge)
```

***
## 10. Everyone hates solving word problems by hand so let’s make a program to solve them for us. 
### x years from now Alice will be y times older than her brother Bob. Bob is 12 years old. How many years does Alice have?

```swift
var x = 3
var y = 2
var bob = 12

var alice = ?

Example 1
Input: 
var x = 3
var y = 2
var bob = 12

Expected values: 
alice = 27

Example 2
Input: 
var x = 1
var y = 3
var bob = 12

Expected values: 
alice = 38

Hint:
alice + x = y * (bob + x)
Solve for alice

```
For examples 1 and 2, include the following code below lines 256 and 265 respectively:
```swift
var alice = ((bob + x) * y) - x
```
***
## 11. You have x apples. Bob trades 3 oranges for 5 apples. He does not accept trades with cut fruit. How many oranges can you get from Bob and how many apples will you have left? The number of apples you will have left should be stored in a variable named apples. The number of oranges you will have after the trade should be stored in a variable named oranges.

```swift
var x = 17

Example 1
Input: 
var x = 17

Expected values: 
apples = 2
oranges = 9

Example 2
Input: 
var x = 25

Expected values: 
apples = 0
oranges = 15

Hint:
Use the division(/) and the remainder(%) operator

```
For examples 1 and 2, include the following code below lines 286 and 294 respectively: 
```swift
apples = x % 5
oranges = ((x - apples) / 5) * 3
```
***
## 12. A class consists of numberOfBoys boys and numberOfGirls girls.
### Print the percentage of boys in the class followed by the percentage of girls in the class. The percentage should be printed rounded down to the nearest integer. For example 33.333333333333 will be printed as 33.

```swift
var numberOfBoys = 20
var numberOfGirls = 60

Example 1
Input: 
var numberOfBoys = 20  
var numberOfGirls = 60

Output:
25 // percentage of boys
75 // percentage of girls

```

For example 1, include the following code below line 314:
```swift
var numberOfBoysDouble = Double(numberOfBoys)
var numberOfGirlsDouble = Double(numberOfGirls)
var sum = Double (numberOfBoysDouble + numberOfGirlsDouble)
let perBoy = floor( Double (numberOfBoysDouble / sum) * 100)
let perGirl = floor( Double (numberOfGirlsDouble / sum) * 100)
print(perBoy)
print(perGirl)
```

***
## 13.Which of the following expressions evaluate to true?

```swift
a. false || true
b. false && true
c. !false
d. !!!true
e. !(true && true)

```
Choices a and c

***
## 14.Which of the following expressions evaluate to true?

```swift
a. 3 < 12.3
b. 9 == 2
c. "Hello!" == "Hello!"
d. 19.0 >= 19.0
e. 9 > 7 && 7 < 10

```
Choice c, d and e
