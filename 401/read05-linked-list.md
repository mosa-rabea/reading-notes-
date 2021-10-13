# linked list


### The definition 
it's a sequence of nodes that are connected to each other,
 each node is a reference to the next node in the link.

### linked list types:
* singly linked list. (the most commonly used)
* doubly linked list.
* circular linked list.
* doubly circular linked list.


### Traversal
when we want to traverse a linked list we cant use regular loop methods like for or foreach, we depends on 'Next' property in each node to guide us to next reference.

one of the best ways to approach a traversal is by using while() , this will allow you to keep checking the Next node if its null.

in linked list if we try to traverse on a null node, the program will crash after it throws an error.



### Terminology
* the linked list is considered as a data structure type, each node links to the next node in the list.
* next is a property for node which contains the reference to the next node.
* head is a reference for the first node in the linked list.
* in a singly linked list each node has only one reference which points to the next node in the list.
* in doubly linked list each node has two references, one for the next node and the other for the previous node.
* nodes they are the items which live in the linked list.


### adding new node to the front.

first thing you need to knwo is that you have to pay attention to all the references to be properly assigned.
the big O notation (both time and space complexity) of adding to the front method is always equals to O(1) .

#### adding steps:


* first we use the Add() method to pass the value of the node.
* then we want our newNode.Next to point to the same location that the Head is pointing at.
* re assign Head to point at the newNode.


### Add a node to the middle:

the big O notation of adding to the middle method is equals to O(n) because it uses a loop.

#### adding steps:
* first we use the Add() method to pass the value of the node.
* then use AddBefore or SddAfter method they are the same.
* traverse while the next node is not null.
* do a check for the value of the next node before moving current to the next node,if it equals to the value we want to put our newNode before.
* set the newNode Next equal to the existing node.





## [BACK](../README.md)