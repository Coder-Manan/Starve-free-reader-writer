# Starve-free-reader-writer
This repo contains pseudocode for a starve free solution to the reader writer problem
This is my submission for the project for course CSN 232 (Operating Systems), spring semester 2022-23

## Pseudocode Explanation
Two binary semaphores(`ww, w`) and a counting semaphore(`r`) are used.
New reader processes are allowed to start reading as long as no writer is waiting. When a writer is waiting all the new readers are blocked. The binary semaphore `ww` tells whether a writer is waiting or not. Writers also perform the wait operation for this semaphore.
The counting semaphore `r`’s count tells the number of readers currently reading. When all readers finish reading, signal operation is performed on semaphore `w` indicating that now a writer can write, in case it is waiting.

# Details
Manan Garg<br>
21114056<br>
B.Tech CSE 2Y<br>
IIT Roorkee
