---
layout: normal
title: SRM 2014 Web developers
published: true
permalink: srm/
description: Codebrahma SRM Questions
---

<div id="questions" class="unit whole" markdown="1">

## Instructions

1. You have 90 minutes time.   
2. Each question has a fiddle associated to it, fork the fiddle and implement the solution on the browser and save your answer. Call one of the Codebrahma team members and get your output verified. 
3. There are infinite ways to solve these problems. If two people submit identical solutions, both of them will be rejected.
4. If the student is not comfortable with Javascript, he/she can use codepad.org and solve it any preferred language. 
5. __Note__: The last question needs to be solved only in Javascript and has bonus marks
6. Submit your responses by filling this [form](https://docs.google.com/forms/d/1JpRK77gVfDJQxmfcNkA-4gq3LVRc53PQMEjlJsENp_g/viewform).

***

## 1. Multiples of 3 and 5

If we list all the natural numbers below 16 that are multiples of 3 or 5 and not multiples of 3 and 5, we get 3, 5, 6 and 9, 10, 12 (__not 15 as it's a multiple of both 3 and 5__). The sum of these multiples is 45.

Write a function which takes in a number n, and returns the sum of all numbers below n which are multiples of  3 or 5, but not 3 and 5.

[JS Fiddle](http://jsfiddle.net/u50pxyka/)

***

## 2. Regular Expressions

Regular expressions are used extensively across programming languages for string/pattern matching.

Write a function which takes in 2 strings, pattern and query, and returns boolean value which indicates whether the query matches the pattern.

Please dont use built in regex functions or third party code.

Possible query patterns.

1. (*) —> 0 or many repetitions
2. (\|) —> OR
3. (?) —> 0 or 1 repetitions


Example:

{% highlight javascript %}
function("ab*", "ab"){} // should return true
function("ab*", "abbbbb"){} // should return true
function("ab*c*d?e", "abbbbccccce"){} // should return true
function("ab*", "abba"){} // should return false

function("ab|ba", "ab"){} // should return true
function("ab|ba", "ba"){} // should return true

function("ab?", "a"){} // should return true
function("ab?", "abb"){} // should return false

function("nith?in", "nitin"){} // should return true
{% endhighlight %}

[JS Fiddle](http://jsfiddle.net/7jasysfa/)


***

## 3. The Button Game

Observe the following video carefully and implement the functionality in the given [fiddle](http://jsfiddle.net/fdzLaqku/).

The text box takes in a integer "n". Once you press the submit button. "n" buttons, ranging from 1 to n are created. When you click on one of those n buttons. The numbers are shifted to the right.

<iframe src="//player.vimeo.com/video/103901971" width="500" height="375" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe> <p><a href="http://vimeo.com/103901971">Button Game</a> from <a href="http://vimeo.com/user19541206">CodeBrahma</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

In case the video isn't working refer [this](/images/srm puzzle.gif).


[JS Fiddle](http://jsfiddle.net/fdzLaqku/)

</div>

<style type="text/css">
.main-nav {
  visibility: hidden;  
}
#questions img {
  height:400px;  
  width:500px;
}
</style>




