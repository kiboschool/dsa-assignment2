# Assignment 2 Analysis

## Task 1: Mystery Sort

### Random List Results

Below is the table of results from running the mystery sort on random lists of various sizes:

| List Size | Number of Comps | Number of Moves |
|-----------|-----------------|-----------------|
|  1000     |    499500       |    765147       |
|  2000     |    1999000      |    3096396      |
|  4000     |    7998000      |    12252267     |

As the length of the list doubles 1000 --> 2000, the number of comparisons quadruples (~500k --> 2M). As the length of the list doubles from 2000 --> 4000, the number of comparisons again quadruples (2M --> 8M). Therefore, the number of comparisons is likely O(n^2) for random lists.

As the length of the list doubles 1000 --> 2000, the number of moves approximately quadruples (750k --> 3M). As the length of the list doubles from 2000 --> 4000, the number of moves again quadruples (3M --> 12M). Therefore, the number of moves is likely O(n^2) for random lists.

Overall, the time complexity is therefore O(n^2).

### Almost-Sorted List Results

Below is the table of results from running the mystery sort on almost-sorted lists of various sizes:

| List Size | Number of Comps | Number of Moves |
|-----------|-----------------|-----------------|
|  1000     |    499500       |    1443         |
|  2000     |    1999000      |    2958         |
|  4000     |    7998000      |    6315         |

As the length of the list doubles 1000 --> 2000, the number of comparisons quadruples (~500k --> 2M). As the length of the list doubles from 2000 --> 4000, the number of comparisons again quadruples (2M --> 8M). Therefore, the number of comparisons is likely O(n^2) for almost-sorted lists.

As the length of the list doubles 1000 --> 2000, the number of moves approximately doubles (1,500 --> 3,000). As the length of the list doubles from 2000 --> 4000, the number of moves again doubles (3,000 --> 6,000). Therefore, the number of moves is likely O(n) for almost-sorted lists.

Overall, the time complexity is still O(n^2) because the n^2 in the comparisons dominates the O(n) term from the moves.

## Task 2: Radix Sort

### Random List Results

Below is the table of results from running radix sort on random lists of various sizes:

| List Size | Number of Moves |
|-----------|-----------------|
|  1000     |    5000         |
|  2000     |    10000        |
|  4000     |    20000        |

As the size of the list doubles, the number of moves doubles. Therefore, the algorithm is O(n).

### Almost-Sorted List Results

Below is the table of results from running radix sort on almost-sorted lists of various sizes:

| List Size | Number of Moves |
|-----------|-----------------|
|  1000     |    5000         |
|  2000     |    10000        |
|  4000     |    20000        |

As the size of the list doubles, the number of moves doubles. Therefore, the algorithm is O(n).
