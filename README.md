# LTimer

Simple yet powerful object-oriented timer library for Arduino (and other systems).

Why did I do it?

I couldn't find the functionalities I was looking for in other Arduino libraries... They were either too simplistic or too difficult to get used to.
It has a strong (chrono-)logical model, meaning the order in which the timers will fire will always be the same, given the same initial conditions.

How does it work?

The main difference with other libraries is that it always knows what timer is next to be fired.
This is practical, because, then, you can just wait the right amount of time.

What are its weaknesses?

I can see it's not perfect. For example, the memory allocation is standard C++ which is good but may be considered too slow for some people. This is not a big deal: I can think of simple improvements to handle this. If you need it contact me.
It's powerful, and handles a lot of things which makes it a little slow sometimes ("just a little").
It's not perfect: as I had Arduino in view, it's been made simpler on a few little points.

What are its strong aspects?

Strong object-oriented model, relatively pure C++.
Strong chronological model.
Handles 32-bit overflow transparently.
Can be adapted easily (to a different granularity (microsecond, nanosecond, ...), to other platforms, ...)

Versioning

v1.0: basic functionality (goals: one simple LTimer object, <10kb)

v2.0: extensions of v1.0 (goals: new objects for extended functionalities, <20kb)

PS: I've got a new library on that subject which will be made available in github... Interested? contact me at ludovic.bertsch@gmail.com
