# Automate Project

## Description
This project implements a finite state automaton (FSA) parser and analyzer. It provides functionality to parse automata from files, generate visual representations, and process word recognition within the automaton.

## Features
- Parse automata from input files
- Generate `.dot` files for visualization
- Check if a word is recognized by the automaton
- Search for recognized words in a file

## Technologies Used
- C programming language
- Finite State Automaton (FSA) concepts
- Graph representation using adjacency lists
- File handling and parsing techniques

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/mbelouar/AutoTheory.git
   cd AutoTheory
   ```
2. Compile the source files using `make`:
   ```sh
   make (gen_dot_file / find_word / find_in_file)
   ```

## Usage
### Generate DOT File for Visualization
```sh
./gen_dot_file input.txt output.dot
```
- `input.txt`: Input file containing the automaton description
- `output.dot`: Generated Graphviz DOT file

### Check if a Word is Recognized
```sh
./find_word input.txt word
```
- `input.txt`: Input file with automaton data
- `word`: Word to check in the automaton

### Find Words in a File
```sh
./find_in_file input.txt words.txt
```
- `input.txt`: Input file with automaton data
- `words.txt`: File containing words to check

## File Structure
```
.
├── include
│   ├── automate.h  # Header file with struct and function definitions
├── src
│   ├── find_in_file.c       # Search for recognized words in a file
│   ├── find_in_file_main.c  # Entry point for file search
│   ├── find_word.c          # Recursive word recognition
│   ├── find_word_main.c     # Entry point for word checking
│   ├── get_dot_file.c       # Generate .dot files for visualization
│   ├── gen_main.c           # Entry point for .dot file generation
│   ├── parser.c             # Automaton parser implementation
├── Automations
│   ├── Automata1.txt             # Test file containing automaton and word data
|   ├── Automata2.txt
├── Makefile                 # Compilation instructions
└── README.md                # Documentation
```

## Contributing
Feel free to open issues and submit pull requests if you have improvements or bug fixes.

