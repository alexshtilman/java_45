# java_45 Deadlock task "The Dining Philosophers"

Task – Resolve the Deadlock in class Philosophers

## The history of the problem:

The Dining Philosophers problem is one of the classic problems used to describe synchronization issues 
in a multi-threaded environment and illustrate techniques for solving them. 

Dijkstra first formulated this problem and presented it regarding computers accessing tape drive peripherals.
The present formulation was given by Tony Hoare, who is also known for inventing the quicksort sorting algorithm.

## The Problem:

- There are five silent philosophers (P1 – P5) sitting around a circular table, 
  spending their lives eating and thinking.
- There are five forks for them to share (1 – 5) and to be able to eat, 
  a philosopher needs to have forks in both his hands. 
- After eating, he puts both of them down and then they can be picked 
  by another philosophers who repeats the same cycle.
- The goal is to come up with a scheme/protocol that helps the philosophers achieve their goal of eating
  and thinking without getting starved to death.

## Explanation of the problem in source code:

We can get to situation, when each of the Philosophers has acquired his left fork,
but can’t acquire his right fork, because his neighbor has already acquired it. 
This situation is commonly known as the Circular Wait and is one of the  
conditions that results in a Deadlock and prevents the progress of the system.
