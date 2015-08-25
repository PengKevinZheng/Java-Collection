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



