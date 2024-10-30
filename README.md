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

# How Shell Sort Works
## Step-by-Step Process:
1. **Gap Sequence**: The array is first sorted with a large gap (```n/2```). Then the gap is reduced to half, and the process repeats.
2. **Sorting Within Gaps**: For each gap, elements that are gap positions apart are sorted relative to each other.
3. **Final Pass with Gap = 1**: This final pass works like a traditional insertion sort, but with fewer elements to shift, thanks to the previous gapped sorting passes.

## Shell Sort Characteristics:
  - **Time Complexity**: Varies depending on the gap sequence used. Typically between O(n<sup>3/2</sup>) and 
𝑂(𝑛<sup>2</sup>) in most cases, but can be close to 𝑂(𝑛log<sup>2</sup>𝑛) with optimized gaps.
  - **Space Complexit**y: 
𝑂(1) since it’s an in-place sort.
  - **Stability**: Not stable, as it can change the relative order of equal elements.

This example shows how Shell Sort works, with its characteristic gap-based sorting approach, which makes it more efficient than simple quadratic sorts like Bubble Sort or Insertion Sort for larger arrays.
