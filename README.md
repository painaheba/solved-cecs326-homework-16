Download Link: https://assignmentchef.com/product/solved-cecs326-homework-16
<br>
Purpose: Gain experience with page tables.

You will implement a simple version of page tables so that several “programs” can safely share main memory.

Since we are doing a simplified version of page tables, main memory will be a single global array of integers, and instead of programs, we will use threads.

Remember, each program (thread), has its own page table. It should be different from the page tables of the other programs or they will have memory conflicts. Thus if we have 3 programs running, we will need 3 page tables. Every reference to memory by a program needs to use the page table.

You are given a program (/net/326/pagetables.c) that doesn’t use page tables. It will work only if one thread is running, but it won’t work correctly if you have more than one thread, because the memory references don’t use page tables.

You job is to change all the memory references to use page tables.

Remember to use thread:

gcc pagetables.c -lpthread

Demo: Your modified pagetables program and show the code changes you made.