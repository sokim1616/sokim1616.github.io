---
layout: post
title:  "How Node.js Works - 02"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/19.jpg
---

When you create a new file for example called **app.js**, and write a function that prints a greeting, you can see it printing on the terminal that you run the file.
For instance, think of below as a function in **app.js** file:
```
function greetSomeone(name) {
    console.log("Hello" + name);
}
greetSomeone('Kim')
```

When you run this file in a terminal like so:
```
$node app.js
```
you can see
```
Hello Kim
```
on the terminal.

This is because Node.js is a program that runs in Google Chrome's JavaScript engine, **v8**. When the **app.js** file gets passed to Node.js, the Node.js then passes the file to **v8** in order for the function in the file to be processed, which prints it out on the terminal as a result.

However, if you try to console.log(window) (note that window is working as a variable, and NOT in a string type), the terminal will show:
```
window is undefined
```

Again, this is because in Node.js, there is no such thing as **window**, or **document objects** like browsers do.
There are other objects in Node.js that work with files, operating system, network, and so on, which I will write about in the next post.


Thanks for reading and please let me know if there's any errors! :)