# Java-Collection

For Collection interface, we have list, set and queue. Java also has an interface called Map.

Why Map interface doesn’t extend Collection interface?
If  Map  extends  Collection  interface,  then  where  are the  elements?  Map contains  key-value  pairs  and  it  provides methods to retrieve list of Keys or values as Collection but it doesn’t fit into the “group of elements” paradigm.

Hashcode() and equals()

The contract between equals() and hashCode() is that: 

1)  If two objects are equal, then they must have the same hash code. 

2)  If two objects have the same hashcode, they may or may not be equal.

Collection vs Collections: 

Collections in java is a framework that provides an architecture to store and manipulate the group of objects.
All the operations that you perform on a data such as searching, sorting, insertion, manipulation, deletion etc. can be performed by Java Collections.

Java Collection simply means a single unit of objects. Java Collection framework provides many interfaces (Set, List, Queue, Deque etc.) and classes (ArrayList, Vector, LinkedList, PriorityQueue, HashSet, LinkedHashSet, TreeSet etc).

The procedure of inserting an element to a HashSet
•	Step 1: the HashSet verifies whether the new element is a duplicate or not. If it is not a duplicate, then move to St
•	Step 2: Use a hash function to operate on the hash code of the new element and get the location in the bucket.
•	Step 3: If the location is empty, save the new element as well as its hash code to the location; if the location is already occupied, then build a linked list and add the new element at the end of the linked list.  
•	If all the elements have the same hash codes in the HashSet, then the HashSet will be reduced to a LinkedList and its lookup time will be decreased from O(1) to O(n).

What is the load factor of a HashSet?
•	By default, load factor is 75%. If the number of the elements reaches 75% of the capacity, the HashSet will double its size and all the elements will be rehashed to the new container.
•	The load factor can be customized as a parameter when we instantiate a HashSet.


ArrayList, LinkedList, Vector

Difference between ArrayList and Vector
ArrayList is not thread-safe, while Vector is thread-safe. So ArrayList has better performance than Vector.
When the collection needs resizing, ArrayList  increases 50%, while Vector increases 100%






