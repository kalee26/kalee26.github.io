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
Every partition has a partner, called its conjugate.  We denote the conjugate of a partition $$\lambda$$ as $$\lambda^{\ast}$$. To find the conjugate of a partition, we swap the rows and columns.  For example, we can see that the conjugate of (7,5,3,1,1) is (5,3,3,2,2,1,1), as shown in the image below.

<iframe style="width: 470px; height: 280px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/e2ZrTT-TO" src="https://editor.p5js.org/klee26/full/IZhnc_BWJ"></iframe> 

You can find the conjugate of a partition without drawing out the Young diagram. Look at your partition $$\lambda = (\lambda_1, \dots, \lambda_r)$$ and for each $$i \in \lbrack 1,\lambda_1 \rbrack$$, count the number of parts in $$\lambda$$ which are greater than or equal to $$i$$.

For example, take the partition $$(5,3,2,2,2)$$.  There are 5 parts greater than or equal to 1, 5 parts greater than or equal to 2, 2 parts greater than or equal to 3, 1 part greater than or equal to 4, and 1 part greater than or equal to 5.  Thus the conjugate of $$\lambda$$ is $$\lambda^{\ast} = (5,5,2,1,1).$$

You can test your understanding by choosing your own partitions to conjugate using the interactive sketch below.  Click 'Flip it' to see the conjugated partition.
<iframe style="width: 470px; height: 280px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/pFiieeQ9h"></iframe>

### Adding and removing boxes

One thing we can look at with partitions is the conditions for adding or removing boxes.  What if we want to add (or remove) a box in such a way that the result is a valid partition?

Suppose $$\lambda$$ is a partition of $$n$$, and $$\lambda^{\prime}$$ a partition of $$n+1$$ obtained by adding 1 to one of the parts of $$\lambda$$, or by adding a new part of value 1.  (For some $$n \in \mathbb{N}$$.) We call $$\lambda$$ the *parent* of $$\lambda^{\prime}$$, and we call $$\lambda^{\prime}$$ the *child* of $$\lambda$$.

Proposition:
Let $$\lambda$$ be a partition of $$n$$ with parts of $$w$$ different values.  Then $$\lambda$$ has $$w+1$$ children. (For some $$n \in \mathbb{N}$$.)

Proof:
Group together the parts of $$\lambda$$ which have the same value. We need to add $$1$$ to one of the parts.  The only possibilities of doing this and maintaining the convention of descending parts is to add $$1$$ to the first element of the group of parts with the same value, or to add another part of value $$1$$. There are $$w$$ groups, so the number of possibilities is $$w+1$$.  Hence $$\lambda$$ has $$w+1$$ children.

Proposition:
Let $$\lambda$$ be a partition of $$n$$ with parts of $$w$$ different values. Then $$\lambda$$ has $$w$$ parents. (For some $$n \in \mathbb{N}$$.)

Proof:
We know that 1 has been added to one of the parts of $$\lambda$$, or a part of value 1 has been added.  Again, group the parts into parts of the same value.  The only place 1 could have been added within each group is the last element of each group (because we write partitions in descending order).  It follows that $$\lambda$$ has $$w$$ parents.

Corollary: The number of addable boxes of a partition is 1 greater than the number of deletable boxes

<iframe style="width: 600px; height: 600px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/b0JLnIhW0"></iframe>

<iframe style="width: 600px; height: 600px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/e1ISiOZA7"></iframe>

<iframe style="width: 600px; height: 600px; overflow: hidden;"  scrolling="no" frameborder="0" src="https://editor.p5js.org/klee26/full/e2ZrTT-TO"></iframe>
