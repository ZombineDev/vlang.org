# Why D ? #
>"D aims to be C++’s successor in the realm of systems programming. Like Java and C#, D aims to avoid the complexity of C++, and to this end it uses some of the same techniques. Garbage collection is in, manual memory management is out. Single inheritance and interfaces are in, multiple inheritance is out. But then D starts down a path of its own." - Scot Mayer

## A Brief Feature List of D
* A short learning curve for C++ programmers
* Competent programmers should be able to understand the entire D language without great effort
* There is no text preprocessor
* No need of memory management
* Design by Contract for building reliable programs
* Unit testing is built into the language
* When necessary, down and dirty to the metal coding should be supported
* Using pointers should be exceptional, rather than ubiquitous

## Setting Your Expectations
* You are not a SW engineer, you are a HW designer and your job is verification of HW. The struggle of D against C++, Java, C# etc is D's own fight in SW domain and you have nothing to do with it. 
* The extension of D we are proposing is not proposed to compete C++/SystemC, rather the extension will compliment C++/SystemC. 
* D is equally (or more ) powerful in comparison to C++ and much more than SystemVerilog, it is neither SystemC/C++ nor Verilog/SystemVerilog and hence it has high prospect to verify designs and models written in SystemC/C++ and SystemVerilog.  
* Using D and VLang you will write testbenches and test cases which needs to be fast & dirty and you need a compiler which cleans up all dirt.
* As a verification engineer you are more interested in advanced features of language and you do not want to take the pain of performance issues of your implementation.
* Vlang will never be used like SystemC OR verilog design, it will never be synthesized - it will only be used in verification.
* D is a **Systems Programming** language like C/C++ and hence they are complimentary - you want that feature.
* D can inline assembly code like C/C++ and hence they are complimentary - you want that feature.
* D has some features like Java and you want them - again you will not write a GUI with your verification language.
* You do not want your test suit to take hours to compile and elaborate - you have a job to run many test cases.
* You need a language where nothing can go wrong - you cannot maintain a **Coding Guideline** for everything and deploy it scrictly - you need a modern language which takes care of dirty coding.
* You need a language which is very readable and clean syntax while providing you & your team immense power.
* You want a language which you & your team can learn fast.

## Gliding Through Exclusive Features of D
### Interoperability with C/C++

Although D is a **re-engineered C++ language**, but it still maintains a strong compatibility with C/C++.

* D is ABI compatible with C++.
* c.stdio allows you to use standard C library.
* Interfaces are natural with C:
 * Calling C++ Global Functions From D
 * Calling Global D Functions From C++
 * Calling C++ Virtual Functions From D
 * Calling D Virtual Functions From C++
* Inline assembly
* How does D do it ?
 * matching C++ name mangling conventions
 * matching C++ function calling conventions
 * matching C++ virtual function table layout for single inheritance

### Features - C++11 and Beyond

* Compile Time
* Run Time
* Garbage Collector (GC is one reason people find SV usable and SystemC tough. We need GC and pointerless programming)

* Object oriented programming
 * Classes & Interfaces
 * Function & Operator Overloading

* Productivity
 * Modules
 * Declaration vs definition
 * Templates, generic programming and concepts (known as constraints in D)
 * Arrays, associative arrays, dynamic arrays, slices and associated conveniences
 * Real typedefs   
 * Bit types

* Functions
 * Nested functions
 * Function literals (lambdas)
 * Dynamic closure
 * *in*, *out* and *inout* paramaters
 * Strings   

* Resource management
 * Garbage collection
 * Explicit memory management
 * RAII
 * Inline assembler

* Reliability
 * Contracts
 * Unit testing
 * Debug attributes and statements
 * Exception handling
 * Synchronization
 * Compile time checks
 * Run time checks

* Compatibility
 * Operator precedence and evaluation rules
 * Direct access to C API's
 * OS exception handling
 * Exception handling
 * Uses existing tools

* Project management
 * Versioning
 * Deprecation
 * No warnings




### Gotchas 

How many of you have not went through standard SystemVerilog Coding guidelines?
How many of you have not went through standard C++ Coding guidelines?

* D does not have known coding gotchas
* Try *if ( a = b)* in D ... 
* There were known gotchas which were bugs and got fixed gradually, like *enum a = [0, 1, 2]*
* You might consider something as gotchas due to language migration, like slices behavior, floating point, etc


```D
void main() {
  import std.stdio: writeln;
  writeln("Hello World");
}
```
