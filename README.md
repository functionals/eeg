There are six predicates which must be defined at run time.  This can be done using the command structure:

:-dynamic Name/Arity

where Name is the predicate and Arity is the variables of the predication.  For example, predicate(X,Y) is Name "predicate" and has an Arity of 2 (X,Y).  The command would then be:

:- dynamic predicate/2

This is incomplete, however, and requires the use of the "assert" function of prolog, which is done by using the "assert/1" command.  Thus the full command structure for defining a dynamic run time predication is done by the following:

:- dynamic l:grab/2.

This must be typed for each of the six predicates:

l:grab/2

l:letter/2

l:noun_p/0

l:prep_p/0

l:verb_p/0

l:word/4

Once done, the algorithms will compile without error, and work more efficiently.
