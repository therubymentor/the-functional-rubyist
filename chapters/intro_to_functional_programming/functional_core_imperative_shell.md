## Functional Core - Imperative Shell

Ruby is almost an entirely Object Oriented language built on top of some Functional core concepts. It is a dirty mix of the two as a friend of mine once put it. While this prevents you from writing the kind of "pure functional code" you would write in Haskell or Clojure, we use a paradigm called, Functional Core - Imperative Shell.

This concept was first introduced to me by Gary Bernhardt, a polyglot who once has gave the Ruby community some really great ideas (before he left our ranks for greener grasses). The concept breaks down like so:

Since a program that changes *no* state isn't much more useful than a calculator, we acknowledge that our program will change *some* state. But we will keep the vast majority of our functions pure.

> A pure function is a method that takes arguments and does some calculation, then returns a new value. It does not alter any program state *outside* itself.

If your function simply takes arguments and returns values, it not only becomes a lot easier to rationalize, it brings it a lot closer to being able to run on multiple cores without creating a disaster.

This is because if the functions don't change any state around them, they can essentially be offloaded to different processors and
