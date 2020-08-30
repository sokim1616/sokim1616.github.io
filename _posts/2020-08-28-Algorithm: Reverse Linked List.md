---
layout: post
title:  "Algorithm: Reverse Linked List"
author: So Hyun K.
date: 2020-08-28
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
let headNode = head;
let nextNode = head.next;
```

The last element after the final node had to be null, so I assigned the node after the head to be null.
```
headNode.next = null;
```






The Sahara is a desert located on the African continent. It is the largest hot desert in the world, and the third largest desert overall after Antarctica and the Arctic. Its area of 9,200,000 square kilometres (3,600,000 sq mi) is comparable to the area of China or the United States.[3] The name 'Sahara' is derived from a dialectal Arabic word for "desert", ṣaḥra (صحرا /ˈsˤaħra/).

The desert comprises much of North Africa, excluding the fertile region on the Mediterranean Sea coast, the Atlas Mountains of the Maghreb, and the Nile Valley in Egypt and Sudan. It stretches from the Red Sea in the east and the Mediterranean in the north to the Atlantic Ocean in the west, where the landscape gradually changes from desert to coastal plains. 

To the south, it is bounded by the Sahel, a belt of **semi-arid tropical savanna** around the Niger River valley and the Sudan Region of Sub-Saharan Africa. The Sahara can be divided into several regions including: the western Sahara, the central Ahaggar Mountains, the Tibesti Mountains, the Aïr Mountains, the Ténéré desert, and the Libyan Desert.

For several hundred thousand years, the Sahara has alternated between desert and savanna grassland in a 20,000 year cycle caused by the precession of the Earth's axis as it rotates around the Sun, which changes the location of the North African Monsoon. The area is next expected to become green in about 15,000 years (17,000 AD).