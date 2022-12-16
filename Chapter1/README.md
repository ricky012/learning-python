How does Python work?

Python is an interpreted, high-level, general-purpose programming language. It is is dynamically typed and garbage-collected.

Python is an interpreted language and not a compiled one, although compilation is a step. Python code, written in .py file is first compiled to what is called bytecode (discussed in detail further) which is stored with a .pyc or .pyo format.This bytecode is a low-level set of instructions that can be executed by an interpreter.

Why Interpreted?

One popular advantage of interpreted languages is that they are platform-independent. As long as the Python bytecode and the Virtual Machine have the same version, Python bytecode can be executed on any platform (Windows, MacOS, etc).

Dynamic typing is another advantage. In static-typed languages like C++, you have to declare the variable type and any discrepancy like adding a string and an integer is checked during compile time. In strongly typed languages like Python, it is the job of the interpreter to check the validity of the variable types and operations performed.

Disadvantages of Interpreted languages:

Dynamic typing provides a lot of freedom, but simultaneously it makes your code risky and sometimes difficult to debug.

Python is often accused of being ‘slow’. Now while the term is relative and argued a lot, the reason for being slow is because the interpreter has to do extra work to have the bytecode instruction translated into a form that can be executed on the machine.

What exactly is Garbage Collection?

In a simplified way, it keeps track of the number of references to an object. When that number goes down to zero, it deletes that object. This is called reference counting. This cannot be disabled in Python.

What is __pycache__ ?

Many times in your personal project or on GitHub, you might have seen a folder named __pycache__ being created automatically.

---folder <br/>
&nbsp;&nbsp;&nbsp;- __pycache__<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- test.cpython.pyc<br/>
&nbsp;&nbsp;&nbsp;-test.py<br/>

In this name of the python code it embeded type of interpreted and then .pyc it contain bytecode. Type of interpreted language is C, for the java it will be JPython.
But why is the folder created in the first place? Well, it slightly increases the speed of the Python program. Unless you change your Python code, recompilation to bytecode is avoided, thereby saving time.