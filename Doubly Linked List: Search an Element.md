# 📝 Doubly Linked List: Search an Element

This Python program demonstrates the implementation of a **Doubly Linked List** where you can insert elements at both the beginning and the end of the list. Additionally, it allows you to search for a specific element in the list.

---

## 🎯 Aim

To write a Python program that:
- Implements a **Doubly Linked List** with functions to insert elements at the beginning and the end of the list.
- Implements a search function to check if a given element exists in the list.

---

## 🧠 Algorithm

1. **Step 1:** Define a class `Nodeq` with:
   - `data` to store the node's value.
   - `next` to store the reference to the next node.
   - `prev` to store the reference to the previous node.

2. **Step 2:** Define a class `DoublyLinkedList` with:
   - `head` to point to the first node.

3. **Step 3:** In the `DoublyLinkedList` class, define methods:
   - `insert_beginning(data)` to insert a node at the beginning.
   - `insert_end(data)` to insert a node at the end.
   - `search(data)` to search for an element in the list.

4. **Step 4:** Create an instance of `DoublyLinkedList`.
   - Insert elements at the beginning and end.
   - Search for specific elements.

---

## 💻 Program
```
class Node:
def init (self, data):
self.data = data
self.next = None
class LinkedList:
def init (self):
self.head = None
def push(self, new_data):
new_node = Node(new_data)
new_node.next = self.head
self.head = new_node
def search(self, x):
current = self.head
while current:
if current.data == x:
return True
current = current.next
return False
llist = LinkedList()
llist.push(10);
llist.push(30);
llist.push(11);
llist.push(21);
llist.push(14);
data = int(input())
if llist.search(data):
print("Yes")
else:
print("No")
```

## Sample Output
<img width="319" height="184" alt="image" src="https://github.com/user-attachments/assets/5069fc24-9bf4-4eb3-80f0-04b16e2dcc02" />

## Result
Thus the program has been successfully executed
