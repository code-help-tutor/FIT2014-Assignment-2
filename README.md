# Monash University FIT2014 Assignment 2

**Due**: 11:55pm, Friday 4 October 2024

## 1. Introduction
In this assignment, you will:
- Implement a lexical analyser using lex (Problem 3).
- Implement parsers using lex and yacc (Problems 1 - 6).
- Program a Turing machine (Problem 7).
- Learn about some aspects of quantum circuits and quantum registers (Problems 2 - 6).
- Practise skills related to Pumping Lemmas and Context - Free Languages (Problem 8).

## 2. Assignment Management
- Start working early and spread the work over time. Do as much as possible before week 10.
- Don't be deterred by the length of the document. Much of it is a tutorial and documentation.

## 3. How to Begin
1. Download the workbench `asgn2.zip` from Moodle.
2. Create a new Ed Workspace and upload the file, let Ed extract it.
3. Edit the `student - id` file with your name and student ID.
4. Open a terminal and change into the `asgn2` directory.

## 4. Files in the Directory
- `plus - times - power.l`: Starting point for some lex files.
- `plus - times - power.y`: Starting point for some yacc files.
- `quant.h`: Should remain unaltered.
- `prob6.awk`: An awk program for a specific task.

## 5. Submission Requirements
Your submission must include:
- `student - id` file edited with your name and student ID.
- `prob1.l`: Obtained by modifying a copy of `plus - times - power.l`.
- `prob2.pdf`: Your solution to Problem 2 (Context - Free Grammar for QCIRC).
- `prob3.l`: Obtained by modifying a copy of `plus - times - power.l`.
- `prob4.l`: Obtained by modifying a copy of `prob3.l`.
- `prob4.y`: Obtained by modifying a copy of `plus - times - power.y`.
- `prob5.l`: Obtained by modifying a copy of `prob4.l`.
- `prob5.y`: Obtained by modifying a copy of `prob4.y`.
- `prob6.txt`: Ten lines, solution to Problem 6.
- `prob7.tm`: Tuatara Turing machine file.
- `prob8.pdf`: Your solution to Problem 8.

## 6. Assignment Tasks

### Problem 1 (2 marks)
Construct `prob1.l` to be used with `plus - times - power.y` to build a parser for PLUS - TIMES - POWER.

### Problem 2 (3 marks)
Write a Context - Free Grammar for the language QCIRC over the alphabet {I, H, X, Y, Z, CNOT, TOF, *, ⊗, (, ) } and save it as `prob2.pdf`.

### Problem 3 (3 marks)
Construct a lex file `prob3.l` starting from `plus - times - power.l` to build a lexical analyser for QCIRC.

### Problem 4 (6 marks)
- Make a copy of `prob3.l` called `prob4.l` and modify it for use with yacc.
- Construct a yacc file `prob4.y` from `plus - times - power.y`.
- Build a parser for QCIRC that can evaluate expressions.

### Problem 5 (5 marks)
- Make copies of `prob4.l` and `prob4.y` called `prob5.l` and `prob5.y` respectively.
- Modify them further to build a parser for QUANT.

### Problem 6 (5 marks)
- Use the `prob6.awk` program to convert your student ID to a quantum register expression.
- Copy the expression into `prob6.txt` as the first line.
- Run your parser on the expression and append the result to `prob6.txt`.

### Problem 7 (7 marks)
Build a Turing machine in Tuatara v2.1 that computes the number choice function and save it as `prob7.tm`.

### Problem 8 (9 marks)
- Prove there is no Universal Regular Expression using the Pumping lemma for Regular Languages.
- Prove there is no Universal Context - Free Grammar using the Pumping lemma for Context - Free Languages. Save the proof as `prob8.pdf`.

## 7. Lex and Yacc Basics

### Lex
- An input file to lex ends in `.l` and has three parts: definitions, rules, C code.
- The `plus - times - power.l` file is used as an example. It identifies tokens like nonnegative integers (NUMBER), `Power` (POWER), and specific characters.
- When lex runs on the file, it generates `lex.yy.c` which can be compiled to create a lexical analyser.

### Yacc
- An input file for yacc ends in `.y` and has three parts: declarations, rules, programs.
- The `plus - times - power.y` file is used as an example. It has a grammar for PLUS - TIMES - POWER and declarations for tokens and nonterminals.
- To generate a parser, you need to modify `prob1.l` and use `plus - times - power.y` along with some compilation steps.

## 8. Quantum Circuits and Registers
- A quantum computer uses quantum physics for computation.
- It has a register that stores information in a superposition and a quantum circuit expression that transforms the register.
- The languages QCIRC, QREG, and QUANT are defined to describe quantum expressions.
- QCIRC is for valid quantum circuit expressions, QREG for valid quantum register expressions, and QUANT is their union.

## 9. The Number Choice Function
- Input: A sequence $k, x_{1}, x_{2},..., x_{n}$ encoded as $a^{k}ba^{x_{1}}ba^{x_{2}}b\cdots a^{x_{n}}$.
- Output: $x_{k}$ encoded as $a^{x_{k}}$.
- A Turing machine for this function should reject invalid inputs.

## 10. Universal Models
- Universal regular expressions and universal context - free grammars are defined.
- The goal is to find expressions/grammars that can match/generate all relevant strings for a given set of regular expressions/context - free grammars.
# FIT2014 Assignment 2

# CS Tutor | 计算机编程辅导 | Code Help | Programming Help

# WeChat: cstutorcs

# Email: tutorcs@163.com

# QQ: 749389476

# 非中介, 直接联系程序员本人
