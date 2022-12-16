## Python Memory Management

Every thing in the python is a object, even some of the objects can hold other objects like list,set and tuples. It require the alot of memory allocation, because of the dynamic alloation of memory python need alot of small memory allocation. To perform this python uses PyMalloc as the memory allocator.

Small object allocation For Python Interpretor:

Python sub-allocates big blocks of memory to reduce the overhead for the small object(less size then 512 byte) memory  allocation.There are three type of the memory:
1) Block
2) Pool
3) Arena

### Block: <br/>
Block is a chunk of memory of a certain size. Each block can keep only one Python object of a fixed size. The size of the block can vary from 8 to 512 bytes and must be a multiple of eight (i.e., use 8-byte alignment). For convenience, such blocks are grouped in 64 size classes.






