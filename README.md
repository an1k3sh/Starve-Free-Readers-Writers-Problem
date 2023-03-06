# Starve-Free-Readers-Writers-Problem

The Readers-Writers problem is a classical computing problem in the field of concurrency and synchronization, wherein a resource like a database, file, storage area etc. is being accessed by multiple processes concurrently. Each of these processes has a critical section where it is accessing the resource for reading or writing. If the resource is being accessed by a writer process, no other reader or writer process may access it. While, if it is being accessed by a reader resource, other reader processes may access it, but no writer can access it.

Semaphores or monitors can be used to solve the Readers-Writers problem without conflicts. The well-known solutions for the Readers-Writers problem raise the issue of starvation of either the Readers or the Writers. The given solution for the problem solves the issue of starvation.

## Data Structures Used

The given pseudocode used a FIFO queue for the processes which are waiting currently. A new structure PCB (Process Control Block) has been defined. It contains details about each process. Semaphore structure has been used to implement semaphores.

## Files

1. PCB.pseudo -  It contains the declaration of the Process Control Block (PCB) data structure.
2. queue.pseudo - It contains the declaration of the Queue data structure used.
3. semaphore.pseudo -  It contains the declaration of semaphore data structure.
4. global_variables.pseudo - It contains the declaration of all global variables.
5. reader.pseudo - It refers to the code for readers.
6. writer.pseudo - It refers to the code for writers.

## References

1. *Operating System Concepts* (Ninth Edition), Silberschatz, Galvin, Gagne
2. [Faster Fair Solution for the Reader-Writer Problem](https://arxiv.org/pdf/1309.4507.pdf)
