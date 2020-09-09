## Linked Lists

* Linked Lists are **linear data structures**, meaning that there is a sequence and an order to how they are constructed and traversed.   

* Linked Lists are similar to arrays - HOWEVER where arrays require memory in a contiguous block, linked lists do not need to be contiguous because they contain references to the next (and sometimes prior) node in the list.  They are **dynamic data structures** (as opposed to arrays, which are considered static data structures)

* In addition to singly linked lists (which contain a next reference) and doubly linked lists (which contain both a next and previous reference) one can make a circular linked list that begins with a 'tail' and then goes on to reference the next/prior node in a loop (instead of ending in a null value) - excluding the tail from the loop so that we have a starting point to work with.

---

* **Big O Notation** is a way to evaluate the performance of an algorithm based on efficiency - specifically in terms of time and memory

* When adding new nodes to a linked list, one needs to update the references not just in the new node, but also in any node affected (always the prior node, and in the case of a doubly linked list the next node as well)

* Because of the nature of linked lists, when inserting a new node we need to traverse the current list as far as the point where we want to insert the new node in order to create the references correctly.

  - This means that inserting new nodes at the head of the list is always the most efficient place to add a node, and becomes less efficient the farther down the list you need to add a node.

Overall, *arrays* are preferable if you:
* know the size of the list upfront
* need random access to elements
* want to iterate quickly through the elements

Alternately, *linked lists* are preferable if you:
* do *not* know the size of the list upfront
* do *not* need random access to elements
* primarily want to add or remove elements

