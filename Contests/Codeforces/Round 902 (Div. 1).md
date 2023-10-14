#div1
https://codeforces.com/contest/1876

### C. Autosynthesis

#graphs 

We can represent the problem as a graph, where each node has exactly one out edge. Now, we want to color each node either black or white such that every black node has at least one white node pointing to it, and each white node has no white nodes pointing to it. Our answer is going to be the edges corresponding to the white nodes.

Leaves must be white, since they have no edges into them. Any node that a white node is pointing to must be black. Do a top-sort until there are only cycles left.

For the remaining cycles, if they are odd cycles, it's impossible. Otherwise just two-color the cycle.

### D. Lexichromatography

#counting #dsu 

The second condition is equivalent to saying that for any two $i$ and $j$ such that $a[i] = a[j]$ and there are no $k$ where $i < k < j$ and $a[i] = a[k]$, $i$ and $j$ must be different colors. Also, for any partition, if it's good, we can swap the colors and then it won't be good. So, if we take the total number of partitions $2^{distinct\ values}$, and subtract out the number of partitions such that the blue and red subsequences are equal, that number divided by two will be the answer.

Now we need to count the number of ways to have both subsequences be equal. Consider two values. Take the subsequence corresponding to those values, e.g. (1, 1, 2, 2) is one such subsequence of (1, 1, 3, 2, 2).