# Exercise: Simple Project using Reagent

[reagent] is a minimal ClojureScript wrapper around the [React] library.

Reagent is a great introduction to the mental mode of building a user interface
using reactive Components.

Your mission, should you choose to accept it, is to write Tic-Tac-Toe or Bear,
Ninja, Cowboy using reagent and reactive components.

## Important: please re-use code!

Hopefully by now you have already written one (or both) of these exercises. The
goal of this exercise is not to re-write the HTML and CSS and game logic, rather
to practice a new paradigm for building UIs.

In other words, we want to re-use our existing knowledge here and only change
"one variable" of the learning process.

## Learning Objectives

- learn Reagent and the reactive component paradigm
- build something that already exists, focus on the architecture / differences from other approaches

## For Tic-Tac-Toe

You may find [this url helpful](https://github.com/oakmac/clojurescript-tic-tac-toe/tree/lecture1).

## For Bear, Ninja, Cowboy

Consider Katie's Phase 1 project: [Bear, Ninja, Cowboy](https://github.com/oakmac/Bear-Ninja-Cowboy)

## For a Challenge

If you finish this exercise quickly, add the following feature as a bonus /
challenge: On the same page, add a button called "Add Game". When pressed, it
should append another instance of the game onto the page. The user should be
able to add N games onto the page as desired. Please ensure that each game
retains it's own state. How can you make your code re-usable so that this
functionality is easy to add?

If you finish this, add a "Remove Game" button for each instance of the game to
allow for it to be removed from the page.

[reagent]:http://reagent-project.github.io/
[React]:https://reactjs.org/
