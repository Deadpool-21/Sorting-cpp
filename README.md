
# Sorting in C++

### Aim

To implement and understand various sorting algorithms using C++, analyze their time and space complexities, and compare their performance based on different input sizes.

---

### Objectives

* Understand the working of popular sorting algorithms:

  * Bubble Sort
  * Selection Sort
  * Insertion Sort
  * Merge Sort
  * Quick Sort
* Implement these algorithms in C++.
* Analyze and compare their time and space complexity.
* Visualize sorting mechanisms using flowcharts.
* Construct tables for performance comparison.

---

### Theory

Sorting is the process of arranging data in a specific order, usually ascending or descending.
Efficient sorting is fundamental as it directly influences the performance of other algorithms such as searching, merging, and optimization tasks.

Sorting algorithms can be classified based on:

1. **Time Complexity** – Best, Average, Worst case performance.
2. **Space Complexity** – Extra memory usage.
3. **Stability** – Whether the relative order of equal elements is preserved.
4. **Method** – Comparison-based or non-comparison-based approaches.

---

### Sorting Algorithms Overview

| Algorithm      | Time Complexity (Worst) | Stability | Method           |
| -------------- | ----------------------- | --------- | ---------------- |
| Bubble Sort    | O(n²)                   | Stable    | Comparison-based |
| Selection Sort | O(n²)                   | Unstable  | Comparison-based |
| Insertion Sort | O(n²)                   | Stable    | Comparison-based |
| Merge Sort     | O(n log n)              | Stable    | Divide & Conquer |
| Quick Sort     | O(n²), Avg O(n log n)   | Unstable  | Divide & Conquer |

---

### Descriptions of Algorithms

1. **Bubble Sort**

   * Repeatedly compares adjacent elements.
   * Swaps them if they are in the wrong order.
   * After each pass, the largest element bubbles up to its correct position.
   * **Time Complexity:** O(n²), **Stable**.

2. **Selection Sort**

   * Finds the minimum element in the unsorted portion.
   * Places it at the beginning by swapping.
   * Repeats until the array is sorted.
   * **Time Complexity:** O(n²), **Unstable**.

3. **Insertion Sort**

   * Builds the sorted portion element by element.
   * Each new element is placed in its correct position relative to the already sorted part.
   * **Time Complexity:** O(n²), **Stable**.

4. **Merge Sort**

   * Divide-and-conquer algorithm.
   * Divides the array into two halves, recursively sorts them, and merges them back.
   * Guarantees O(n log n) performance.
   * **Time Complexity:** O(n log n), **Stable**.

5. **Quick Sort**

   * Divide-and-conquer algorithm.
   * Chooses a pivot element, partitions the array, and recursively sorts sub-arrays.
   * Very efficient in practice but suffers O(n²) in the worst case (e.g., already sorted arrays with poor pivot choice).
   * **Time Complexity:** Avg O(n log n), Worst O(n²), **Unstable**.

---

### Example: Quick Sort Time & Space Complexity

| Case    | Time Complexity | Space Complexity |
| ------- | --------------- | ---------------- |
| Best    | O(n log n)      | O(log n)         |
| Average | O(n log n)      | O(log n)         |
| Worst   | O(n²)           | O(log n)         |

---

### Conclusion

* **Simple algorithms** like Bubble Sort, Selection Sort, and Insertion Sort are easy to understand but inefficient for large datasets due to O(n²) time complexity.
* **Efficient algorithms** like Merge Sort and Quick Sort perform much better on large datasets, achieving O(n log n) on average.
* **Quick Sort** is often faster in practice due to in-place partitioning but can degrade to O(n²) in the worst case.
* **Merge Sort** guarantees O(n log n) performance and maintains stability, making it useful when order preservation is required (e.g., sorting linked lists).

