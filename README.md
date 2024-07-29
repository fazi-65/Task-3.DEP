# Task-3.DEP
File Compression Tool
Overview
This project implements a simple file compression and decompression tool using the Run-Length Encoding (RLE) algorithm. The tool allows users to compress text files by reducing consecutive character sequences and decompress them back to their original form.

Features
Compression: Reduces file size by encoding consecutive characters.
Decompression: Restores the original file from the compressed format.
File Handling: Supports reading from and writing to files.
Error Handling: Basic error handling for file operations.
Requirements
C++ Compiler (e.g., g++, clang++)
Standard C++ library
Installation
Clone the repository or download the source code files.

Open a terminal and navigate to the directory containing the source code.

Compile the program using the following command:

bash


Copy
g++ -o file_compressor file_compressor.cpp
Usage
Run the compiled program:

bash


Copy
./file_compressor
When prompted, enter the name of the input file you wish to compress. The program will create a compressed file with the same name as the input file, appended with .rle.

The program will then decompress the compressed file and create a new file prefixed with decompressed_.

Example
Assuming you have a text file named example.txt:

Input: example.txt
Compressed Output: example.txt.rle
Decompressed Output: decompressed_example.txt
File Format
Compressed File: The compressed file uses RLE, where each sequence of identical characters is represented by the count followed by the character (e.g., 4A represents AAAA).
Decompressed File: The decompressed file restores the original content.
Error Handling
The program includes basic error handling for file operations. If the input file cannot be opened, or if there are issues creating the output files, an error message will be displayed.

Limitations
The program currently handles only text files. Binary files may not be compressed correctly.
It assumes valid input for RLE encoding during decompression.
Edge cases, such as very large files or special characters, may require additional handling.
Future Improvements
Support for different file formats (e.g., binary files).
Enhanced error handling and logging.
Optimization for larger files and performance improvements.
User interface enhancements for better usability.
