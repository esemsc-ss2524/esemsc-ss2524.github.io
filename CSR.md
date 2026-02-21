---
layout: default
title: Compressed Sparse Row
---

# Compressed Sparse Row

Efficient data structure to store sparse matrices.

Example sparse matrix:
```
Row 0: [ 5, 0, 0, 8]
Row 1: [ 0, 0, 3, 0]
Row 2: [ 0, 6, 0, 0]
Row 3: [ 7, 0, 0, 4]
```

### Three Arrays
- Values Array
```
V = [5, 8, 3, 6, 7, 4]
```

- Column Indices Array (zero-indexed)
```
C = [0, 3, 2, 1, 0, 3]
```

- Row Pointers Array (zero-indexed)
Indices in the `V` array where rows start.
```
R = [0, 2, 3, 4, 6]
```

Here, 6 corresponds to the total num of non-zero elements (6), marking the *end of matrix*.
