# Data-Structures-and-Algorithms-JAVA-
Labs from UTD's Data Structures and Algorithms class in JAVA programming language

Ji Min Yoon
JXY210022
CS 3345.503

ArrayStack
This code implements a stack ADT implementation using an array and uses the double data type. The constructor initializes the stack with hard coded values (10); however, there's an implementation resize() which allows the stack to have dynamic capacity. 
This method uses the Array class’ copyOf(currentArray, newArraySize) method to create a new array (stack) twice the size of the current array, and copies all the elements of the current array to the new array. Since the code uses the Array class, the copyOf has the time complexity of O(n).
The isEmpty() method returns a boolean (TF) value if the size (the number of elements in the stack) is equal to zero (empty), and has the time complexity of O(1).
The count() method returns the variable size (the number of elements in the stack), and has the time complexity of O(1).
This code sets the top of the stack as position 0 of the array, and pushes the elements (shift them to the right) as new elements get pushed in. If the size (the number of the elements in the stack) reaches the length of the array (the max capacity of that array), it increases the size of the array by double using the implementation explained above. The time complexity of a push operation in a stack will be O(n) since a single element is inserted at the last position. 
The pop method will pop the element on the top position and shift the next element to the top position in order to simulate LILO. Before it pops the top element, it checks if the stack is empty and throws an exception, else it retrieves the element (get the value of arr[0]), and returns it. The time complexity of the pop operation is O(n) since it only deletes an element in the front of the array. 
The peek() method allows the user to peek at the top element’s value without popping the value, and also throws an exception if the stack is empty. This method has the time complexity of this operation is O(1). The reason why the top of the stack was at position 0 was to simulate the LILO of a stack. If the top of the stack were to be at the last position, there will always be empty spaces above the top, which defeats the purpose of the assignment. The upper-bound time complexity of ArrayStack is O(N) due to the method resize().



LinkedStack
This code implements a stack ADT implementation using an LinkedList and uses the double data type. This stack is dynamic, as new values get added on to the stack, new Nodes are created and pushed.
The ListIterator implements the interface from the iterator interface which consists of hasNext(), next(), and remove(). The hasNext() which checks if the data structure has another element after, next() which returns the value and moves the position to the NEXT element in the stack. Furthermore, this class also has variables like private Node current, which represents the current node being traversed. All the methods in this class have the time complexity of O(1).
This project includes the Node class which contains the Accessor And Mutator methods for the variables data, next, and size of the list. This class only has the time complexity of O(1). 
The isEmpty() checks if the stack is empty by looking if the first element(head) is null, if it is, then the stack is empty. The Big O notation for this method is O(1). 
The push method inserts (pops) the new node at the top of the stack. If the head is null, then the head and tail = node since it's the first value of the stack. When the push method receives a double value, a new node is created with that double value and the reference for the first node gets updated. 
The pop() method removes and returns the top element from the stack. The value in the top stack is returned and the top stack reference is set to the new position below. The Big O notation for the method is O(1). 
