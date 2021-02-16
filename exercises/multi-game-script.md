# Multi-game CLI Script

## Learning Objectives

- Compile a ClojureScript project to a Node.js script
- Parse command line arguments
- Split code using namespaces
- Use conditionals and write simple logic

## Exercise

Let's use what we have learned so far to write a CLI script that can play multiple games.

- I recommend doing the games in order starting with \#1, then \#2, etc
- Be sure to separate your code logically using namespaces
- Don't forget to commit or save your work often!

#### Game 1 - Even or Odd?

The classic game of "even or odd" played by children and adults worldwide. The
user inputs a number and your program should print whether the number is "even"
or "odd". I spent countless hours playing this game as a youth.

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

Rock, Paper, Scissors is a lesser-known game from the remote mountain towns of Olympus Mons.

It is played with two players who each throw their hand as either: rock, paper, or scissors

- Rock beats Scissors, but loses to Paper
- Paper beats Rock, but loses to Scissors
- Scissors beats Paper, but loses to Rock
- The game results in a Tie if both players throw the same object

Your program should accept two arguments (one for each player) and return the winner.

```sh
$ node app.js rps rock paper
> Player 2 wins! Paper covers Rock

$ node app.js rps rock rock
> Tie! Both players threw Rock

$ node app.js rps Scissors Rock
> Player 2 wins! Rock smashes Scissors

$ node app.js rps scissors Paper
> Player 1 wins! Scissors cuts Paper

$ node app.js rps Scissors scissoRs
> Tie! Both players threw Scissors
```

#### Game 4 - Calculator for Julian

Julian loves playing with his favorite abacus. Unfortunately, a seagull stole it
when he was at the beach the other day! Apparently the seagull thought it was "mine!".

Can you help build a calculator for Julian to replace his beloved abacus?

> NOTE: Julian only needs to pass one, two, or three numbers to the calculator. More than that would just be crazy!

```sh
$ node app.js calc add 2 3
> 5

$ node app.js calc add 1
> 1

$ node app.js calc add 6 2 3
> 11

$ node app.js calc subtract 6 2
> 4

$ node app.js calc subtract 2 5
> -3

$ node app.js calc subtract 82
> 82

$ node app.js calc multiply 2 5
> 10

$ node app.js calc multiply 2 5 60
> 600

$ node app.js calc multiply -2 6
> -12

$ node app.js calc multiply 9
> 0

$ node app.js calc divide 9 3
> 3

$ node app.js calc divide 8 2
> 4

$ node app.js calc divide 0 24
> 0
```

> Note for Math nerds: do not worry about edge cases for this exercise. Focus on getting the basics working.

#### Game 5 - Tic Tac Toe

Sally loves playing Tic Tac Toe with her little brother James. The only problem
they run into is determining when the game is over.

Can you build a program to help Sally and James know when their game is over?

```sh
$ node app.js ttt ooo,xnx,nxn
> O wins!

$ node app.js ttt oxo,oxn,nxn
> X wins!

$ node app.js ttt oxo,oon,nxx
> No winner yet. Play on!

$ node app.js ttt xoo,oxx,xxo
> Game over: draw
```

#### Game 6 (bonus) - Go Engine

This one is a real challenge!

Write a program that can beat most 6 dan amateur human players at the classic game of [Go](https://en.wikipedia.org/wiki/Go_(game)).

Be sure to evaluate all possible future board states from the current position: leave no stone unturned!

If you need a hint on how to get started, there is one below encoded using [base64](https://www.base64decode.org/):

```txt
VGhpcyBpcyBub3QgYWN0dWFsbHkgcG9zc2libGUuIFBsZWFzZSBkbyBub3QgYXR0ZW1wdCB0aGlzIGV4ZXJjaXNlIPCfmII=
```
