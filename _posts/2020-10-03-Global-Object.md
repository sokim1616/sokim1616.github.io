---
layout: post
title:  "Global Object"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/19.jpg
---

Did you know that the ```console.log``` that you write to check what is happening at that particular moment, is actually a global object?
When you use ```console.log()```, it means that you want to check the **log** of the **console** object. Since you can write this code anywhere in a Node.js file, it is said to be in a **global scope**, so we can access it from anywhere in any file.

Other than ```console.log```, below are other examples of global objects:
<ul>
    <li>setTimeout(): used to call a function after a delay of a given time</li>
    <li>clearTimeout(): used to stop calling that function</li>
    <li>setInterval(): used to keep calling a function after a given delay</li>
    <li>clearInterval(): used to stop that function from being called</li>
</ul>

These functions above can be used in the window of a browser. In other words the window objects in browsers, are also in the global scope, and all variables and functions that are defined globally can be accessed via window object.

However, when a variable is declared in **app.js**, it is NOT added in the global object, because that variable is scoped ONLY to the **app.js** file that it was called in.


In the next post, I will explain about this **scope** concept, called **module** in more detail.
Let me know if there is any errors! :)