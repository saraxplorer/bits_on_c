There are two types of memory allocation.

Stack Allocation: When you declare int pipefd[2];, memory is allocated on the stack for the array. This is a fixed-size allocation and automatically managed.

Dynamic Allocation: Using malloc allocates memory on the heap, which must be managed manually (allocation and deallocation).

In both cases, memory is allocated.\
So, making an array also means allocating memory. It is the stack allocation


