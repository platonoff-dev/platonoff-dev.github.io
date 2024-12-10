---
title: Alcor implementation plan
date: 2024-12-10
---
# Alcor implementation plan

Creating a programming language has always been a fascinating challenge, one that combines creativity with technical depth. Alcor is my experiment in this realm—a project where I explore language design, compilers, and interpreters while deepening my understanding of how programming tools work. The journey is one of discovery, frustration, and, most importantly, immense satisfaction. Through Alcor, I aim to learn not just about making a language but also about the decisions, trade-offs, and artistry behind them.

## Lexing and Parsing

Every programming language begins with the fundamentals of lexing and parsing. For Alcor, I decide to handwrite both components, immersing myself in the nuances of converting raw text into meaningful structures. Writing the lexer reveals how languages break down the chaos of code into manageable symbols. Parsing, on the other hand, is about constructing order, turning tokens into a logical abstract syntax tree (AST).

### Bringing Alcor to Life: Tree-Walking Interpreter

Seeing my code come to life feels magical, and that’s exactly what the tree-walking interpreter brings to Alcor. By traversing the AST and evaluating each node directly, I execute small programs almost immediately. This stage isn’t about performance but about momentum—it’s the fastest way to breathe life into Alcor and keep myself motivated

### Thinking Ahead: From Interpreter to Compiler

After getting Alcor off the ground, I take the next step—transforming it from an interpreted language to a compiled one. Designing a virtual machine (VM) is both exciting and intimidating, as it requires me to think about bytecode, stack management, and execution models. Writing a bytecode interpreter helps me solidify these concepts, while designing an intermediate language (IL) serves as a bridge between the AST and VM. It’s here that I truly begin to appreciate the craftsmanship of modern programming languages.

### Optimizing Alcor

Once the basics of compilation are in place, optimization becomes the focus. Initially, I implement simple techniques like constant folding and dead code elimination, which make a noticeable difference in performance. Diving into more advanced optimizations—like inlining and common subexpression elimination—is both challenging and rewarding. Optimization isn’t just about making things faster; it’s about understanding the trade-offs and ensuring correctness while improving performance.

### Adding a Typing System

Typing is one of the most complex and intellectually stimulating parts of Alcor’s journey. I start with a dynamic type system to keep things simple but soon realize the power and elegance of static typing. Designing a hybrid system requires balancing flexibility with safety, as well as researching type inference and generics. This stage pushes me to explore the theoretical foundations of type systems and reflect on how typing shapes a language’s usability and behavior. Although it’s daunting, it becomes one of the most rewarding aspects of the project.

### The Extras: Standard Library, Module System, and Debugger

A language is more than just syntax and semantics—it’s also about the tools and utilities that make it usable. For Alcor, building a standard library with basic functionality, like string manipulation and file I/O, is essential. Adding a module system gives the language structure and modularity, making larger programs feasible. Creating a debugger is a fun and satisfying challenge; implementing breakpoints and variable inspection makes Alcor more approachable for developers (myself included). These extras transform Alcor from a prototype into something that feels like a real language.