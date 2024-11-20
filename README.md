Huffman Coding Compression and Decompression
This project implements Huffman Coding, a popular algorithm for lossless data compression. The code provides functionalities to compress and decompress text files using Huffman Coding.

Features
Compression: Reads a text file, generates Huffman codes, and writes the compressed data to an output file.
Decompression: Reads the compressed file, decodes it using the stored Huffman codes, and writes the original text to a decompressed file.
How It Works
Character Frequency Count: Reads the input file and counts the frequency of each character.
Min-Heap Construction: Builds a min-heap (priority queue) of nodes where each node represents a character and its frequency.
Huffman Tree Construction: Constructs the Huffman tree by repeatedly merging the two nodes with the smallest frequencies.
Huffman Code Generation: Generates the Huffman codes for each character by traversing the Huffman tree.
Compression: Encodes the input text using the generated Huffman codes and writes the encoded data along with the Huffman codes to an output file.
Decompression: Reads the compressed file, reconstructs the Huffman codes, decodes the encoded data, and writes the original text to a decompressed file.
How to Use
Prerequisites
Ensure you have a C++ compiler installed, such as g++.
Steps to Use
Clone the Repository:

git clone https://github.com/ShashankBhushan007/file-compressor.git
cd file-compressor
Compile the Program:

g++ -o file-compressor code.cpp
Run the Program:

./file-compressor
Choose an Option from the Menu:

Enter 1 to compress a file.
Enter 2 to decompress a file.
Follow the Prompts:

For compression, enter the filename of the text file you want to compress. The compressed output will be saved as output.txt.
For decompression, enter the filename of the compressed file (e.g., output.txt). The decompressed output will be saved as decompressed.txt.
Notes
Ensure the file to be compressed or decompressed is in the same directory as the compiled program.
The compressed file (output.txt) contains the Huffman codes and the encoded text.
The decompressed file (decompressed.txt) will contain the original text.
Repository
