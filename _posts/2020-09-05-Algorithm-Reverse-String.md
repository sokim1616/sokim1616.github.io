---
layout: post
title:  "Algorithm: Reverse String"
author: So Hyun K.
date: 2020-09-05
categories: [ Algorithm ]
tags: [ Algorithm ]
image: "https://images.unsplash.com/photo-1559925393-8be0ec4767c8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1351&q=80"
---

Today's algorithm problem was called **Reverse String** from ***leetcode***.
The title of the problem is pretty straight-forward, but the main goal is to reverse a given string.

For example, a given string "Hello" has to be returned as "olleH".

This was the code that I had to start with:
```
var reverseString = function(s) {

}
```
where 's' is the given string.

I have tried this problem with the code below:
```
var reverseString = function(s) {
    
     let result = [];
    
     for (let i = 0; i < s.length; i++) {
         console.log("s[i]", s[i])
         result.unshift(s[i])
     }
     console.log("result", result) // [ 'o', 'l', 'l', 'e', 'h' ]
     return result; // ["h","e","l","l","o"]
```

I wanted to try to solve this provlem using bubble sort at first, but then after 30 minutes of trial, I found out that there is a perfect method to use in cases like this: reverse()...

So basically, all I needed to do was
```
var reverseString = function(s) {
    s.reverse()
}
```
and then it would automatically reverse the order of the string 's'!