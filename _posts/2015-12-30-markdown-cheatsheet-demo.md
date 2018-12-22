---
layout: post
title: "Graph-Based Semi Supervised Learning"
comments: true
description: "Markdown Cheatsheet Demo..."
keywords: "markdown, typography components, dummy content"
---

시작에 앞서, 고려대학교 강필성 교수님의 강의 및 자료를 바탕으로 정리하였음을 밝힙니다.
이번 포스팅에선 Graph-Based Semi Supervised Learning에 대해서 살펴보도록 하겠습니다. 

<div class="divider"></div>



## SSL이란?

![SL_USL_SSL](http://log0629.github.com/images/SL_USL_SSL.png)


## Headings H1 to H6

# H1 Heading

## H2 Heading

### H3 Heading

#### H4 Heading

##### H5 Heading

###### H6 Heading

<div class="divider"></div>

## 이수빈 개똥쟁이 메렁메렁메렁 

Let's say you have text that you want to refer with a footnote, you can do that too! This is an example for the footnote number one [[^1]]. You can even add more footnotes, with link! [[^2]]

<div class="divider"></div>

## Blockquote

> Start by doing what's necessary; then do what's possible; and suddenly you are doing the impossible. --Francis of Assisi

**NOTE:** This theme does NOT support nested blockquotes.

<div class="divider"></div>

## List Items

1. First order list item
2. Second item

* Unordered list can use asterisks
- Or minuses
+ Or pluses

<div class="divider"></div>

## Code Blocks

```javascript
var modularpattern = (function() {
    // your module code goes here
    var sum = 0 ;

    return {
        add:function() {
            sum = sum + 1;
            return sum;
        },
        reset:function() {
            return sum = 0;    
        }  
    }   
}());
alert(modularpattern.add());    // alerts: 1
alert(modularpattern.add());    // alerts: 2
alert(modularpattern.reset());  // alerts: 0
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting.
But let's throw in a <b>tag</b>.
```

<div class="divider"></div>

## Table

### Table 1: With Alignment

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

### Table 2: With Typography Elements

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

<div class="divider"></div>

## Horizontal Line

The HTML `<hr>` element is for creating a "thematic break" between paragraph-level elements. In markdown, you can create a `<hr>` with any of the following:

* `___`: three consecutive underscores
* `---`: three consecutive dashes
* `***`: three consecutive asterisks

renders to:

___

---

***

<div class="divider"></div>

## Media

### YouTube Embedded Iframe

<div class="video-container"><iframe src="https://www.youtube.com/embed/n1a7o44WxNo" frameborder="0" allowfullscreen></iframe></div>

### Image

![Minion](http://octodex.github.com/images/minion.png)

---
Footnote:

[^1]: 1: Footnote number one yeah baby!

[^2]: 2: A footnote you can link to - [click here!](#)
