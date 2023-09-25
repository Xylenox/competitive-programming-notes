#div2 

[Dashboard - Educational Codeforces Round 155 (Rated for Div. 2) - Codeforces](https://codeforces.com/contest/1879)

### E. Interactive Game with Coloring

#trees #interactive

The color of the parent edge must be different than the color of all of the child edges. This means that in order to do one color, every node must have no children.

In order to do two colors, each edge should be colored differently to the parent edge, so the coloring is forced. This leads to a problem when a node has exactly one child. Then, you don't know which edge to take. The only way to fix this is if all nodes with exactly one child have the same parity. Otherwise, you wouldn't be able to tell which one was which.

For three colors, just color the edge by the depth mod 3. Then, take the one after the 0, unless it's a leaf, in which case take the 1.