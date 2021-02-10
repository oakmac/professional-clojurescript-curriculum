# Lesson 1005 - Why ClojureScript?

## Learning Objectives

- Understand some of the main value propositions of Clojure / ClojureScript.
- Understand why ClojureScript was created.
- Understand the difference between simple and easy.
- Understand that Lisp languages have a long history and unique benefits.
- Get excited about learning this powerful technology!

## Lecture

- [Simple Made Easy](https://www.infoq.com/presentations/Simple-Made-Easy/)
  - [transcript](https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/SimpleMadeEasy.md)
  - [YouTube version](https://www.youtube.com/watch?v=oytL881p-nQ)
  - If you only watch one talk about Clojure I would recommend this one.
  - several important Clojure concepts are presented here:
  - distinction between things that are "easy" vs things that are "simple"
  - "construct" vs "artifact"
  - mental limits for complexity
  - "What's in your toolkit?" comparisons

- [Beating the Averages](http://www.paulgraham.com/avg.html)
  - classic essay on the unique power of Lisp as a programming language
  - The Blub Paradox is useful to think about when choosing languages for your programs and career

- [Are we there yet?](https://www.infoq.com/presentations/Are-We-There-Yet-Rich-Hickey/)
  - [transcript](https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/AreWeThereYet.md)
  - from 2009 (pre-dates ClojureScript)
  - Offers a critical look at existing paradigms in popular programming languages
  - In particular, the ideas behind Object Oriented Programming and how they map to the real world that we are trying to model in our programs
  - Introduces the concepts of Value, State, Identity, and Time
    - these are important Clojure ideas
  - Explains the benefits and trade-offs of Persistent Data Structures
  - A good introduction to may of the most important ideas behind Clojure

- [Rich Hickey announces ClojureScript](https://www.youtube.com/watch?v=tVooR-dF_Ag)
  - NYC Clojure Meetup in 2011
  - This was the first big "public introduction" to ClojureScript to the world
  - "Why are we doing this? Because Clojure rocks, and JavaScript reaches."
  - Great overview of Rich's thinking about the world of JavaScript and the role for ClojureScript in it
  - Note how much of the JavaScript world has changed since 2011, and how stable ClojureScript has remained through all of that change
  - Explains the choice and role of Google Closure tools for ClojureScript
  - Note: audio/video quality is not the best

- [ClojureScript for Skeptics](https://www.youtube.com/watch?v=gsffg5xxFQI)
  - covers lots of the reasons why you would want to choose ClojureScript
  - a good overview of the ClojureScript ecosystem from 2015
    - Note that some things have changed since then (notably: shadow-cljs)
  - Derek is really funny and a great speaker; enjoyable to watch
  - interesting to observe how much the JavaScript ecosystem has changed from that talk to today

- [Effective Programs - 10 Years of Clojure](https://www.youtube.com/watch?v=2V1FtfBDsLU)
  - [transcript](https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/EffectivePrograms.md)
  - Where does the complexity lie in our programs?
  - How does Clojure help with this?
  - Where does Clojure not help?

- [Spec-ulation](https://www.youtube.com/watch?v=oyLBGkS5ICk)
  - [transcript](https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/Spec_ulation.md)
  - Semantic versioning is a lie. Dependencies are hard.
  - Creating `api2` is better than changing `api1`

- CO Reasons
  - JavaScript is a core part of the "new web"
  - In a long haul, complexity kills software projects
    - this is where ClojureScript shines
  - JavaScript is not designed for complexity over time
  - JavaScript has a short-term culture
  - ClojureScript is a great long-term technology bet
    - There is a reason Lisp has survived for over 50 years (no other syntax has)
    - Macros mean that ClojureScript will always be able to "keep up" with changes

## Exercise

- Watch some (or all) of these and get excited about ClojureScript!
- https://medium.com/@lwhorton/why-clojure-script-e4a69cc5168a
