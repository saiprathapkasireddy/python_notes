# Garbage Collection 

- Garbage Collector is used to reclaim the memory that used by objects that are no longer in use by the programm.
- Garbage Collection is automatic and transparent to the programmer.

### Cyclic Garbage Collection:

- Python uses a cyclic garbage collector that can identify and collect cyclic references.
- Preventing memory leaks that might occur if cyclic references were not properly handled.

### Generational Garbage Collection :

- Python's garbage collector uses a generational approach, dividing objects into three generations: young, middle-aged, and old. 

-  New objects are initially allocated in the young generation, and if they survive a garbage collection cycle, they are promoted to older generations.

### Reference Counting:

- Python's memory management combines reference counting with garbage collection. 
- Reference counting handles short-term memory management, while garbage collection handles long-term memory management and cyclic references.

### 'gc' Module:

- Python provides the `gc` module, which allows for manual control and fine-tuning of the garbage collection process. 
- While automatic garbage collection is generally effective, the `gc` module can be used to trigger collections,disable collections, or obtain information about the garbage collector's behavior.

```python
a = [1,2,3]
# Reference count of the list is 1.

b = a
# Reference count of the list is 2.

del a
# Now reference count is decreased to 1.

del b
# Now reference count is 0. Memory for list is deleted.
```

## Conclusion:

Garbage collection in Python is a sophisticated system that combines reference counting with cyclic garbage collection to manage memory efficiently. By understanding these mechanisms, developers can write more efficient and memory-safe programs. However, in most cases, Python's automatic garbage collection handles memory management transparently, allowing developers to focus on other aspects of programming.

# Memory Management:

- Memory management in Python involves the allocation and deallocation of memory space for objects during program execution. 

- Python uses a private heap space to manage memory, and the Python memory manager handles the dynamic storage needed by the program. 

## Features:

### Memory Allocation:

- When an object is created in Python, the memory manager allocates space for that object on the heap.The size of the memory block allocated depends on the type and structure of the object.

### Reference Count:

- Python uses a reference counting mechanism to keep track of the number of references to each object.  Each object has a reference count associated with it, and when the count drops to zero, the memory occupied by the object can be reclaimed.

### Garbage Collection:

- While reference counting is a fundamental part of memory management in Python, it may not handle cyclic references (when objects reference each other in a cycle). To address this, Python employs a garbage collector to identify and collect unreachable objects.
