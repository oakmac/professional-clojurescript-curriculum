# Lesson 1050 - Namespaces and Require

## Learning Objectives

- Understand what a ClojureScript namespace is.
- Understand the relationship between namespaces and folders / files.
- Understand that namespaces map 1-to-1 with Google Closure modules after compilation.
- Understand how to uniquely name namespaces (reverse URL scheme).
- Understand that namespaces can depend on other namespaces.
- Understand that namespaces requires cannot resolve in a circular dependency.
- Understand that `core` is the "root" namespace by convention.
- Understand what it means to require a namespace into another namespace
- Understand what it means to use `:as` in a `require` statement.

## Lecture

- namespaces are a central, important part of a CLJS program
- all code is written inside a namespace
  - there is no "global scope" for code in ClojureScript
  - even at the REPL, you are in `cljs.user` by default
- one file, one namespace
  - `foo.bar.biz` --> `src-cljs/foo/bar/biz.cljs`
  - `banana-corp.website.core` --> `src-cljs/banana_corp/website/core.cljs`
  - these examples assuming your source path is `src-cljs/`
- hyphens in a namespace translate to underscores in folders and files
  - this is a limitation of the JVM classpath
- the "name" of a namespace is it's location
  - all ClojureScript namespaces should be globally unique
  - prefix all projects with a unique root base
  - "reverse URL" is recommended
  - it is common to use your name or company name
- namespaces can depend on each other via the `:require` form
  - all of the namespaces for a project form a tree
  - by convention, the `*.core` namespace should be at the top of that tree
- namespaces **cannot** have a circular dependency
  - the compiler will refuse to compile a project with circular dependency
  - this is a huge positive which forces you to organize your code cleanly
  - no namespace should `:require` the "core" namespace
- Nuanced, but important point: namespaces are how you **organize code** in a CLJS project,
  but they are only concerned with the code's **location**, not it's **function**.
  - In other words, namespaces do not define the architecture of your program.
  - Counter example: in Node.js it is common to "include all `\*.js` modules from a folder" at runtime.
  - You cannot do this in ClojureScript. You must use `:require` and build the namespace tree for the compiler.
- Namespace size
  - **most** namespaces should be less than 200 lines of code
  - in general, namespaces should not exceed 1,000 lines of code
  - there will be exceptions, but these are usually good guidelines

## Demo

- multiple source paths
- `:require`
  - `:as`
  - `:refer`

## Exercise

- [Red Squirrel Project](../exercises/red-squirrel-namespaces.md)

## References

- [Namespaces and Program Structure](https://www.learn-clojurescript.com/section-4/lesson-23-namespaces-and-program-structure/)
- [deep dive on the ns form](https://clojurescript.org/guides/ns-forms)
