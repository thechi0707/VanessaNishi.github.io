---
layout: project
type: project
image: img/bank.jpeg
title: "Bank Database Project"
date: 2023
published: true
labels:
  - C
  - C++
summary: "A simple bank database which allows a user to add, delete, find, and print records of accounts. Created as a final project for my ICS212 class."
---

Last semester for my ICS 212 class, our major project was to create a simple bank database that stores records of accounts in descending order of account number. Each record consists of the account number and the name and address of the account holder.
It additionally allows the user to add, find or delete a record or print all the records. The program was originally written in C and converted into C++ later.

The process to building it was to write out the each of the functions in pseudocode to ensure to logic was correct and then write it out in C code. 
It required a good understanding of pointers, linked lists, writing in and out of files, allocating memory in the heap space, as well as basic C coding conventions. 
One of the most important tasks was ensuring a record was added in the correct spot, so as to maintain the descending order of the account numbers.
This involved traversing the linked list with various pointers in order to find the right place. 
