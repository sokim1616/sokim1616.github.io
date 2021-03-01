---
layout: post
title:  "Module Wrapper Function"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/24.jpg
---

It's been a while since I updated my blog.
I once again realized that having a break for a long period of time requires more time and effort to catch up.

So today, I'm going to define what the **Module Wrapper Function** is.
In the previous post, we learned that variables and functions that we define in a module, are scoped to THAT module. They are private, and NOT visible from the outside.

But HOW does node do this? This is where the **Module Wrapper Function** comes in.

Everything that you write on a javascript file is wrapped around an invisible function in the form of:
```
function (exports, require, module, __filename, __dirname) {}
```

In other words, node does not directly read and execute the code that you write; it wraps your code around another function that it can translate better.