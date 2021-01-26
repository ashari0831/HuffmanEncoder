# Making Huffman Tree with java and compress a text file
## Overview
This app is created for my university project and it includes Huffman Tree code which help us to compress text files.
 
## Features
- This app get your text file address and compress it into a .cmp file.
- This app store the Huffman tree in the cmp file with Json.
- It uses Gson class in google library to work with Json.
- Also it can decompress the cmp file and give you the recent text.

**Note:** If you want to know how to add Gson library to your IDE, check this video on Youtube:
[Watch Now](https://www.youtube.com/watch?v=HSuVtkdej8Q&t=245s)

## Explanation for classes and methods
- This is a static class for nodes which also Overriding compareTo method for comparing nodes:

>static class Node implements Comparable<Node> {}


- This help us arrange nodes in a increasing order

>static Node buildTree(int[] freq) {}

- This is for aski codes and characters

> static int ALPHA_SIZE = 256;

- this will encode the tree including chars and frequencies

> public EncodedResult compress(String data) {}

- this will decode the encoded data and give us the text

> public String decompress(EncodedResult result) {}

- it counts number of each char in the string

> static int[] buildFrequencyTable(String data) {}
