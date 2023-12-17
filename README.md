0x19. C - Stacks, Queues - LIFO, FIFO
Best way to declare and define global variables
The clean, reliable way to declare and define global variables is to use a header file to contain an extern declaration of the variable.

The header is included by the one source file that defines the variable and by all the source files that reference the variable. For each program, one source file (and only one source file) defines the variable. Similarly, one header file (and only one header file) should declare the variable. The header file is crucial; it enables cross-checking between independent TUs (translation units — think source files) and ensures consistency.
