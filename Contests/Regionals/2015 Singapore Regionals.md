https://open.kattis.com/problem-sources/2015%20ACM%20ICPC%20Singapore%20Regional

### Apples, Cherries, and Mangos

#generating-functions #fft #combinatorics #inclusion-exclusion
#todo

First, try $\frac{(a+c+m)!}{a!c!m!}$. This counts all ways of arranging the fruits in general, but we're over counting cases where two fruits of the same kind are adjacent. To combat this, we can use inclusion-exclusion.

Subtract out the number of ways to arrange the fruits such that at least 1 pair of fruits are adjacent. However, this would over subtract cases where 2 pairs of fruit are adjacent. So we add those back in, and then subtract out 3 pairs, etc.

Another way to think about it is in terms of groups of fruits that are the same. If we have a group of 2 adjacent apples, that corresponds to one pair being the same, 3 adjacent Apples corresponds to 2 pairs, and so on. In other words, the number of pairs is $n-num\ groups$.

Now, if we know the number of groups of each type, calculating the number of ways to arrange these groups is easy. Let $g_a$ be number of groups of apples, $g_c$ be groups of cherries, and $g_m$ be number of groups of mangos. Then the number of ways to arrange these groups is $\frac{(g_a+g_c+g_m)!}{g_a!g_c!g_m!}$.

Now we would like to calculate the number of ways to have a certain number of groups