In this chapter, we will develop a complete program: goto, a URLShortener web application, because the web is all-ubiquitous, and we don’t want to type long URLs. The example is taken from the excellent lecture from Andrew Gerrand at FOSSDEM 2011. We will do this in 3 stages; each stage has more functionalities and shows progressively more features of the Go language. We will draw heavily on what we have learned about web applications in Chapter 13.

Version 1: a map and a struct are used, together with a Mutex from the sync package and a struct factory.

Version 2: the data is made persistent because it is written to a file in gob-format.

Version 3: the application is rewritten with goroutines and channels.

Version 4: what has to change if we want a JSON-version.

Version 5: a distributed version is made with the rpc protocol.
