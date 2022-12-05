# **JavaScript**
JavaScript (JS) is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions. 
While it is most well-known as the scripting language for Web pages, many non-browser environments also use it,
such as Node.js, Apache CouchDB and Adobe Acrobat. JavaScript is a prototype-based, multi-paradigm, single-threaded, 
dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles.
<br/>
<br/>

## Understanding of Javascript

1. Lightweight means it doesn't consume heavy resources while its running.

2. Interpreted means the parsing of code happens line by line before it's getting executed. Due to this, Javascript is very easy to debug
and very slow compared to compiled languages, but debugging is very difficult to do in compiled languages.

3. Just in time compiled means instead of ahead of time(like pure compiled languages), it does compilation part by part. With this, we
can able to debug and get good execution speed.
Suppose in javascript,  Typical scenario
The source code is completely converted into machine code

<br/>
<br/>

**JIT scenario**
The source code will be converted into assembly language like structure [for ex IL (intermediate language) for C#, ByteCode for java].

The intermediate code is converted into machine language only when the application needs that is required codes are only converted to machine code.
<br/>
<br/>

**JIT vs Non-JIT comparison :**

In JIT not all the code is converted into machine code first a part of the code that is necessary will be converted into machine code then if a method or functionality called is not in machine then that will be turned into machine code, which reduces burden on the CPU. As the machine code will be generated on run time, the JIT compiler will produce machine code that 
is optimized for running machine’s CPU architecture.
<br/>
<br/>

*Some examples of JIT are:*

1. Java: JVM (Java Virtual Machine)
2. C#: CLR (Common Language Runtime)
3. Android: DVM (Dalvik Virtual Machine) or ART (Android RunTime) in newer versions
The Java Virtual Machine (JVM) executes bytecode and maintains a count as of how many time a function is executed. If this count exceeds a predefined limit JIT compiles the code into machine language which can directly be executed by the processor (unlike the normal case in which javac compiles the code into bytecode and then Java, the interpreter interprets this bytecode line by line converts it into machine code and executes).
<br/>

Also next time this function is calculated same compiled code is executed again unlike normal interpretation in which the code is interpreted again line by line. This makes execution faster.

Same thing happens with javascript as well, when we run/execute the code in browser or server-side it will start execute from global (top level) and create a compiled version of global execution context. This global execution context will get execute in main call stack and if this execution context needs any other function call then another execution context will get created (means the new function will get compiled and interpreter will run/execute the machine code for that newly created execution context). In this way the JIT compilation happens in Javascript.

To know more about JIT in javascript follow this [link](https://www.freecodecamp.org/news/just-in-time-compilation-explained), and to know more about execution context and its phases please follow this [link](https://www.freecodecamp.org/news/javascript-execution-context-and-hoisting/)
