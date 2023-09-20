https://codeforces.com/gym/100960
### A. Prevent a Galactic War
#matrix #math #optimization
Basically turns into solving the inverse of a matrix, but you can do some optimization stuff on like

### E. Cryptographic Argument
#to-upsolve
Upsolve later

### F. The Jedi Killer
#geometry #casework #upsolved
Given three points and the dimensions of a T shape, find whether or not the three points can fit on the T.
At least two points must lie on the same line, by pigeon-hole principle. This leads to two cases, either they are both on the guards, or they are both on the main line.

I think you can do this with doubles, but it's sketchy. I'm doing it with fractions, where I get $\frac{dot(b-a, c-a)^2}{|b-a|^2}$, and $\frac{dot(b-a, c-a)}{|b-a|}$ should be the length of the projection. Similarly for cross product.

There is a special case for when all 3 points are collinear. In this case, if they are all on the guard, there is no restriction on each individual length, just the total length.