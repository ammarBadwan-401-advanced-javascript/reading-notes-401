# Stacks and Queues

## Stack

* A stack is a data structure that consists of nodes, each of them references the next node in the stack but not the previous one.

* Stack Terminology:
1-Push : Nodes that are inserted are pushed

2-Pop: Nodes that are removed.

3-Top: The top of the stack.

4-Peek: See the value of the top node of the stack.

5-IsEmpty: Returns true if a stack is empty.

* Stack follows concepts of First in last out, and Last in first out.

## Push O(1)

Pushing node into a stack will always be O(1) because it takes the same amount of time no matter how many nodes you got inside the stack.

* You push by assigning it as the new top, so first:

1- Create a new node.

2- Assign the new node's next to the previous top node.

3- Reassign the top reference to the new node.

## Pop O(1)

You can delete the top node by popping out the top node, reassigning the entire stack to a reference.

Reassign the top to the next value and return the value of temp Node.

## Peek O(1)

Peek will be inspecting the top node of the stack.

First check if isEmpty is true, but then you can return the value of the top node in the stack.

## Queue

1- Enqueue: Nodes that are added to the queue.

2- Dequeue: Nodes that are removed from the queue.

3- Front: The front or first node of the queue.

4- Rear: The last node.

## Enqueue O(1)

To add, first change next property of the read node to the new node,after that we need to change the read reference point to the new node.

## Deqeueu O(1)

You always remove the front node in a queue, first create a temporary reference named temp and point it to the same node that the front is pointing to.

Then re-assign front to the next value of the queue, then remove the valaue and return the temp node after changing the front reference point.

## IsEmpty O(1)

if the front is null, then return true.