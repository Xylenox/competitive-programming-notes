#div2 

https://codeforces.com/contest/1705

### F. Mark and the Online Exam

#randomized #math #zealots #to-upsolve

I'm thinking about making 1024 orthogonal basis, where $B_{ij} = 1$ if $i$ & $j$ has an odd number of bits, and and $0$ otherwise. Then, pick 675 random basis'. Probably that is enough information to find a unique solution.

So if our answers are (1, 1, 1, -1), and we guess (-1, -1, 1, 1), we would get -2 as our value.

Center at (0.5, 0.5), or (0, 0)? Probably (0, 0) is better, since it's more convenient.

I think this basis idea has some merit, but it's really hard to find the answer after getting the values.

I read the editorial, it seems you can do 2 moves for 3 things. If you query FFF and FTF to begin with, if you query TTF and get 2 or -2, you know the first two. Otherwise if you get 1 or -1, query TFT. The first two must either give +2 or -2. If -3, the answer is FTF. If -1, the answer must be FTT. If 1, the answer is TFF, and if 3 the answer is TFT. 