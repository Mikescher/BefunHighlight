![](https://raw.githubusercontent.com/Mikescher/BefunUtils/master/README-FILES/icon_BefunHighlight.png) BefunHighlight
==============

BefunHighlight is just a helper library mainly for BefunExec.  
BefunExec has normal Befunge syntax-highlighting implemented, that means that every character is colored based on its function.
The problem here is that there may be code that never gets executed (not part of the real program), or there may be code that only gets used inside of string-mode (so the function doesn't matter, only the ASCII value).

BefunHighlight tries to solve this by evaluating every possible path an program can execute and so calculating the ways a single command is used.
Based on these informations it's now possible for another program to better highlight the source code.

![](https://raw.githubusercontent.com/Mikescher/BefunUtils/master/README-FILES/BefunExec_ESH_example.png)

Be aware that put (**p**) and get (**g**) operations will invalidate the calculated values and it is needed to update them.

BefunHighlight can also calculate the graph of all possible ways your program can move (excluding put and get operations). This is a great way to debug and analyze your program:

![](https://raw.githubusercontent.com/Mikescher/BefunUtils/master/README-FILES/BefunExec_ESG_example.png)

Download
========

You can download the binaries from my website [www.mikescher.de](http://www.mikescher.de/programs/view/BefunUtils)

Set Up
======

*This program was developed under Windows with Visual Studio.*

You don't need other [BefunUtils](https://github.com/Mikescher/BefunUtils) projects to use this.  
Theoretically you can only clone this repository and use it.  
But it could be useful to get the whole BefunUtils solution like described [here](https://github.com/Mikescher/BefunUtils/blob/master/README.md)  
Especially BefunDebug could be useful for testing.

To see the this in action look at my [BefunExec](https://github.com/Mikescher/BefunExec) source code