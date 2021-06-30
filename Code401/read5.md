# Linked Lists :
### Reading, Research, and Discussion
* **Linked List:** A sequence of nodes that are connected (linked) to one another. Cricially, each node references the next node in the link.

* Two types of linked lists, each of which refers to the number of references each node has:
1. **Singly** : Nodes only have one reference, and it points to the next node in a linked list.
2. **Doubly**:  Nodes have two references - which point to both the next and the previous node.
* **Node** : The individual items or links in a linked list. Contain data for each item or link. Each node contains at least a property called next, which references the next node in the list.

### Properties of Nodes:

Next: Each node has a property named Next
  * “Next” represents the next node
  * If “next” is ever null, it means that that node is the the last one in the list
* Head: The Head is a property only of the first node in a linked linked
* Current: A reference to whatever node is being examined at this moment.

### Traversing Linked Lists

* For loops cannot be used to traverse linked lists.
Instead, we use the “Next” value of nodes to “point” us to the next reference and guide the traversal of the list
* While loops are the best method for travering linked lists
Continually check that the “next” node is not “null”.

### Other Sources
[Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

[What’s a Linked List, Anyway? (Part 1)](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)

[What’s a Linked List, Anyway? (Part 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)