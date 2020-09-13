---
layout: post
title:  "Github Blog Error Fix"
author: So Hyun K.
categories: [ Dev Diary ]
image: assets/images/12.jpg
---

It has been so long since I updated the logs of my blog.
At one point, the posts that I have written would not load on the actual blog page. So I have been fixing codes of all different sorts of files.
Since using **Github** as a blog is not really something that I was used to, I was struggling to fix this error for, believe it or not, more than a couple weeks! XD

These are the list of things that I've tried:
<ul>
    <li>
    Putting spaces in between colon(:) and the actual content in the settings
    </li>
    <li>
    Renaming the files just in case there was a structure error
    </li>
    <li>
    Fixing so many things in the '_config.yml' file just in case
    </li>
    <li>
    Googling about this same issue which I couldn't find..
    </li>
</ul>

But then, I realized I wasn't aware of the easiest way to find the error..!
Since the commit records has been updating (even though it didn't show on the blog) I looked through them and saw since when did the error occur.
And after find it, I compared which file had the first error.
When I just simply deleted the line which was added after the commit that was successfully shown on the blog, all my posts have magically appeared on the blog instantly.

So the message that I wanted to give today was,
> When there is an error, look at the commit record!
> Think simply!

I hope there is not someone out there making the same simple mistake that I have made!