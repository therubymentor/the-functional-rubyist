## Is Ruby a Functional Programming Language?

Ruby is _almost_ a functional language. You can write a lot of purely functional code in it, but the downside is that the language was built with side-effects and mutations in mind. So writing purely functional code will get you a lot more mileage in something like Haskell or Clojure, those languages are not very good for newer programmers, or for that matter, as a tool to teach functional programming.

### So why write Funcional Ruby at all?

We write so called functional code to make _our own lives_ easier. Because the program doesn't actually change state while it runs, it is much easier to debug. You can simply focus on the inputs and outputs of a specific function without looking at the state of the program as a whole.

If the functions you are trying to reason about don't rely on variables whos scopes can change outside your function, you can learn everything you need to know about the behavoir at hand, because it is all isolated to the specific location where the behavior happens.

Side effecting code, or "stateful code" as I will call it from now on, on the other hand has operations and changes ocurring from far away from the locality of the code we are debugging. Whenever that is the case, instead of just looking at the function in front of you, you have to consider the _program state_ as a whole, along with the function you want to debug.


