fuckthisshit
============

State-of-the-art C++ code quality checker and debugging tool.

The algorithm works by deleting all the lines in your source code where g++ claims there is an error. It does this repeatedly until g++ doesn't complain anymore. But sometimes, that's just not enough, so I added a few options:

```
./fuckthisshit lab.cpp
```
will *clean* lab.cpp of all errors returned by the compiler


```
./fuckthisshit --hard lab.cpp
```
will remove all errors and warnings returned by the compiler


```
./fuckthisshit --roulette lab.cpp
```
will first remove all errors; then, fuckthisshit (TM) will proceed to wipe out your hard-drive if and only if your program erred. Very fun if you are "feeling lucky".


```
./fuckthisshit --suicide lab.cpp
```
will first remove all errors and warnings; then fuckthisshit (TM) will wipe out your hard-drive regardless of whether or not your program erred. For what it's worth, fuckthisshit (TM) will first try to repair your program completely before wiping out the hard-drive.


Based on Matt Diamond's <a href="https://github.com/mattdiamond/fuckitjs">fuckitjs</a> jQuery plugin.
