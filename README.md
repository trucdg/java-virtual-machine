# What is Java Virtual Machine (JVM)?
- JVM is a program that provides a runtime environment to run the java code or applications.
- JVM converts `Java bytecode` into machine languages.
- JVM is a part of the Java Runtime Environment (JRE).
- In other programming languages, the compiler produces machine code for a particular system. However, Java compiler produces machine code for a Virtual Machine known as Java Virtual Machine.
> Note: `compilers` analyze and convert ***source code (i.e Java, C++. etc)*** to **machine code** or **bytecode** that can be executed by the target host system.

## What is the JVM used for?
Java Virtual Machine serves 2 primary purposes:
1. To provide a means for a Java program to run on any platform. (java is platform independent, but JVM is platform dependent i.e different configurations of JVM is needed for different O.S).
2. To maintain and optimize program memory

## JVM Architecture
![image](https://github.com/trucdg/java-virtual-machine/assets/91285203/db3182ee-56e6-4e18-9130-6ebb413229d3)

1. **ClassLoader**
   - The class loader is used for loading class files. Class files are needed for the class loader to perform its 3 primary functions: Loading, Linking, and Initialization.
2. **Method Area**
   - JVM Method Area stores class structures like metadata, the constant runtime pool, and  the code for methods.
3. **Heap**
   - All the **Objects**, their related **instance variables**, and **arrays** are stored **in the heap**. **This memory is common and shared across multiple threads.**
4. **JVM language stacks**
   - Java language stacks store local variables, and it's partial results.
   - Each thread has its own JVM stack, created simultaneously as the thread is created. A new frame is created whenever a method is invoked, and it is deleted when method invocation is completed.
5. **PC Registers** (Program Counter register)
   - PC register store the address of the Java Virtual Machine instruction which is currently executing. In Java, each thread has its separate PC register.
6. **Native Method Stacks**
   - Native method stacks hold the instruction of native code depends on the native library. It is written in another language instead of Java.
7. **Execution Engine**
   - It is a type of software used to test hardware, software, or complete systems. It does so without retaining any information about the tested product.
8. **Native Method Interface**
    - The Native Method Interface is a programming framework. It allows Java code which is running in a JVM to call libraries and native applications.
9. **Native Method Libraries**
    - Native Method Libraries is a collection of the Native Libraries (C, C++) which are needed by the Execution Engine.
      
## Software Code Compilation and Execution process
In order to write and execute a software program, you need the following:
1. Editor - to type your program into, a notepad can be used for this.
2. Compiter - to convert your high language program into native machine code.
3. Linker - to combine different program files reference in your main program together.
4. Loader - to load the files from your secondary storage device like Hard Disk, Flask Drive, CD into RAM for execution. The loading is automatically done when you execute your code
5. Execution - actual execution of the code which is handled by your O.S & processor

### Resources:
- [What is JVM: Architecture explained!](https://www.guru99.com/java-virtual-machine-jvm.html)



























