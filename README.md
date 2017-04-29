# CSS Tutorial

## 1, CSS Introduction

What is *CSS*?
* CSS stands for Cascading Style Sheets
* CSS describes how HTML elements are to be displayed on screen, paper, or in other media
* CSS saves a lot of work. It can control the layout of multiple web pages all at once
* External stylesheets are stored in CSS files

## 2, CSS Syntax and Selectors
A CSS rule-set consists of a selector and a declaration block:

![css syntax](https://www.w3schools.com/css/selector.gif)

* The element selector
```css
p {
     text-align: center;
     color: red;
 }
 ```
* The id selector
```css
#para1 {
    text-align: center;
    color: red;
}
```
* The class selector
```css
.center {
    text-align: center;
    color: red;
}
```

## 3, Hot to insert css?
### 3.1 Three ways to insert css
>* External style sheet
```html
<link rel="stylesheet" type="text/css" href="mystyle.css">
```
>* Internal style sheet
```html
<head>
<style>
body {
    background-color: linen;
}
</style>
</head>
```
>* Inline style
```html
<h1 style="color:blue;margin-left:30px;">This is a heading</h1>
Try it Yourself »
```

### 3.2 Cascading Order
What style will be used when there is more than one style specified for an HTML element?

Generally speaking we can say that all the styles will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

-[x] Inline style (inside an HTML element)
-[x] External and internal style sheets (in the head section)
-[x]  Browser default

So, an inline style (inside a specific HTML element) has the highest priority, which means that it will override a style defined inside the <head> tag, or in an external style sheet, or a browser default value.