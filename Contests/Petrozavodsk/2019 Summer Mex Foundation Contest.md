https://codeforces.com/gym/102412

### A. The One Polynomial Man

#fft #math #discrete-log

First observation is that all terms in the numerator and denominator have the same degree. That means that only the ratio a/b matters. We can take the discrete log of every value, and now the problem is for each ratio how many values subtract to this ratio, which is classic fft.