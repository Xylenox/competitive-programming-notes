[Dashboard - 2018 ACM-ICPC World Finals - Codeforces](https://codeforces.com/gym/102482)

### C. Conquer the World

#trees #to-upsolve

### D. Gem Island

#math #combinatorics #probability #inclusion-exclusion #to-upsolve 

The probability that a certain sequence of gem counts is possible, for example, 4, 1, 2. To calculate the probability, first count the number of ways to do it, and then divide by the total number of ways ($\frac{(n+d-1)!}{(n-1)!}$). The number of ways is $(4-1)!*(1-1)!*(2-1)!*\frac{4!}{(4-1)!(1-1)!(2-1)!}$ . The first three factorials are the ways to permute among each person's gems, and the fraction is the number of ways to choose which gems go to which people. However, the factorials cancel out, and so every sequence of counts is equally likely.

Now, the problem turns into out of all ways to divide $d$ gems among $n$ people, what is the average sum of the biggest $r$ people. There is some stars and bars behavior.

### E. Getting a Jump on Crime

#math #bfs

### G. Panda Preserve

#geometry #voronoi