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

//Referenced https://github.com/COSC3020/little-o-proof-JacobMorgan3 for help 
finding formal big-Oh definition

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$
$f(n)\in O(g(n)) \iff \exists c>0, \exists n_0 > 0: f(n) \le c g(n)$

$f(n)\in o(g(n)) \implies f(n)\in O(g(n))$

$\implies$ { $\forall c>0, \forall n\ge n_0 : f(n) < c g(n)$ } $\in$  { $\exists c>0, \forall n\ge n_0 : f(n) \le c g(n)$ }

Thus we can say for certain that if for all $c>0, f(n) < c g(n)$ is true, then there must exist some $c>0$ such that $f(n) \le c g(n)$ since the set of c's that make little-oh true are a subset of the set of c's making big-oh true.