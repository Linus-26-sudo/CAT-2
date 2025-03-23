**Q1.md**
**1) Rules of Big O Notation in algorithim analysis.**
**a) Focus on the dominant term.**
- Under this rule, only the trem with the highest growth rate matters.
- Example: O(n2 + n) = O(n2)
- In the example above, the n term is the dominant term. Therefore as n becomes dominant, the n2 term will overshadow the n term since it dominates twice faster then the other term. Thus having the result as O(n2).

**b) Ignore constants.**
- In this rule, the coeffients and lower order terms are irrelevant for large input sizes.
- Example: O(2n) = O(n)
- As shown in the example in the above, the constant value, that is '2', has been ignored and it coeffient, which is 'n' has been selected. The complexity of data is simplified by dropping coeffients since the do not impact the growth rate for large inputs.

**c) Dropping non-dominant terms.**
- In a combined complexity, the term with the highest growth rate is retained and the other terms are discarded since the are insignificant for large input sizes.
- Example: O(n + n2 + logn) = O(n2)
- The example clearly shows that n2 is the dominant term because its growth rate is much faster than the other terms (n, logn). Therefore the overall complexity simplifies to O(n2).

**d) Constant time operations.**
- Under constant time operations, these are the kind of operations that take the same amount of time to be executed regardless of the input size.
- Example: O(1).
- Constant time operations are more efficient, since they are not affected by the input size.

**e) Consider input size changes.**
- When the input size reduces, the time complexity of the algorithim will present a logarithimic growth which is denoted as O(logn).
- This occurs since the number of operations required grows in proportion to the logarithim of the input size.

**Q2.md**
**2) Difference between arrays and linked list.**
   **i) Memory allocation.**
     Arrays.
   - An Array is a collection of homogeneous data elements in a contiguous memory.
   - Arrays store large amounts of data that are of the same type.
   - The data elements in an array are stored in a linear order.
     Linked list.
   - A linked list is a linear collection of data elements.
   - The data elements are known as nodes. Each node stores the address of the next node, each node contains one or more than one data field and an address field that stores the address of the next node.
   - A Linked list is dynamic where by the memory is allocated as when it is required.

   **ii) Performance.**
   - Arrays allow direct access to the data using indexing. This is beacuse the collection of data elements in an array is contigous and thus allows a linear search in an unsorted array and a binary search in a sorted array.
   - A linked list however does not allow direct access to the data since the elements are stored separately in nodes. Therefore in order to access the data elements, a traversing action must be done so as to obtain the required data element.
     
   **iii) Insertion and deletion.**
   - Under arrays, during the insertion of data at the beginning, all the data elements must be shifted to the right side so as to create space for the new data elements while if the arrays are at the middle, the elements after the insertion must be shifted to the right.
   - During deletion of arrays, if the array is the end, the last element of that array is removed and if the array appears at the beginning, the elements of that array must be shifted to the left side to fill the gap.
   - Insertion of data in linked list occurs in the nodes whereby if the linked list is at the beginning, an update will be performed on the header pointer to the new node, and if the linked list is at the end and a tail pointer is maintained, the traversal method will be used.
   - Deletion of a linked list involves moving the header pointer to the next node if the linked list is at the beginning, and if the the linked list deletion occurs at the end, the second last node is traversed to remove the last node in a singly linked list.
     
  
