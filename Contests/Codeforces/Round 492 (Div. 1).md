#div1

[Dashboard - Codeforces Round 492 (Div. 1) [Thanks, uDebug!] - Codeforces](https://codeforces.com/contest/995)

### E. Number Clicker

#graphs #meet-in-the-middle

The graph is nearly random, so doing a meet in the middle bfs will probably run pretty fast. Won't have to hit very many nodes.

### F. Cowmpany Cowmpensation

#trees #dp #polynomials #interpolation #upsolved

The naive dp is $O(n^2)$, but the answers to the dp at each node is a polynomial. The degree is at most n which can be proven through induction, so you can do the naive dp and then use interpolation to calculate $dp[0][N]$.