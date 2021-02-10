# Lesson 1020 - Simple Types: Strings, Numbers, Keywords

## Learning Objectives

- Understand what Strings, Numbers, and Keywords are in ClojureScript.

## Lecture

- Many ClojureScript simple types map 1-to-1 to JavaScript types

- ClojureScript Strings are JavaScript Strings
  - Strings are always wrapped with double quotes `"abc"`
  - Strings can be multi-line with no escape sequence
  - Strings in JavaScript are immutable
    - this allows for fast comparison
    - JS engines are well-tuned for Strings; use them
  - JavaScript does not have chars; only Strings
  - `clojure.string` has many useful functions to operate on Strings

- ClojureScript Numbers are JavaScript Numbers
  - IEEE 754 Double Precision floating point
  - there can be some strangeness when doing math with these (floating)
    - floating-point errors
    - do not use JS numbers to manage a bank account
    - operations on Integers can be trusted

- ClojureScript Functions are JavaScript Functions

- Keywords

```clj
;; Keywords are kind of like Strings, but mainly used as static identifiers
:foo
:bar-biz
:AAA_BBB_CCC
:logged-in?

;; You can create a Keyword from a String
(assert (= :foo (keyword "foo")))

;; Keywords can be namespaced:
:my-app.fruits/apple
::apple ;; <-- the double-colon will use the current namespace

;; Keywords are most often used in the context of Maps as keys
(def some-point {:x 10, :y 12})

(def user-from-the-db
  {:user/id 33781
   :user/name "John Doe"
   :user/username "john_doe_45"
   :user/email "johnd@example.org"
   :user/createdAt "2016-10-30 08:12:34"})

(def course-instructor
  {:fname "Chris"
   :lname "Oakman"
   :cool-factor 1000000})

;; Keywords can be used like a function to extract a value out of a Map
(assert (= 33781 (:user/id user-from-the-db)))
(assert (= "Chris" (:fname course-instructor)))

;; Under the hood, Keywords implement the IFn protocol, which we will learn about in a later lesson.
```

## Exercise

- [cljs101](https://github.com/oakmac/cljs101)
- https://github.com/opqdonut/clojure-exercises
