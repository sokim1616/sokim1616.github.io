---
layout: post
title:  "How Node.js Works"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/18.jpg
---

Node.js is highly-scalable, which means that it can be flexible and cope with increased uses. And this is because Node.js is **asynchronous**.
An **asynchronous** architecture can handle multiple requests, unlike **synchronous** one which is the exact opposite. When a request is received on the server, a thread is assigned to handle that request. In the process, it likely to query a database. When the database is processing the query, that thread is waiting for the process to be finished. (It cannot serve another client at the same time, so another thread is needed)

However, **asynchronous** architecture such as Node.js has a single thread that handles all requests: Database executing the query while serving another client.

In Node.js, when the database prepares the result, it puts a message in something called, "event queue", which the Node is continuously monitoring in the background. WHen the Node finds an event in this "queue", it will take the event out and process it.
This makes the Node idea for building apps that includes a lot of disk spaces, or other network accesses. In other words, Node.js is said to be **I/O-intensive**, because it can serve numerous clients without expanding the number of hardware.

However, Node.js should NOT be used for CPU-intensive apps, because such apps does not have much operations that works with the file system or the network.

To summarize, Node.js is a runtime environment that is suitable for data-intensive applications.