https://open.kattis.com/problem-sources/2015%20ACM%20ICPC%20Singapore%20Regional

### Apples, Cherries, and Mangos

#generating-functions #fft #combinatorics #inclusion-exclusion
#todo

First, try $\frac{(a+c+m)!}{a!c!m!}$. This counts all ways of arranging the fruits in general, but we're over counting cases where two fruits of the same kind are adjacent. To combat this, we can use inclusion-exclusion.

Subtract out the number of ways to arrange the fruits such that at least 1 pair of fruits are adjacent. However, this would over subtract cases where 2 pairs of fruit are adjacent. So we add those back in, and then subtract out 3 pairs, etc.

Now we need to count the number of ways to 