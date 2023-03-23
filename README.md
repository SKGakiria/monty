Project name: 0x19. C - Stacks, Queues - LIFO, FIFO

Contributors: Stacy Gakiria and Alex Maina

Stack: This is a linear data structure that follows the LIFO (Last In First Out) approach 
	to implement basic  operations such as push, pop, peek, and traverse.
	A Stack can be implemented using an Array or Linked List.

Queue: This is also a linear data structure to store and manipulate the data elements.
	It follows the order of First In First Out (FIFO).
	This means that the first element entered into the array is the first element to be removed from the array.

To demonstrate this, we shall use the monty program which implements simple stack based code.

The goal for the project is to create an interpreter for the monty bytecode files (this files usually have an '.m' file extention).

opcode: operation code

NB: We are only allowed to use malloc and free for dynamic memory allocation for this project.


The monty program

Usage: monty file
where file is the path to the file containing Monty byte code

If the user does not give any file or more than one argument to your program, print the error message USAGE: monty file, followed by a new line, and exit with the status EXIT_FAILURE

If, for any reason, it’s not possible to open the file, print the error message Error: Can't open file <file>, followed by a new line, and exit with the status EXIT_FAILURE

where <file> is the name of the file
If the file contains an invalid instruction, print the error message L<line_number>: unknown instruction <opcode>, followed by a new line, and exit with the status EXIT_FAILURE

where is the line number where the instruction appears.
Line numbers always start at 1

The monty program runs the bytecodes line by line and stop if either:
it executed properly every line of the file
it finds an error in the file
an error occured

If you can’t malloc anymore, print the error message Error: malloc failed, followed by a new line, and exit with status EXIT_FAILURE.
