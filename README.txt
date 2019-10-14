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

To set up:
	1) Run "make image"
	2) Run "docker image ls" (to check it successfully
				created the image "proj1")
	3) Run "docker run -it proj1"

The dockerfile copies from michalyoung/cis461:base, creates
my project as proj1, and builds the program.

To run (after building):

	./bin/lexer samples/LexChallenge.qk

The output (for that example) should be:

CLASS	(258)	@5.0-3
IDENT	(273)	@5.6-13
(	(40)	@5.15
)	(41)	@5.16
{	(123)	@5.18
IDENT	(273)	@6.3-5
.	(46)	@6.7
IDENT	(273)	@6.8
=	(61)	@6.10
IDENT	(273)	@6.44
+	(43)	@7.11
IDENT	(273)	@7.13
;	(59)	@9.15
IDENT	(273)	@11.24
=	(61)	@11.26
STRING_LIT	(275)	@13.13-14
+	(43)	@13.17
STRING_LIT	(275)	@13.51
;	(59)	@13.52
}	(125)	@14.0

