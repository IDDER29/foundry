# foundry

**foundry** is a custom implementation of a formatted output engine in C.

It focuses on the mechanics behind formatted printing — parsing format strings, managing variadic arguments, and producing precise, predictable output.

Rather than treating formatted output as a black box, this project explores how formatting systems are built from the ground up.

---

## Philosophy

Formatted output sits at the intersection of parsing, data representation, and performance.

This project is guided by the following principles:

- **Explicit parsing logic**  
  Format strings are processed step by step with no hidden behavior.

- **Controlled output**  
  Every character written is intentional and accounted for.

- **Separation of concerns**  
  Parsing, formatting, and output are kept logically distinct.

- **Predictable behavior**  
  Edge cases are handled deliberately, not implicitly.

---

## Features

The library supports a subset of standard `printf` functionality, including:

- Variadic argument handling
- Integer and string formatting
- Width and precision control
- Flags and format specifiers
- Modular formatting pipeline

All behavior is implemented from scratch without relying on the standard `printf`.

---

## Structure
.
├── include/ # Public interface
├── src/ # Core implementation
│ ├── parser/ # Format string parsing
│ ├── format/ # Value formatting
│ └── output/ # Write logic
├── Makefile
└── README.md

The structure emphasizes clarity and separation between stages of the formatting process.

---

## Usage

Build the library and link it into your C project:

