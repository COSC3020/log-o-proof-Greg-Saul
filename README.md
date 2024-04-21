[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/fbkbKZ5N)
# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$



## Proof

$T(n) \in O(\log_{5} n) \iff \exists c, n_0: T(n) \leq c \cdot \log_{5} n \forall n \geq n_0$

let $\log_{5} n = \frac{\log_{2}n}{\log_{2}5}$

$\frac{1}{\log_{2}5}$ is a constant

=> $T(n) \in O(\log_{5} n) \iff \exists c, n_0: T(n) \leq \frac{c}{\log_{2}5} \cdot \log_{2} n \forall n \geq n_0$

=> $T(n) \in O(\log_{5} n) \iff \exists c, n_0: T(n) \leq c \cdot \log_{2} n \forall n \geq n_0$

When comparing these definitions, after using log properties to manipulate the statement, we can see that $O(\log_{5} n) = O(\log_{2} n)$








### Sources

https://www.efunda.com/math/exp_log/log_relation.cfm -> used for logarithmic properties






