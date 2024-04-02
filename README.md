[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

//Referanced https://github.com/COSC3020/little-o-proof-JacobMorgan3 for help 
finding formal big-Oh definitions

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$
$f(n)\in O(g(n)) \iff \exists c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

$f(n)\in o(g(n)) \implies f(n)\in O(g(n))$

$\implies$ { $\forall c>0, \forall n\ge n_0 : f(n) < c g(n)$ } $\in$  { $\exists c>0, \forall n\ge n_0 : f(n) < c g(n)$ }
The only difference between little-oh and big-oh is the " $\forall c$ " in little-oh
and the " $\exists c$ " in big-oh with the same condition, we can say for certain that
if for any constant $c$ the condition is true, then there must exist a constant $c$
such that the condition is true. 