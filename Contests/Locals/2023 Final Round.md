### Drake Robbing

#greedy #dp #knapsack #upsolved

Do a greedy based on efficiency until full, then remove 1000 from each. Then do a knapsack dp on the remaining 20\*1000\*1000 capacity. There's 20 elements, but each one has at most 1,000,000 capacity left. To do the 0-k knapsack, Sslit each element into $log_2(count)$ elements, and then do a 0-1 knapsack,