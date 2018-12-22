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



## Semi-Supervised Learning

![SL_USL_SSL](http://log0629.github.io/assets/images/SL_USL_SSL.png)


Graph-Based Semi Supervised Learning에 대해 살펴보기에 앞서, Semi Supervised Learning에 대해 간단히 알아보겠습니다. 데이터를 다루는 대부분의 사람들은 Supervised Learning과 Unsupervised Learning에 대해서 주로 배우게 됩니다. Supervised Learning은 레이블(Y)이 있는 데이터셋을 활용한 학습 방법인 반면 Unsupervised Learning은 레이블이 없는 데이터셋을 활용한 학습 방법으로, 모델 스스로가 학습하는 것을 의미합니다. 
Semi Supervised Learning의 경우 위의 두 학습 방법을 병합한 것으로, 레이블이 달려있는 데이터와 레이블이 달려있지 않은 데이터를 동시에 활용하는 것입니다.

이제 본격적으로 Graph-Based Semi Supervised Learning에 대해 알아보겠습니다.



## Graph-Based Semi Supervised Learning

Graph-Based SSL(이하 GSSL)은 그래프에 의해 나타내어지는 데이터셋들에 대해 사용됩니다. 대표적으로 Social Network를 꼽을 수 있습니다. 그리고 각 요소들의 형태가 동일하지 않은 이질 데이터형을 표현하기 위해 쓰이기도 합니다. 여기서 GSSL은 다음과 같은 가정이 필요합니다.

 1.	그래프는 Semi Supervised Learning에 사용되는 데이터에 기반합니다. 

 2.	Heavy edge에 의해 연결된 노드들은 같은 라벨을 지니려고 합니다.


# Graph construction

다음 세 가지 방법으로 그래프의 Edge를 정하게 됩니다.

1) k-Nearest-Neighbor Graph 
k-Nearest-Neighbor Graph는 하나의 노드와 이 노드의 k-nearest neighbors 사이에 edge를 연결시킵니다. 

![KNNG](http://log0629.github.io/assets/images/KNNG.png)

2) Fully Connected Graph
Fully Connected Graph는 하나의 노드를 기점으로 모든 노드를 연결하는 것을 의미합니다.

![FCG](http://log0629.github.io/assets/images/FCG.png)

3) ε-Radius Graph
ε-Radius Graph는 하나의 노드를 기점으로 e radius의 구를 생성하여 그 안에 있는 노드들에 edge를 연결시킵니다.

![ERG](http://log0629.github.io/assets/images/ERG.png)


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
