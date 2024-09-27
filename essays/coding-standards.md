---
layout: essay
type: essay
title: "Setting the Standard"
# All dates must be YYYY-MM-DD format!
date: 2024-09-26
published: true
labels:
  - Coding Standards
---

## Rules and Regulations

At first glance, coding standards might seem like a bunch of unecessary nitpicky rules about indentation and using single quotation marks... and honestly, it definitely feels like that. While I recognize that coding standards help programmers write more efficient, readable, and cleaner code, I can't help but feel that following strict coding standards takes away the individuality in coding. Personally, I have my own way of writing code, but when using tools like ESLint, I often have to adjust the way I write my code. For example, here are some code snippets that reflect my personal style:

```
// Snippet 1:
const word: string = "hello";

function numWord(arr: string[]): number{
  return arr.map((str) => (str.toLowerCase().includes(word) ? 1 : 0)).reduce((total: number, item: number) => total + item, 0);
}

// Snippet 2:
class Menu{
  menuItems: menuItem[] = [];

  addMenuItem(item: menuItem): void{
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

  addMenuItem(item: menuItem): void {
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
