=============== PROJECT 1 ===============
===     Austen Kelly (951632601)	  ===
===            10/14/2019	       	  ===
=========================================

This project contains a lexer written in Re/flex.
It includes 

REflex reads quack.lxx and creates lex.yy.cpp. 
Building in docker will compile lex.yy.cpp to get
the file-scanning program.

RE/flex should be installed in the standard places, 
with a library in /usr/local/lib, include files 
in /usr/local/include/reflex, and 'reflex' on the 
search path.

To run (after building):

./bin/lexer samples/LexChallenge.qk