---
layout: post
title:  "How Node.js Works"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/7.jpg
---

Node.js is highly-scalable, which means that it can be flexible and cope with increased uses. And this is because Node.js is **asynchronous**.
An **asynchronous** architecture can handle multiple requests, unlike **synchronous** one which is the exact opposite. When a request is received on the server, a thread is assigned to handle that request. In the process, it likely to query a database. When the database is processing the query, that thread is waiting for the process to be finished. (It cannot serve another client at the same time, so another thread is needed)

However, **asynchronous** architecture such as Node.js has a single thread that handles all requests: Database executing the query while serving another client.