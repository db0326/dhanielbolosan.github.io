---
layout: essay
type: essay
title: "Frustrations to Solutions"
# All dates must be YYYY-MM-DD format!
date: 2024-09-12
published: true
labels:
  - Smart Questions
---

## Finding Smart Solutions

We’ve all had those moments where we find ourselves stuck on a problem and turn to the internet for help. Whether it be debugging a program, fixing your car, or learning how to cook a new dish, seeking assistance from online resources has become common in the modern world. Websites such as Quora, Reddit, and StackOverflow are a few examples of online resources that many people go to when they are stuck with certain situations. While these websites are excellent for finding help, the quality of answers can vary and often depends on how well the question is asked. According to [Eric Raymond’s guidelines](http://www.catb.org/esr/faqs/smart-questions.html#stackoverflow), a smart question is a question that is well-researched, clearly articulated, and provides relevant details.

## StackOverflow Success

An example of a smart question that follows the guidelines of Eric Raymond can be found on a StackOverflow post titled “[Javascript By Reference vs. By Value](https://stackoverflow.com/questions/6605640/javascript-by-reference-vs-by-value)”. While the original poster doesn’t necessarily ask a question, they clearly show an invested effort in researching the topic, are well articulated, and provide relevant examples to help with their confusion. The poster presents examples such as:

```
function f(a,b,c) {
  a = 3;
  b.push("foo");
  c.first = false;
}

var x = 4;
var y = ["eeny", "miny", "mo"];
var z = {first: true};
f(x,y,z);
```

and also ...

```
function f() {
  var a = ["1", "2", "3"];
  var b = a[1];
  a[1] = "4";
}

function f () {
  var a = [{yellow: "blue"}, {red: "cyan"}, {green: "magenta"}];
  var b = a[1];
  a[1].red = "tan";
  b.red = "black";
}
```

By providing these examples, the poster demonstrates a desire to get a better understanding of pass by reference versus pass by value in Javascript rather than looking for a surface level answer. Furthermore, the answers they received reflect upon the quality of his smart question as they provide a clear answer to his confusion

## Ask and Fail

An example of a not-so-smart question can be found on another StackOverflow post where the original poster asks the question, “[What’s the difference between JavaScript and Java?](https://stackoverflow.com/questions/245062/whats-the-difference-between-javascript-and-java)” Although this question may be a good question to ask for a beginner programmer, the manner in which the question was asked leaves much to be desired. The post simply copied and pasted the title as the question itself with the tags “java” and “javascript". This shows a lack of effort in researching the topic and fails to provide any context or examples. Consequently, the quality of responses reflects on the quality of this question. For example, the top voted answer sarcastically states, “Java and Javascript are similar like Car and Carpet are similar.”

<p align="center">
  <img src="../img/smart-questions/not-so-smart-question.png" width="500px">
</p>
