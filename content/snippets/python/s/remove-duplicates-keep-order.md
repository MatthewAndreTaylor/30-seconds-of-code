---
title: Remove duplicates, and preserve the list's order.
type: snippet
language: python
tags: [list]
cover: dark-leaves-6
dateModified: 2023-11-29
---

Remove all duplicates from a list, preserving the original list's order.

- Use `set()` on the given list to remove duplicates.
- Use `sorted()` to return a sorted list comparing elements of the list based on their indices in the original list.

```py
def rem_duplicates_keep_order(lst):
  return sorted(set(lst), key=lst.index)
```


```py
rem_duplicates_keep_order([1, 2, 2, 3, 4, 4, 5]) # [1, 2, 3, 4, 5]
rem_duplicates_keep_order(['x', 'y', 'x', 'z'])  # ['x', 'y', 'z']
```