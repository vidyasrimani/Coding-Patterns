# Coding Patterns

These coding patterns will help you solve Leetcode problems effectively. These programs are written in Python.

| Coding Pattern                | Problem Format                            | Code Snippet                                  |
| :---                          |     :---:                                 |          ---:                                 |
| Sliding Window                | Input: Continuous Subarray with K elemenis|  `start = 0                                   |
|                               |        in a List/LinkedLList of N elements|   sum = 0                                     |
|                               | Approach: A Window of size K,             |   result = []                                 |
|                               | slide along the array                     |   for end in range(0, len(arr)):              |
|                               | Reason: Minimize duplicate operations     |       sum += arr[end]                         |
|                               | Time: `O(N)`                              |       if end >= k-1:                          |    
|                               | Brute Force Time: `O(N*K)`                |           result.append(sum/k)                |
|                               |                                           |           sum -= arr[start]                   |
|                               |                                           |           start+=1                            |
| :---                          |     :---:                                 |          ---:                                 | 




