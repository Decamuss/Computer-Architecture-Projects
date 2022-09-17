# projectAssignments
Programming assignments from Computer Architecture Class

rot13.c: Write a program rot13 that encodes its argument using rot-13 and prints the results, followed by a newline character. You MAY assume that rot13 will receive exactly one argument, but it is good practice to check whether the number of arguments is correct. Only scenarios with one argument may be tested.


sorta.c: Write a program sorta that sorts and prints its arguments. sorta takes zero or more arguments, sorts them lexicographically, and then prints each argument on its own line.


sudoko.c: Write a program sudoku that (part 1) checks whether a proposed Sudoku solution is correct and (part 2) checks whether a partially-solved Sudoku puzzle with one unknown square can be solved. sudoku takes a single argument, which is the path to a file containing a completed or almost-completed Sudoku puzzle.


list.c: Write a program list that maintains and manipulates a sorted linked list according to instructions received from standard input. The linked list is maintained in order, meaning that the items in the list are stored in increasing numeric order after every operation.
Note that list will need to allocate space for new nodes as they are created, using malloc; any allocated space should be deallocated using free as soon as it is no longer needed.
list supports two operations:
insert: n Adds an integer n to the list. If n is already present in the list, it does nothing. The instruction format is an i followed by a space and an integer n.
delete: n Removes an integer n from the list. If n is not present in the list, it does nothing. The instruction format is a d followed by a space and an integer n.
After each command, list will print the length of the list followed by the contents of the list, in order from first (least) to last (greatest).


mexp.c: Write a program mexp that multiplies a square matrix by itself a specified number of times. mexp takes a single argument, which is the path to a file containing a square (k ×k) matrix M and a non-negative exponent n. It computes M nand prints the result.
Note that the size of the matrix is not known statically. You must use malloc to allocate space for the matrix once you obtain its size from the input file.
To compute M n, it is sufficient to multiply M by itself n −1 times. That is, M 3 = M ×M ×M .
Naturally, a different strategy is needed for M 0.


bst.c: Write a program bst that manipulates binary search trees. It will receive commands from standard input, and print resposes to those commands to standard output. bst will need to allocate space for new nodes as they are created using malloc; any allocated space should be deallocated using free before bst terminates.
This portion of the assignment has two parts.

Part 1 In this part, you will implement bst with three commands:
insert: n Adds a value to the tree, if not already present. The new node will always be added as the child of an existing node, or as the root. No existing node will change or move as as result of inserting an item. If n was not present, and hence has been inserted, bst will print inserted. Otherwise, it will print not inserted. The instruction format is an i followed by a decimal integer n.
search: n Searches the tree for a value n. If n is present, bst will print present. Otherwise, it will print absent. The instruction format is an s followed by a space and an integer n.
print: Prints the current tree structure

Part 2 In this part, you will implement bst with an additional fourth command:
delete: n Removes a value from the tree. See section 1.6.2 for further discussion of deleting nodes.
If n is not present, print absent. Otherwise, print deleted. The instruction format is a d followed by a space and an integer n.
