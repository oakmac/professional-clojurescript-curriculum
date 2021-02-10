# Lesson 1022 - Functions, Anonymous or not

## Learning Objectives

- Understand the three different ways to write a function in ClojureScript
- Understand the difference between `(fn [])` and `#()`
- Understand how function arity works in ClojureScript
- Understand what `:pre` and `:post` can do

## Lecture

- ClojureScript Functions are JavaScript Functions

- `defn` is the primary way to write functions in ClojureScript
  - top-level form
  - creates a symbol that you can reference elsewhere

- Anonymous Function syntax #1: `(fn [])`

```clj
;; this is an Anonymous function:
(fn [a b]
  (+ a b))

(let [my-fn1 (fn [x] (str x "-" x))
      my-fn2 (fn [] nil)]
  (assert (= "aaa-aaa" (my-fn1 "aaa")))
  (assert (nil? (my-fn2))))

(my-fn2) ;; <-- compiler error - it does not recognize "my-fn2" in this scope
```

- Anonymous Function syntax #2: `#()`
  - Shorthand for creating anonymous functions
  - Nested `#()`s are not allowed
  - Should be very short
  - Best if they are one or two arity

- the JavaScript runtime does not enforce function arity
  - Arity is the number of arguments to a function
  - the ClojureScript compiler will yell at you for wrong arity (warning)
    - but ultimately the JS runtime does not care
  - [ClojureScript Function Arity Example](supplementary/1022-arity-example.md)

- TODO: `:pre` and `:post` conditions

## Exercise

- Write some of these
