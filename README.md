# QAOA_Maxcut_for_weighted_graphs
The code here is a modification from https://lucaman99.github.io/new_blog/2020/mar16.html
In order to understand the code and the idea being approximating _Maxcut_ using Quantum Approximate Optimization Algorithm (QAOA), I recomment you read [this](https://lucaman99.github.io/new_blog/2020/mar16.html) amzing guide from Musty thoughts.
However, you would need basics from [Variational Quatnum Eigensolver (VQE)](https://www.mustythoughts.com/variational-quantum-eigensolver-explained).
Moreover, I would urge you to read this awe inspring essay while will give you some _basis_ (pun intended!) to better comprehend the content of the aforementioned blogposts.
Furthermore, if you are not familiar with Linear Algebra, I recomment you pause here, revise it, learn it, and come back!

# The code
This code has a number of functions which would aid in estimating the ground state of a Hamiltonian of the cost function.
The cost function is minimized to do just that.

## Create a Graph
The first step in making use of this code is to declare a graph with some edges and defined weights, like this:
**A square graph would look like this**
**The graph would contain a set of edges**
*set_edges = [E(0,1,10), E(1,2,1), E(2,3,10),E(3,0,10)]
*graph_ = G(set_edges)*

## Aproximate the Max cut
**call the approximate_maxcut function defined in the code and pass the declared graph as a parameter
*approximate_maxcut(graph_)*

## Interprating the resutls
The final printed line is in the form _|0010>_ where each bit represent each node in either being S or S'