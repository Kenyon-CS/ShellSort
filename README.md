# ShellSort

## Explanation
1. Gap Sequence:
  - Shell Sort uses a gap sequence to divide the list. Here, we start with a gap of n/2 and reduce the gap by half each time (```gap /= 2```) until it reaches ```1```.
  - A gap of ```1``` is equivalent to a regular Insertion Sort.
2. Gapped Insertion Sort:
  - For each gap, the algorithm performs an insertion sort on elements separated by that gap.
  - The inner loop shifts elements in the sorted gap until the correct position for the current element (```arr[i]```) is found.
3. Efficiency:
  - By starting with larger gaps, Shell Sort reduces the number of overall shifts needed, improving performance compared to a standard Insertion Sort.
