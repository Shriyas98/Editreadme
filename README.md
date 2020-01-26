# EE577A Lab 1 Part 1
## Description
In Lab1 Part 1 of EE577A, we were assigned three tasks to be performed using Python scripting. The objective of this lab is to get us familiar with Python scripting which is used in industry for various simulation and automation steps of design and verification.

## Task 1
A Python script (lab1p1.py) that reads the sample input text file text_in.txt. The file includes special characters and numbers. The script then writes every word in text_in.txt into an output file text_out1.txt with the following requirement: for each paragraph in text_in.txt, you should rewrite the words in the paragraph in reverse order.

### Comments of the Code for Task 1
Open the input text_in.txt in r+ mode and read it.
Asssign an empty list 'paragraph' and an empty varaible 'para'.
Use while loop to iterate through the contents of the input file.
We have used 3 cases to define if its a next line or end of a paragraph or not.
##### if condition
This is for a next line only, when nothing is to be done.
##### elif condition
This is for the end of paragraph where we actually have to reverse the the paragraph.
The end of paragraph is identified if it ends with a '.' or '?' and with a space and next line.
##### else condition
If its not from the above conditions, just iterate through the file.

Then use split function and reverse it from the last word using b=b[::-1]
Generate the output after using join function in an output file named text_out1.txt.


