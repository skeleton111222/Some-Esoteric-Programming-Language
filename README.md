# Brainfuck Programming Language

**Brainfuck** is an esoteric programming language designed to challenge programmers by limiting the available commands to a very minimal set. Despite its simplicity, Brainfuck is **Turing complete**, meaning it can theoretically compute anything that can be computed by other programming languages (given enough memory and time).

---

## Overview

- **Paradigm(s)**: Imperative
- **Designed by**: Urban Müller
- **First Appeared**: 1993
- **Memory System**: Cell-based
- **Dimensions**: One-dimensional
- **Computational Class**: Turing complete

---

## Major Implementations

- **Original Brainfuck**: [Link to the original Brainfuck interpreter](http://main.aminet.net/dev/lang/brainfuck-2.lha)
- **Awib**: [GitHub Repository of Awib](https://github.com/matslina/awib)
- **Online BF Interpreter**:[TryItOnline](https://tio.run/#brainfuck)

---

## Influences

- **Influenced by**: FALSE, P''
- **Influenced**: List of derivatives (various Brainfuck-based languages)

---

## File Extensions

- `.b`
- `.bf`

---

## Language Instructions

Brainfuck operates using **only 8 commands**, and all programs are written using combinations of these characters. Below is a table listing each character and its associated operation.

| Character | Instruction                                                         | Description                                                                                    |
| --------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `>`       | Move the pointer to the right                                       | Increases the memory cell pointer by one                                                       |
| `<`       | Move the pointer to the left                                        | Decreases the memory cell pointer by one                                                       |
| `+`       | Increment the memory cell at the pointer                            | Increases the value at the current memory cell by 1                                            |
| `-`       | Decrement the memory cell at the pointer                            | Decreases the value at the current memory cell by 1                                            |
| `.`       | Output the character signified by the cell at the pointer           | Prints the character corresponding to the ASCII value stored at the current cell               |
| `,`       | Input a character and store it in the cell at the pointer           | Accepts a single character input from the user and stores it in the current memory cell        |
| `[`       | Jump past the matching `]` if the cell at the pointer is 0          | Begins a loop; skips to the matching `]` if the value at the current memory cell is 0          |
| `]`       | Jump back to the matching `[` if the cell at the pointer is nonzero | Ends a loop; jumps back to the matching `[` if the value at the current memory cell is nonzero |

---

## Example Code

Here’s a simple example of a Brainfuck program that prints **"Hello, World!"**:

```brainfuck
++++++++[>++++[>++>+++>+++>+<<<<-]>+>+>->>+[<]<-]>>.>---.+++++++..+++.>>.<-.<.+++.------.--------.>>+.>++.
```
