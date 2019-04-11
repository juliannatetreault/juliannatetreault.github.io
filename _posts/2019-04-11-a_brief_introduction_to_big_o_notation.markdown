---
layout: post
title:      "A Brief Introduction to Big O Notation"
date:       2019-04-11 20:59:15 +0000
permalink:  a_brief_introduction_to_big_o_notation
---


### What is Big O?

Big O notation, otherwise known as just *Big O,* is a concept in computer science that expresses an algorithm’s runtime—it is a way of calculating just how long any one algorithm or function will take to run. One important thing to note is that Big O not only calculates an algorithm’s runtime, but it is also used to calculate just how quickly that runtime will grow as the inputs – expressed as `n` in Big O notation – themselves grow.

### Why use Big O?

While understanding Big O can be challenging, understanding why it’s important to use Big O is crucial. *So, why use it?* Big O is an essential part in designing and scaling—it is an extremely important concept to keep in mind when thinking about efficiency or scalability for a given algorithm. Big O allows developers to optimize their algorithms to fit their needs. It aids in a developers ability to analyze, allowing them to choose between algorithms in pragmatic way: `“Is algorithm A or B faster?”` 

#### Planning for the worst case

When it comes to choosing the appropriate time complexity route to take, choosing the worst-case scenario is *always* advised. While this may sound counterintuitive, once broken down, planning for the worst case makes perfect sense. 

#### Best-Case Complexity

Calculating the best-case complexity can be done by figuring out the fewest number of steps that an algorithm or function can perform at. While calculating the best-case complexity might seem like the most appropriate thing to do, it is advised against. In calculating the best-case, we don’t take into account any issues our runtime may encounter and instead settle for the fastest length of time to get through an algorithm, leaving out important edge case considerations.

#### Average-Case Complexity

Calculating average-case complexity is similar to the best-case complexity approach. The average-case can be found by calculating the time complexity of an algorithm. To do so, one must take the sum of all of the algorithm’s inputs and then find the average of that. Overall, average-case complexity is difficult to calculate and neglects to take important runtime issues into consideration, making it unreliable and again, not the ideal choice.  

#### Worst-Case Complexity

So, if best-case complexity and average-case complexity are not ideal, then worst-case complexity must be the way to go, *correct*? Correct! Worst-case complexity is calculated by finding the longest possible runtime and most resources necessary for an algorithm to perform. The benefit of calculating the worst-case scenario for an algorithm or function is that is gives developers insight as to what it would be like if *the algorithm was performing in the worst possible way*. Figuring out what the worst-case scenario is for any given algorithm allows developers to build and scale with this in mind. Ultimately, this allows developers to plan and optimize for the worst, while building the best. 

### Recap 

Big O notation is a useful way of approaching complex algorithmic problems. Thinking in terms of Big O allows developers to plan for the worst possible scenario when designing or scaling, which can ultimately lead to smoother performance and better runtimes. While Big O is a tough concept to grasp, it is important to understand to take your development skills to the next level.

