---
layout: article
title: An introduction to partitions.
mathjax: true
---
### What is a partition?
In its simplest terms, a partition is an ordered collection of positive integers, and each of those integers is called a part.  We order the parts from largest to smallest.  Mathematically, we define them like this: A partition is a multiset $$\lambda = (\lambda_1, \lambda_2, \dots, \lambda_r)$$, where $$\lambda_i \geq \lambda_{i+1}$$, for $$i \in \lbrack 1,r-1 \rbrack$$.

A useful way of thinking about partitions is as rows of boxes, starting with the first part.  This is called a Young Diagram.  Drawing  partitions as Young Diagrams opens up all sorts of mathematical questions.  You can have a go at building your own partitions below.  Enter positive integers in descending order, separated by a comma, then press 'Draw' to see your partition.

[//]: <> (Essentially, you can think of a partition is rows of boxes stacked on top of each other.  The rule is that a row cannot stick out below another one, or more mathematically speaking, the $$i^{th}$$ row is greater than or equal to the $$(i+1)^{th}$$ row.)  

[//]: <> (This is also a comment.)

<iframe style="width: 520px; height: 460px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/zEYjhDenP"></iframe>


### Conjugation
Every partition has a partner, called its conjugation.  We denote the conjugation of a partition $$\lambda$$ as $$\lambda^{\ast}$$. To conjugate a partition, we swap the rows and columns.  For example, we can see that the conjugation of (6,4,4,1,1) is (5,3,3,3,1,1), as shown in the image below.

[//]: <> (Make the image)

Add the flip it sketch

<iframe style="width: 620px; height: 420px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/e2ZrTT-TO" src="https://editor.p5js.org/klee26/full/IZhnc_BWJ"></iframe> 

Explain how to conjugate without looking at Young Diagrams.


<iframe style="width: 600px; height: 600px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/e2ZrTT-TO"></iframe>
