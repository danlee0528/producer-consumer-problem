# producer-consumer-problem
A simplified solution to a bound-buffer problem using POSIX threads semaphores and mutexes in C

# Description
There are 3 consumers who produce products according to different combinations of materials and tools and 3 producers who generate different materials and store generated materials into a buffer (a shared resource).
Buffers used in this program are FIFO queues. The key concept of this problem is that each thread whether it is a prodcuer thread or consumer thread must take a turn to gain access to a shared resource one at a time. Otherwise, deadlock is likely happen and program will stay paused.
