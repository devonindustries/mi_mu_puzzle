# Solving the MI-MU Puzzle

The very first puzzle in the book 'An Eternal Golden Braid' presents us with a formal system, where we are given a set of rules, and an initial condition **MI**, and we are asked whether or not it is possible to produce **MU** based on the following axioms:

1. **xI** may be transformed into **xIU**;
2. **Mx** may be transformed into **Mxx**;
3. **III** may be replaced with **U**;
4. **UU** may be removed where present.

where we use **x** to refer to any arbitrary string. So, for example, the string **MI** may be transformed into **MIIII** by applying Axiom 2 twice, and then into either **MIU** or **MUI** by applying Axiom 3.

In terms of code, we declare a function `next_step` which does not take **M** into consideration throughout any of its calculations, since the **M** remains at the same spot throughout the entire puzzle. The goal of this project is to exhaust all of the possible outcomes, and find out if it is indeed possible to derive **MU** from **MI**.