# Graph Coloring Problem
We have been given a graph and we are asked to color all vertices with the ‘M’ number of given colors, in such a way that no two adjacent vertices should have the same color.

It it is possible to color all the vertices with the given colors then we have to output the colored result, otherwise output ‘no solution possible’.

The least possible value of ‘m’ required to color the graph successfully is known as the chromatic number of the given graph.


Backtracking Algoritm:                                                                                                                                         
Create a recursive function that takes the graph, current index, number of vertices, and output color array.
If the current index is equal to the number of vertices. Print the color configuration in the output array.
Assign a color to a vertex (1 to m).
For every assigned color, check if the configuration is safe, (i.e. check if the adjacent vertices do not have the same color) recursively call the function with the next index and number of vertices
If any recursive function returns true break the loop and return true
If no recursive function returns true then return false
