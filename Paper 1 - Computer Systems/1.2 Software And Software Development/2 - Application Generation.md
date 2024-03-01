
# Nature of Applications

- The two main parts that make up a computer system is the Hardware, and the Software
	- Hardware - The physical components used to make a Computer
	- Software - The programs / code that tells the hardware what to do

- Within this, there are generally two labels that software will normally fall under, that being - 
	- System Software - Software that keeps the computer running how it is supposed to
	- Application Software - Software that runs programs that the user wants to use, e.g. word processors, browsers etc.


# Open vs Closed Source Software

- Open source software means that the source code for the program is open to be viewed by the public, and people can modify and contribute to evolving the program. It is usually free. 
	- The OS "Linux" is open source, making it popular with programmers, as it is highly customizable, and community ran

- Closed source, or "proprietary" software is commercialised, the source code is kept from the user, and to be used, you must buy a license.
	- Microsoft's "Windows" is proprietary, and you have to buy a license to use it.


# Translators

There are a few different types of translators, but the main idea behind them is to break down code into machine code so that it can be properly processed by the computer.

## Assembler 

- Convert assembly code to machine code

## Compiler

- Compilers take the entire script, and processes it in one go, making one executable file, meaning that if there is a mistake in the code, the file will not run when opened.

## Interpreter

- Interpreters process the script, line by line, during the runtime. This means that as the code is run, it will proceed with running the script until there is an error, meaning that it can output data, and then stop running due to an error.

# Stages of Compilation

- High level languages are designed to be easy for us, the programmer to read, making it close to English.
- Processors cannot run source code like that, computers can only process binary, so we need to turn high level languages to machine code, through a compiler.

- There are 4 Stages of Compilation:
	1) Lexical Analysis
	2) Syntax Analysis
	3) Code Generation
	4) Code Optimisation

## Lexical Analysis

- The lexer starts by converting lexemes in the source code into a series of tokens.
- As the lexer reads the source code, it is scanned letter by letter
- When white space, an operator, or a special symbol is found, it decides that a word (lexeme) is complete.
- It then checks if that lexeme is valid, by using a predefined set of rules that allow every lexeme to be identified as a valid token
- Keywords, constants, identifiers, strings, operators and punctuation symbols are all considered tokens.

- In summary, In Lexical Analysis:
	- Comments and white space is removed
	- Remaining code is turned into a series of tokens
	- Symbol Table is created to keep track of variables and subroutines

## Syntax Analysis

***FINISH THE REST OF THE NOTES FOR EACH STEP***





- In summary, in Syntax Analysis:
	- Abstract syntax tree is built from tokens produced in the previous stages.
	- Errors generated if any tokens break the rules of the language.







## Code Generation





- In summary, in Code Generation:
	- Abstract code tree converted to object code
	- Object code is the machine code produced before the final step (linker) is run.


## Optimization





- In summary, in Optimization:
	- Tweaks the code, so that it will run as quickly, and use as little memory as possible.


# Linkers and Loaders

- A library is a ready compiled and tested program that can be run when needed
	- E.G. the built-in Math library in Python

- Windows uses Dynamic Link Libraries (DLL), which contain sub-routines written to complete a commonly used task on the operating system.
	- E.G. Save As

- The pros of using library routines are
	- It is quick and easy to connect to your own code
	- Pre-tested, so there will be pretty much no errors
	- Pre-compiled, so they are quite optimised
- The cons are
	- Adding functionality / tweaks can be difficult / impossible
	- Sometimes you are "black boxed" from the actual implementation
	- You have to trust the developers will continue to maintain the library

## Linkers

- The Linker is responsible for putting the appropriate machine addresses in all the external call and return instructions, so that all external library routines are linked together correctly.
- There are two methods to pull in the library that the code needs:
	- ***Static Linking***: All required code required from libraries are added into finished machine code, resulting in a large executable file.
	- ***Dynamic Linking***: Compiled versions of the libraries are stored on the host computer, and links in the required code from the libraries during runtime, cutting down on the file size.
		- This can cause issues if the libraries change, however, as routines may be called incorrectly.


## Loaders 

- The loader is the part of the OS that loads the EXE file into memory, ready to be run
	- When using Dynamic Linking it also handles loading the required libraries into memory

