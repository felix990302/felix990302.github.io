---
layout: page
title:  RPS Bot
---
![RPS](/assets/pics/RPS.png){: .img-center}

&nbsp;
&nbsp;

# Try Me Out!
[Windows](/assets/downloads/RPS.exe)

[Linux](/assets/downloads/RPS)

&nbsp;
&nbsp;

## Requirements
[Racket](https://download.racket-lang.org/)

### Instructions
Windows: run the .exe file by method of your choice

Linux: run the program as you would a compiled C program ie ./<<program name>>

&nbsp;
&nbsp;

# What Am I?

A simplified implementation of the Iocaine Powder algorithm which won the first world Ro-Sham-Bo competition.

The algorithm is written in Racket, a dialect of LISP and Scheme.

My version switches between 6 meta strategies for each algorithm by guessing, second guessing, and triple guessing opponents then doing the same from the opponent's point of view.

The most basic algorithm simply looks at the opponent's last played move.

History matcher, by far the strongest algorthm, seeks to match the longest sequence of moves identical the last played moves of the opponent.

Distribution looks at the frequency of moves the opponent has been playing and chooses a random but weighted move accordingly.

The fallback method is to play randomly, as there is no way to beat by a wide margin, a truly random player.

Input and output are implemented as unbounded streams.

&nbsp;
&nbsp;

[source](https://github.com/felix990302/Racket-Algorithms/blob/master/a11/RPS.rkt)
