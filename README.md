# The Functional Rubyist
#### By Jim OKelly

## Dedication

> This book is dedicated to my friend and mentor, Jim Weirich. Before him I was just a coder. Jim opened my eyes to the concept of design and I will forever be grateful.

When we lost Jim Weirich we lost not only a funny, respectful, genius, daring, and super kind Rubyist, I fell like we lost a bit of our soul.

This book is a direct result of the Quest dear Jim put me on when he showed me the concept of lazy evalutaion through lambdas and that Ruby was just another LISP, and that LISP was absolutely amazing for the brain.

I miss you big guy. I can only hope you would dig this book if you were still here a strummin your euk.

## Acknowledgements

First off, thank you Matz. Thank you for bringing us such a Frankenstein of a language. The sheer genious of giving us a programming language that truely takes the best ideas out there (at the time) and jamming them together.

Thank you Eiffel, LISP, and SmallTalk for giving Ruby it's best stuff.

Thank you Phil Cohen, who constantly challenged me to do better and to stick with shit. Thanks for all the chill out sessions where we just kicked it and talked.

You are an amazing curator of good ideas. An hour in your head is worth more than it's weight in gold. ;)

Thank you Gary Bernhardt for putting your thoughts together into Destroy All Software and for having paid attention to the stuff going on around you to be another amazing curator of people and ideas. Functional core, imperative shell saved my life.

Thank you Corey Haines for knowing Gary, and also knowing just about anyone worth knowing. Your involvement in XP led me onto J.B. Rainsberger and Kent Beck. I coded with you in India when you were a travelling pair programmer. I had never thought of creative constraints until then. Blew my mind.

Thank you Uncle Bob Martin, for hanging out with Rubyists at least for awhile. If I skipped everything you ever said about programming and just took the rest, my life with still be forever enriched. And you are right, What Killed SmallTalk could kill Ruby.

I have been deeply effected by a lot of things from inside and out of the Ruby community. As is the case in life, there were a few people who turned me on to better people. There is far more to list, but I have that post available online at blog.rubymentor.io so I won't take up more ink here to do so.

## Aims, Goals, and Promises

This book is not an answer to any question. It is not a bible for any solution. It is an exploration of trying to make code you love instead of code you hate. It might have more prenthesis than you were previously comfortable with, and at times it might not look like any Ruby you have ever seen before.

I don't even advocate you use anything found here anywhere. However, if you choose to do so, I think you will find that you can make a lot more sense of your code 2, 3, 12 days later, and that instead of a big mess that constantly needs debugging, you will instead find that you eventually will need less tests and the code works more than it fails.

It will almost always take up more memory than the imperative solution, except when it doesn't, so benchmark and experiment. Using laziness can make things run a lot faster with less memory, but writing mostly non-mutable code does have the side effect of more objects and data in memory.

All in all, this kind of code led me personally to writing more functionality with less code and far less bugs. I envy all of you who gets to learn these lessons early in your careers.

No animals were injured in the writing of this book, however a lot of flowers were burned.
