---
layout: post
title: "Review of Coursera's Functional Programming Principles in Scala"
date: 2014-06-30 09:32:09 -0500
comments: true
categories: 
---

In case you’ve been asleep, functional programming is the new standard in modern programming language and application design. To those of us who have been using languages with functional features, such as Ruby, C# and JavaScript, it doesn’t seem at first glance like a major paradigm shift. This is especially true since functional design is not mutually exclusive to object-oriented design (in fact as the Scala language proves, they complement each other quite nicely). However when you apply functional principles universally using a functional language, it becomes clear that FP is a significant step forward from the Java-style object-heavy approach that it is slowly replacing.  
I signed up for Functional Programming Principles in Scala on Coursera to experience for myself the new secret sauce having heard that the course is outstanding. I’m happy to say that it was outstanding beyond my expectations. It’s a perfectly designed introduction and easily the most rewarding online class I’ve ever taken.  
Perhaps it shouldn’t be a surprise that the course is so good. It’s taught by Scala’s creator, Martin Odersky. What *is* surprising is that throughout the course, he talks very little about functional programming principles at a high level. Instead he teaches by example starting with simple recursive algorithm problems and ending with a really clever algorithmic game solver. In between we solved some classic computer science problems - problems I had solved before in school - using pure FP in a way that highlights where the functional solutions improve on the older procedural solutions. It’s in the progression of increasingly more involved assignments - which stepwise introduce language features and concepts - that the class succeeds so cleverly. One is never instructed to use pure functional programming, but rather arrives there naturally as one technique begets the next and the assignments grow in complexity. If you’re autodidactic like me, and generally wary of formal education, you’ll appreciate Professor Odersky’s subtle approach.  
  
So what did I learn?

*   Recursion combined with immutable linked lists is the best way to do list operations
*   Pattern matching is the hottest language feature since lambdas. They’re super-charged conditionals
*   Lazy sequences and lazy evaluation are a breeze when they’re built into the language
*   Often when I’m using a list, I should be using a set
*   Tuples do serve a purpose when your language is strongly typed
*   You can have strong typing without excessive boilerplate
*   Tail call optimization makes a language more powerful (I’m looking at you, Ruby)
*   Accessing instance variables from within methods is safe if they’re immutable
*   Encapsulation with higher-order functions is cleaner than delegation
*   Side-effect free code weakens the case for test doubles  

Whether you have or have not been exposed to functional programming, this is a great course. If you’ve ever studied recursive algorithms and enjoyed it, this course will rekindle your excitement by giving you new more powerful ways to solve old problems. Be prepared to fall in love with the Scala language: it fixes most of what’s wrong with Java and augments it with new capabilities that lead to simply better code. While it is not addressed in this course, I’m looking forward to seeing how functional programming improves concurrent operations in distributed environments. Fortunately that’s the subject of Dr. Odersky's [next class](https://www.coursera.org/course/reactive) which you can bet I’ll be taking.

