# Lesson 11 - Making Decisions

# Exercise: If Statement Practice

Come to grips with the if statement by rewriting the following comments in code form.

```swift
let a = 20
let b = 30
let c = 20

// If a is equal to c, print "a and c are the same"
if a == c {
    print("a and c are the same")
}


// If a is less than b, print "b is ahead of a"
if a < b {
    print("b is ahead of a")
}


// If b is greater than a, print "a is not winning against b"
if b > a {
    print("a is not winning against b")
}


// If a is less than or equal to c, print "a is either losing to or tied with c"
if a <= c {
    print("a is either losing to or tied with c")
}
```

## Exercise
Add code after each comment above to follow the instructions. (For the greater than and less than operators, remember the rule about the hungry mouth.)

# Exercise: Else Practice

You’ll recall that else statements hold code that’s run when the result of an if statement is not true. They can reduce the amount of code needed, and they make it clearer what the flow of a program should be.

```swift
let secretWord = "banana"
let guess = "apple"

if secretWord == guess {
    print("Your guess is right.")
} else {
    print("Your guess is wrong.")
}
```

## Exercise
Rewrite the code above to use an else statement.

# Exercise: Leap Years

To decide if a year is a leap year, there are several decisions that have to be made:

* Is the year divisible by 4?
*If so, is the year divisible by 100?
*If not, it is a leap year.
*If so, is the year divisible by 400?
*If not, it is not a leap year.
*If so, it is a leap year.

These decisions can be made inside a function.

The number(_:, isDivisibleBy:) function has been built into this playground to make this exercise easier. Below is an incomplete function for deciding if a given year is a leap year:

```swift
func isLeapYear(_ year: Int) -> Bool {
    if number(year, isDivisibleBy: 4) {
        if !number(year, isDivisibleBy: 100) {
            return true
        }
        if number(year, isDivisibleBy: 400) {
            return true
        }
    }
    return false
}
// Should be true
isLeapYear(2000)
// Should be false
isLeapYear(1900)
// Should be true
isLeapYear(2012)
// Should be false
isLeapYear(2017)
```

## Exercise
Complete the function above so that the rules are all followed and the examples get the correct answers.

