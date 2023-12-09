# Linked List Merger

A Python implementation to merge two sorted linked lists with constraints on values and the number of nodes.

## Overview

This script defines a `ListNode` class representing a node in a linked list. The `mergeTwoLists` function merges two sorted linked lists while adhering to the following constraints:

- Each node's value should be within the specified range of -100 to 100.
- The number of nodes per list should be in the range of 0 to 50.

## Usage

```python
Example Usage

from linked_list_merger import ListNode, mergeTwoLists

# Test the code with the given example
list_1 = ListNode(1)
list_1.next = ListNode(2)
list_1.next.next = ListNode(4)

list_2 = ListNode(1)
list_2.next = ListNode(3)
list_2.next.next = ListNode(4)

# Merge the two lists
merged_list = mergeTwoLists(list_1, list_2)

# Print the merged list if it is not None
if merged_list is not None:
    print("Merged List:")
    current_merged = merged_list
    while current_merged:
        print(current_merged.value, end=" -> ")
        current_merged = current_merged.next
    print("None")
