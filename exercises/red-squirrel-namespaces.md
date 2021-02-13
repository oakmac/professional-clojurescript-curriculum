# Exercise: design namespaces for the Acme Corp "Red Squirrel" project

## Problem

You work for Acme Corp and have been assigned to the greenfield (ie: all new
code) project dubbed "Red Squirrel". Acme Corp already uses ClojureScript and
you know that "Red Squirrel" will be using code from a shared namespace
elsewhere in the company.

In particular, you know that several namespaces from `acme-corp.shared.util.*`
will be used, as well as the `acme-corp.shared.critical-business-logic` namespace.

Before any code is written, you already know there will be a few major
subsystems for Red Squirrel that you plan to divide up among team members. These
subsystems are 1) eating nuts 2) jumping 3) being adorable and 4) the UI.

## Exercise Part 1 - Design the Namespaces

> PROTIP: do `git commit` after each exercise step!

Write down the namespaces you think may be needed for the Red Squirrel project.

Remember that there cannot be circular dependencies in namespaces.

## Exercise Part 2 - Create the Skeleton

Create the project skeleton for Red Squirrel.

Please do this "manually", by creating namespace files and folders and typing
things out. The goal here is not to practice typing, but practice an essential
ClojureScript skill.

The end result of this step should be a full ClojureScript project that can be compiled.

> Hint: follow the [shadow-cljs Quick Start](https://github.com/thheller/shadow-cljs#quick-start) to get up and running quickly!

## Exercise Part 3 - Initialize Subsystems

In the `acme-corp.red-squirrel.core/init!` function, initialize the following subsystems:

- eating nuts
- jumping
- being adorable
- the UI

The initialization function for each subsystem should print that it has been
started to the console (you can use `println`).

## Exercise Part 4 - Add UI Subsystems

The UI team needs to initialize the Routing and Rendering subsystems when the UI
is started. Create a namespace for each of these with an initialization function
and add them to the initialization function for the UI.

> Hint: this step should **not** modify the `acme-corp.red-squirrel.core` namespace at all.

## Exercise Part 5 - Requirements Change: New Subsystems

By now you are a month into the project and project Red Squirrel is coming along great!

Through the process of writing code the team has realized a few things:

- "eating nuts" is really a part of the "being adorable" system
- "looking cute" is also a necessary component of "being adorable"
- the system could really benefit from having a few background tasks that get started on system bootup

Make changes to the namespaces and initialization functions to reflect this new
understanding.
