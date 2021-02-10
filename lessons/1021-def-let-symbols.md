# Lesson 1021 - Def Forms, let blocks, Symbols

## Learning Objectives

- Understand `def`, `defn`, `defn-`
- Understand `let` blocks
- Understand what a Symbol is, and how they are scoped

## Lecture

- def forms

```clj
;; use "def" to define things
(def my-name "Chris")

(def cool-factor 1000000)

(def a "a")

;; use "defn" to define a function
(defn add-seven-to-x [x]
  (+ x 7))

(defn hello-world [name]
  (str "Hello, " name "!"))

;; "defn-" means "private to this namespace"
;; otherwise it is exactly the same as "defn"
(defn- my-secret-fn []
  nil)

;; Here is how to create a private "def"
(def ^:private my-secret-value1 :value)
(def ^{:private true} my-secret-value2 :value)

;; Note that "private" is not enforced by ClojureScript (it is with JVM Clojure)

;; TODO: add docstring here
```

- `let` blocks

```clj
;; let blocks are how you define symbols for a scope
;; you can think of them like "let" or "const" in JavaScript
;; Note that let blocks should always have an even number of forms inside of them:
;; symbol --> value, symbol --> value, symbol --> value, etc
(let [my-first-name "Chris"
      my-last-name "Oakman"
      cool-factor 1000000
      number-of-toes (+ 5 5)]

  ;; Inside here, I can use all of these symbols just like any "def" or "defn"
  (println (str my-first-name " " my-last-name " has a cool factor of " cool-factor))

  ) ;; <-- the end of this "let" block

(let [a "a", b "b", c "c"]
  (assert (= "abc" (str a b c))))

(println b) ;; <-- compiler error - it does not recognize b in this scope
```

- Symbols
  - just a name that represents something
  - Symbols are like identifiers in JavaScript or C
  - Symbols in CLJS have no relationship to [JavaScript Symbols]

[JavaScript Symbols]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol

## Exercise

- Write some of these
