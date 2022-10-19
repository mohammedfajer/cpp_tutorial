


# C/C++ Compilation Model

![image info](./GCC_CompilationProcess.png)

# Things to think about
- static library
- dynamic library
- compiler version
- language features
- build systems
- level of abstraction
- low-level language (binary code machine language)
- mediem-level languages (assembly, c/c++)
- high-level languages (python, javascript)
- static typed languages: statically typed languages perform type checking at compile time
- dynamic typed languages: dynamically-typed languages perform type checking at runtime
- compiled languages
- interpreted languages
- intermediate languages
- garbage collection
- stack and heap and memory management
- Operating Systems
- Debugging
- Profilers
- Computer Architectures
- Cross-Platform programming
- Tools Programming
- Assembly Language
- Optimziation


# Questions
 
### How is the C++ standard library linked to my application?
The standard libraries by default are dynamically linked at runtime.



---

### 1. Pre-processor

takes in the source code and preprocess it. insert files from # include, and other preprocessor directives.

```bash

$ g++ -E -P main.cpp > main.ii
$ main.cpp main.ii
```

### 2. Compiling

taking in the pre-processed source code and generate binary object file non-executable (assembly language)

```bash

$ g++ -S main.ii
$ main.cpp main.ii main.s
```

### 3. Assembly

```bash

$ g++ -c main.s
$ main.cpp main.ii main.s main.o

```
### 4. Linking 

```bash

$ g++ main.o -o main
$ main.cpp main.ii main.s main.o main.exe
$ ./main.exe
$ hello world
$
```


### In one Go
```bash
$ g++ main.cpp -o main
$ main.cpp main.exe
$ ./main.exe
$ hello world
$ 
```

# Build Systems
- Batch File
- Make
- CMake
- Ninja

# Compilers
- GNU GCC G++
- Clang
- LLVM
- MinGW
- Intel C++ Compiler
- Microsoft cl




## Good Resources
- https://www.youtube.com/watch?v=zOmUHM0sFOc&t=798s
- https://www.youtube.com/watch?v=I1f45REi3k4
