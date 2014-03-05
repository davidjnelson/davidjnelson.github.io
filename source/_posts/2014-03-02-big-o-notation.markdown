---
layout: post
title: "Big O Notation"
date: 2014-03-02 18:52
comments: true
categories: computer-science-fundamentals
---

Big O Notation is a way to measure how well a computer algorithm scales as the amount of data involved increases.  I will use the javascript programming language throughout this series for the code examples.

O(1)
----

O(1) is read as &quot;order of one&quot;, or &quot;constant time&quot; and means that this algorithm will scale infinitely well regardless of the input size.  An example of an operation that runs in constant time is that of adding an element to an array that does not require the array to be resized:

```
  var theArray = new Array(1);
  theArray[0] = 'Hello!';
```

Note that since we initialized the array to only have a length of 1, if we were to insert a second element into the array it would have to resize, and so inserts to this array would no longer be guaranteed to run in constant time.  This is somewhat specific to the particular javascript vm you are using, but in general you will get amortized constant time [5] for array inserts in javascript [4].



Resources For Additional Learning:
----------------------------------
1. (Derek Banas, Big O Notations Youtube Video)[http://www.youtube.com/watch?v=V6mKVRU1evU]
2. (Big-O complexities of common algorithms used in Computer Science)[http://bigocheatsheet.com/]
3. (Stanford University, Algorithms: Design and Analysis, Part 1 Coursera Course)[https://www.coursera.org/course/algo]
4. (Big O of Javascript Arrays)[http://stackoverflow.com/questions/11514308/big-o-of-javascript-arrays]
5. (Constant Amortized Time) [http://stackoverflow.com/questions/200384/constant-amortized-time]
