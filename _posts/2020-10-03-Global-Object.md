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
    <li>setTimeout()</li>
    <li>clearTimeout()</li>
    <li>setInterval()</li>
    <li>clearInterval()</li>
</ul>
