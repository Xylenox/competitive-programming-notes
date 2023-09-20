### Drake
#greedy #dp #upsolved

Do a greedy based on efficiency until full, then remove 1000 from each
Then do a dp on the remaining 20\*1000\*1000 capacity
how many elements are there?
There's 20 elements, but each one has at most 1,000,000 capacity left
Split each element into $log_2(count)$ elements, and do a 0-1 knapsack