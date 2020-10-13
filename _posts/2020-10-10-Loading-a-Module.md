---
layout: post
title:  "Loading a Module"
author: So Hyun K.
categories: [ TIL ]
image: assets/images/23.jpg
---

Today, I'm going to talk about loading a module.

In order to load a module, **require function** is needed. Require function is specified only to Node.js, which means that browsers do not.
The **require function** takes one argument: the path/name of the target module that you want to bring outside of the file.
To write the path of a target module, there are several rules to follow:
<ol>
    <li>"./(file name)" indicates the current folder</li>
    <li>"../(file name)" indicates the parent folder</li>
    <li>"./(subfolder name)/(file name)" if the target module is in a sub-folder</li>
</ol>

So for example, if you want to export a module named "starter.js", you need to export it by writing:
```
module.exports.starter = starter;
```
in "starter.js" file.

And also, write:
```
require('./starter');
```
in the file that you want to use this module. (For example, in "app.js")

The **require function** returns the object that is exported from this target module.


Oh! And in case you want to export just a single function, instead of the whole module, you can change the module.exports to:
```
module.exports = (function name)
```


Initially, the module was exporting an empty object, but by doing so it is reset to just a function.
