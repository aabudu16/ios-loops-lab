# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**

var range = 1...150

for numbers in range {
print (numbers)
}

## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

var range = 142...159

for numbers in range {
print (numbers)
}

## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

var range = 15...80

for numbers in range {
print (numbers)
}

## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

var range = 19...51

for numbers in range {
if numbers % 2 != 0 {
print (numbers)
  }
}


## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

var range = 1..<100
var InitialNumber = 5

for _ in range{
while InitialNumber < 100 {
print (InitialNumber)
InitialNumber += 10
  }
}

## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

var range = 1...40
var InitialNumber = 7

for _ in range{
while InitialNumber < 40 {
print (InitialNumber)
InitialNumber += 10
}
}
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`


let range = 20...150

for numbersDivisibleBy2And3 in range where numbersDivisibleBy2And3 %  2 == 0 && numbersDivisibleBy2And3 %  3 == 0{
print(numbersDivisibleBy2And3)
}


## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

for numbersDivisibleBy2And3 in range where numbersDivisibleBy2And3 %  2 == 0 || numbersDivisibleBy2And3 %  3 == 0{
print(numbersDivisibleBy2And3)
}

## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

let range = 20...150
var initialValue = 4
let endValue = 150
for _ in range {
while initialValue < endValue {
print (initialValue)
initialValue += 10
}
}

## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

let range = 20...150

for value in range {
if value == 31 {
print (value)
}
if value == 35 {
print (value)
}
if value >= 40 && value <= 60 {
print (value)
}
}

## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// The loop will run infinitely because the condition will alway be true due to the fact that the (i) is already greater than (3) and will continue to be incremented by (1). the condition will always be true.
```

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
//Answer

var i = 5

while (i > 3) {
if i == 10{
continue
}
i += 1
}

// OR

var i = 5

while (i > 3){
print (i)
if i >= 9{
break
}
i += 1
}

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
//Answer

var i = 5

while (i > 3) {
if i == 1005{
break
}
i += 1
}

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
//Answer
var i = 5

while (i > 3){
if i % 2 == 0{
print (i)
}
if i >= 1005{
break
}
i += 1
}

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```
~ loop one checks thw condition first to see if it is TRUE before executing the block code.
~ loop two runs the block code once then check to see if the condio is true. 
~ YES both loop will have the same output

***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

~ break - Once a code is executed it will run, but once the it reaches (break), the code will stop.
~ continue - Once a code is executed it will run, but when it reaches (continue), the code will not execute any line below but instead start over from the top. 
***
## Question 17

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[√]1
[√]2
[√]3
[]4
[]5
[]6
[]7
[√]8
[√]9
[√]10

***
## Question 18

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[√]1
[√]2
[√]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

***
## Question 19

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
```
x = 1, y = 1
x = 2, y = 1
x = 3, y = 1

~ using (labels ":") when the code reaches the "continue", the label points to the outterloop to start from.
***
## Question 20

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

for x in 0...10{
for y in 0...10{
print ("\(x) , \(y)", terminator: " ")
}
}

## Question 21

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

for x in 0...10 {
for y in 0...10 where x - y >= 5 {
print ("(\(x) , \(y))", terminator: " ")
}
}


## Question 22

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```

var n = 5

for n in 1...n{
print (n * n)
}

## Question 23

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

var n = 3
for _ in 1...n {
for _  in 1...n {
print ("*" , terminator: "")
}
print()
}
