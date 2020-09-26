---
layout: post
title:  "Node.js: A Runtime Environment"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/7.jpg
---

As mentioned in the previous post, Node.js is a runtime environment for JavaScript codes. So what exactly is a runtime environment?
Before giving a definition of what it is, a brief history of how Node.js was created should be explained first.

Before Node.js was born, JavaScript was used ONLY to build applications that run inside a browser. Because every browser has such thing called, 'JavaScript Engine', which converts a JavaScript code into another code that the computer understands.
So bascially, all browsers uses JavaScript in order to create a function inside a browser like Internet Explorer, Firefox, or Google Chrome, and they each have 'JavaScript Engine' of their own.
For example, the JavaScript Engine of Internet Explorer is **Chakra**, Firefox **SpiderMonkey**, and Google Chrome **v8**.

However in 2009, a software engineer named **Ryan Dahl** thought it would be better to run JavaScript not just inside a browser. Thus created Node.js. He used Google Chrome's **v8** and embedded it into a C++ program to make a Node.exe.

Here comes the confusing part. The general flow of the system is very similar to that of a browser.
![image](https://miro.medium.com/max/560/1*zeKjWCjyAGZ9JN4fvnWsiA.png)

In the core of a browser, there is a JavaScript Engine. And surrounding it is a 'runtime environment' that includes APIs that are needed in order to build a program AND the JavaScript Engine that decodes human's codes into a computer's code. So 'runtime environment' is a container that stores all that is needed to create a program.

Now, what is the difference between a browser and Node?

Node also is a runtime environment for JavaScript codes. It contains a JavaScript Engine that can execute our JS code and certain objects that provide an environment for our JS code. And these objects are different from environment objects in browsers.
For example, in a browser, we can only do certain actions within a document, or the window, of the browser such as: ```document.getElementById('');```.
However in Node.js, there are much more modules that gives us more options to work around with file system, ```fs.readFile()```, or listen for requests on a given port, ```http.createServer()``` and so on.

To recap,
Node is a runtime environment that includes the **v8** JavaScript Engine AND modules that are not available in a browser.
Both Google Chrome and Node.js share the same JavaScript Engine, but they provide different runtime environments for JavaScript.


Thanks for reading my post, and please let me know if there is anything I should correct! :)