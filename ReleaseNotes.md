# Release Notes

# 0.1.0

ClojureScript at 5d4b407e2ea391bd63b873541e6a0fbb67de400b

With patch for http://dev.clojure.org/jira/browse/CLJS-72

- Extend goog-dependencies* to match double-quotes on first argument

  When using a closure compiler generated goog/deps.clj, goog-dependencies* fails
  to parse anything from the file.  This is due to the compiler writing the
  dependencies using double quotes for the first argument to  addDepenendency.
