---
layout: post
title:  "Algorithm: Reverse Linked List"
author: So Hyun K.
date: 2020-08-31
categories: [ Dev Diary ]
tags: [ Data Structure ], [ Linked List ]
image: assets/images/16.jpg
---

Ever since the boot camp has ended, I've been involved in a study group that solves algorithm problems every morning.
Since algorithm is not my strength, I had to work even harder to keep it up.

Today, I solved a problem in ***leetcode*** related to **linked list**, titled "Reverse Linked List".
The goal was to basically reverse a given linked list.

The given code was this:
```
var reverseList = function(head) {
    
};
```
where **head** is a linked list in the form of: [1, 2, 3, 4, 5].

The structure of a linked list might seem like the one of an array, but they are two different things.
A linked list is a type of a **data structure** composed of elements called 'nodes', which is composed of a 'head' and a 'tail', or 'next'.

So to begin with, I made a conditional statement where if there is no linked list, just return the given input.
```
if (!head) return head;
```

And I assigned two variables that is assigned to the head node and the node after the head node.
```
let node = head;
let nextNode = head.next;
```

The last element after the final node had to be null, so I assigned the node after the head to be null.
```
node.next = null;
```

After that, I used the while loop where as long as the nextNode exists, there will be a cycle of elements changing places with each other.
Let's take a look at the code first.
```
while(nextNode) {
    const nextNextNode = nextNode.next;
    nextNode.next = node;
    node = nextNode;
    nextNode = nextNextNode;
}
```
Inside the while loop, I made another variable called 'nextNextNode', which is the node after the nextNode.

(It's like a tongue twister, huh? XD)

And then, the final outcome would be returned.
So basically, the whole point is to change the first three elements (nodes) of the given linked list, so that the head becomes the tail, and the tail becomes the head.

Below is the final code:
```
var reverseList = function(head) {

    if (!head) return head;
    
    let node = head;
    let nextNode = head.next;
    
    node.next = null;

    while (nextNode) {
        const nextNextNode = nextNode.next;
		nextNode.next = node;
        node = nextNode;
        nextNode = nextNextNode;
    }
    
    return node;
};
```

Thanks for reading, and please let me know if there's anything I should fix! :)