# Phase 1 Project Requirements

This is the final project for "Phase 1" of [Professional ClojureScript] course.

[Professional ClojureScript]:https://cljs.pro

## Context

By now we know the basics of the ClojureScript language: syntax, namespaces,
data structures, sequences, atoms, and have some exposure to the core library.

We are also familiar with the mechanics of a ClojureScript project: using
shadow-cljs, folder / file project structure, compilation modes, connecting a
REPL.

## Project Description

Your task is to build a fun web application using ClojureScript and use what we
have learned so far!

You may work solo or as a team - up to you! If you decide to work with a group,
please consider that you will have to coordinate development efforts.

We will spend approximately two weeks of class time for this project. Roughly 20
hours, plus whatever additional time you spend outside of core class hours.

## Technical Requirements

These are the target learning objectives for this project. Consider these **must have**:

- Build a ClojureScript application that targets the web browser

- The application should be interactive
  - Example: a user clicks on a page element and the DOM changes as a result

- You should manage the state of the application using a ClojureScript atom(s).

- Your project should make use of ClojureScript sequences in some way.
  - This is a purposefully open-ended requirement since almost anything can be represented as a sequence
  - Can you think of a problem where something in the ClojureScript core library offers an elegant solution?

- Your project should represent HTML using ClojureScript data structures (not strings)
  - [hiccup] is the de-facto way to represent HTML in Clojure-land
  - look at the [hiccups] library for ClojureScript

- In addition to hiccups, you must use at least one external library in your application
  - This can be either from [clojars] or the [npm] ecosystem
  - Requiring and using libraries is an important part of application development

- Your project should contain **at least** three namespaces.
  - Separating code into namespaces is an important part of ClojureScript programs
  - Do not put everything in one large file

- Your project should be at least 200 lines of ClojureScript code.
  - We are looking for something more complex than "Hello, world" here :wink:

[hiccup]:https://github.com/weavejester/hiccup
[hiccups]:https://github.com/macchiato-framework/hiccups
[clojars]:https://clojars.org/
[npm]:https://www.npmjs.com/

## Project Recommendations

These are additional suggestions for your project. You do not have to fulfill
all of these as requirements, but hopefully they give you a nudge in the right
direction and spur some ideas!

- Recommend using a CSS framework for easy visual design
  - The purpose of this project is to practice ClojureScript, not visual design.
  - You are free to do custom visual design if you want! It's just not the intention of this project.
  - CSS framework examples:
    - [Bootstrap](http://getbootstrap.com/)
    - [Bulma](https://bulma.io/)
    - [Foundation](https://foundation.zurb.com/)

- Creating a small game is a great project idea
  - Games are interactive and stateful
  - Games have internal logic that can be represented using a sequence
  - Think "Connect Four", not "World of Warcraft"

- Consider using a public API + AJAX requests for some interesting mashups
  - [Big List of Public APIs](https://github.com/toddmotto/public-apis)
  - [Another Big List of Public APIs](https://github.com/abhishekbanthia/Public-APIs)

- Include a `README.md` file with your project to help your portfolio
  - Explanation of what the project is, what it does
  - Technologies used
  - Program architecture and approach
  - Include what you learned from this project. What was easy? What was difficult?
  - If you had more time, what else would you add? Anything you would do differently?

- Deploy your project somewhere publicly accessible
  - It's nice to be able to send someone a link to your work instead of "clone this repo and run locally"
  - [GitHub pages] is easy
  - [NeoCities] is fun
  - Many options here

- Be careful of project scope: pick a small target
  - Scope is the killer of software projects
  - We have a fixed amount of time to work on this, so this project will need to end
  - Better to pick something small and reach your target than "not finish"
  - If you pick too small and have more time, just polish and add features
    - It is easy to add scope from a place of completion
  - A small, fun idea that meets the requirements is better than a complex idea that you don't finish

- Separate your "app logic" from "rendering logic"
  - Think about the Tic-Tac-Toe example from the Multi-Game exercise
  - You can use `(assert)` as a light-weight testing tool to test your application logic

[GitHub pages]:https://pages.github.com/
[NeoCities]:https://neocities.org/

## Example Projects

These are some example projects that would fit the requirements. You may use
these ideas if you want, or riff on them with your own flavor.

If you are unsure of your project idea or need ideas please ask the class and we
will help brainstorm something together.

#### Whac-A-Something

Like the classic [Whac-A-Mole] game, except you pick a funny category of things to whack.

Maybe "Whac-A-Politician" or "Whac-A-Comic-Book-Character". Look for category
ideas by browsing the list of [Public APIs](https://github.com/toddmotto/public-apis).

Maybe you keep score in an interesting way depending on what the user clicks on.

[Whac-A-Mole]:https://en.wikipedia.org/wiki/Whac-A-Mole

#### Battleship

You could implement a version of [Battleship] and have players take turns
sitting at the computer / phone for their move.

[Battleship]:https://en.wikipedia.org/wiki/Battleship_(game)

#### Jeopardy

Create a trivia game that mimics the Jeopardy board using questions from the [Trivia API].

[Trivia API]:https://opentdb.com/api_config.php

## Learning Objectives

- Write a ClojureScript project from scratch
- Write ~200 lines of code
- Manage UI state using an atom
- Represent HTML data as hiccup
- Use a third-party library from Clojars or the JavaScript ecosystem (ie: npm)
- Use ClojureScript sequences and the core library
