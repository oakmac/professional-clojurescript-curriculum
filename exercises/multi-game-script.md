# Multi-game CLI Script

## Learning Objectives

- Compile a ClojureScript project to a Node.js script
- Parse command line arguments
- Split code using namespaces
- Use conditionals and simple logic

## Exercise

Your task is to write a CLI script that can play multiple games.

Let's use what we have learned so far. Be sure to separate your code into different namespaces.

#### Game 1 - Even or Odd?

The classic game of "even or odd" played by children and adults worldwide. The
user inputs a number and your program should print whether the number is "even"
or "odd". I spent hours playing this game as a youth.

```sh
$ node app.js even-or-odd 54
> even

$ node app.js even-or-odd 1
> odd

$ node app.js even-or-odd -4
> even

$ node app.js even-or-odd 5
> odd

$ node app.js even-or-odd 2
> even
```

#### Game 2 - FizzBuzz

Another classic game beloved by millions around the globe. The user inputs a
number and your program should print:

- If the number is divisible by 3: `Fizz`
- If the number is divisible by 5: `Buzz`
- If the number is divisible by both 3 and 5: `FizzBuzz`
- Otherwise, print the number itself

```sh
$ node app.js fizzbuzz 1
> 1

$ node app.js fizzbuzz 6
> Fizz

$ node app.js fizzbuzz 10
> Buzz

$ node app.js fizzbuzz 15
> FizzBuzz

$ node app.js fizzbuzz 20
> Buzz

$ node app.js fizzbuzz 29
> 29

$ node app.js fizzbuzz 12
> Fizz

$ node app.js fizzbuzz 30
> FizzBuzz
```


#### Game 3 - Rock, Paper, Scissors

#### Game 4 - Calculator

#### Game 5 - Tic Tac Toe

#### Game 6 (bonus) - Go Engine

Write


Examples:

```sh
$ node app.js fizzbuzz 54
>
```
