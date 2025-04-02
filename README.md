# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Answers

From the definition of isomorphism, graphs $G_1=(V_1 , E_1)$ and $G_2 = (V_2, E_2)$ are isomorphic to eachother if there exists a one-to-one and onto function between one another. 

We say a function is one-to-one provided all different different inputs always result in different outputs. This means that $|V_1|\le|V_2|$ as every input maps to a distinct output.

We say a function is onto provided all different outputs always result in different inputs. This means that $|V_1|\ge|V_2|$.

For this function to be both one-to-one and onto then both $|V_1|\le|V_2|$ and $|V_1|\ge|V_2|$ must be true. As we are proving this for cases when $|V_1|\neq|V_2|$, this gives us two cases to prove: when $|V_1|<|V_2|$ and when $|V_1|>|V_2|$.

* $(|V_1|\le|V_2)\land(|V_1|\ge|V_2)$
* $((|V_1|=|V_2)\lor(|V_1|<|V_2))\land((|V_1|=|V_2)\lor(|V_1|>|V_2))$
* $(F\lor(|V_1|<|V_2))\land(F\lor(|V_1|>|V_2))$

Case 1: $V_1|<|V_2|=T$
* $(F\lor T)\land(F\lor F)$
* $T\land F$
* $F$

Case 2: $V_1|>|V_2|=T$
* $(F\lor F)\land(F\lor T)$
* $F\land T$
* $F$

From the two cases, I have proved that if $|V_1|<|V_2|$ or $|V_1|>|V_2|$ then the the function is not both one-to-one and onto which means they cannot be isomorphic.

## Sources

I used the definition of one-to-one and onto from my Discrete Mathmatics course (MATH 208 from North Dakota University).

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.