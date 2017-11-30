# CS610

Compression algorithm which implements Huffman coding.

***WARNING***: Passing a file as an argument to HuffmanEncode will **remove the file** and replace it with a new file with the extension '.huf'. I am **not** responsible for any lost files.

	(+) File added
	(-) File removed

For this reason, it is **HIGHLY** recommended that you create a copy of the file to test this program.

	(command) copy originalFile.txt copyOfFile
 	+copyOfFile

(1) Compile both .java files:

	(command) javac HuffmanEncode.java  
 	(command) javac HuffmandDecode.java  

(2) Pass a file as an argument to HuffmanEncode:

	(command) java HuffmanEcode copyOfFile
	-copyOfFile
	+copyOfFile.huf

(3) Pass newly generated '.huf' file to to HuffmanDecode:

	(command) java HuffmanDecode copyOfFile.huf
	-copyOfFile.huf
	+copyOfFile

(4) You can compare these files to assure that the contents are the same after decompression:

	(Windows - command) FC originalFile.txt copyOfFile
	(Linux - command) diff originalFile.txt copyOfFile
	
---Alternatively, you can compare the MD5 hashes on Linux to assure these files are the same---
  
	(Linux - command) md5sum originalFile.txt copyOfFile
