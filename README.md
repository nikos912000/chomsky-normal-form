Chomsky Normal Form (CNF) Converter
==================================

This script can be used to convert a Context Free Grammar (CFG) to Chomsky Normal Form (CNF). 

The implementation is based on the theory provided in the book ''*Elements of the Theory of Computation (2nd Edition)*", by Harry Lewis and Christos H. Papadimitriou.

###*Theory*


According to the book, the right hand side of the rule in a CFG in Chomsky Normal Form must have length two. 

So, there are 3 kind of rules that need to be removed/replaced:

1. **Long rules** (eg. A->BCD)
2. **Empty rules** (eg. A->e)
3. **Short rules** (eg. A->a)

Input
-----

User's input include:

* Number of rules
* Initial state
* Rules, each on in a space-delimited form (A BC, for A->BC)

Example
-------
Here 's an example indicating how to use the script:

| Message              | User Input |
| :------------------: | :--------: | 
| Give number of rules | 3          | 
| Give initial state   | S          |
| Rule #1              | S SS       |
| Rule #2              | S (S)      |
| Rule #3              | S e        | 