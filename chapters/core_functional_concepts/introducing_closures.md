## Introducing Closures

You can think of closures as little bubbles of memory. While the bubble exists, the memory is encapsulated along with the proc or lambda. For now you can ignore Procs completely and we will focus on lambdas.

Essentially a Lambda is a special type of Ruby function. It is a function + a memory context. This means that whatever you pass into your lambda as arguments, that memory will be contained in the closure until you `call` the lambda, in which case the operation will happen and the lambda will return back to where it was called.
