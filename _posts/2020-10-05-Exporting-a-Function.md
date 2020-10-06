---
layout: post
title:  "Exporting a Function"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/23.jpg
---

Let's say you created a function in a Node.js file, or module as we learned in the last post. You might want to use that function in a different module.
In this case, you will have to **export** the function that is scoped to the module that it was created in, to the outside of that module.

In Node.js there are some default modules. So if you console.log(module), you will be able to see these default elements as a JSON object.
In this JSON object, there is a **key** named "exports" which has an empty object, which is the default **value**. And as you can tell from the name of the key, anything that is added to this object will be "exported" from the module, so that this "anything" can be used outside of the module.

However, there is one thing to keep in mind.

You should export just a part of the module, and not EVERY functions in the file. There is no use of dividing into modules if you are to export everything out of it. Also, by keeping the functions inside a module, it is possible to store valuable datas in one spot.
Think of a cell phone for example. There are some buttons in the exterior which the clients can use. This is called **Public Interface**. But on the inside, there are much more functions that the clients do not necessarily need to know. And this is called **Implementation Detail**.