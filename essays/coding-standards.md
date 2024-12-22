---
layout: essay
type: essay
title: "Setting the Standard"
# All dates must be YYYY-MM-DD format!
date: 2024-09-26
published: false
labels:
  - Coding Standards
---

## Rules and Regulations

At first glance, coding standards might seem like a bunch of unnecessary nitpicky rules about things like indentation and using single quotation marks... and honestly, it kinda feels like that. I understand that coding standards help programmers write more efficient, readable, and cleaner code, but I can't help but feel that following strict coding standards takes away the individuality in coding. Personally, I have my own way of writing code, but when using tools like ESLint, I often have to adjust the way I write my code. For example, here are some code snippets that reflect my personal style:

```
// Snippet 1:
const word: string = "hello";

function numWord(arr: string[]): number{
  return arr.map((str) => (str.toLowerCase().includes(word) ? 1 : 0)).reduce((total: number, item: number) => total + item, 0);
}

// Snippet 2:
class Menu{
  menuItems: menuItem[] = [];

  addMenuItem(item: menuItem){
    this.menuItems.push(item);
  }

  findMenuItem(ingredient: string){
    const foundArr = [];
    for(const item of this.menuItems){
      if(item.ingredients.includes(ingredient)){
        foundArr.push(item);
      }
    }
    return foundArr;
  }
}
```

Here is how ESLint would suggest I should rewrite it:

```
// Snippet 1:
const word: string = 'hello';

function numWord(arr: string[]): number {
  return arr
    .map((str) => (str.toLowerCase().includes(word) ? 1 : 0))
    .reduce((total: number, item: number) => total + item, 0);
}

// Snippet 2:
class Menu {
  menuItems: menuItem[] = [];

  addMenuItem(item: menuItem) {
    this.menuItems.push(item);
  }

  findMenuItem(ingredient: string) {
    const foundArr = [];
    for (const item of this.menuItems) {
      if (item.ingredients.includes(ingredient)) {
        foundArr.push(item);
      }
    }
    return foundArr;
  }
}
```

## Getting the Lint Off

In the recent weeks in my ICS 314 class, we've been using ESLint with Visual Studio Code. I've been using Visual Studio Code for the past two years since I have started studying computer science, but this is the first time using ESLint. Although I did somewhat complain about coding standards earlier, I actually don't mind complying with them. It can be a bit tedious at times, especially when it disrupts my usual coding flow, but I can appreciate how it helps me improve my coding practices.
