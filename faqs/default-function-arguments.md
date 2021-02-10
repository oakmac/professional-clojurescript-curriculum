# How do you provide default arguments to a function?

```clj
(def default-parse-something-options
  {:slap-corners? false
   :enumerate-foos? true
   :max-num-lines 15})

(defn parse-something
  ([a-string]
   (parse-something a-string default-parse-something-options))
  ([a-string opts]
   (let [opts (merge default-parse-something-options opts)]
     ;; do the logic of parsing here ...
     nil)))

;; Example usage:
(parse-something "some string to be parsed")
(parse-something "some string to be parsed" {:slap-corners? true})
```
