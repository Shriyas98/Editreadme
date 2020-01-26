# EE577A Lab 1 Part 1
## Description
In Lab1 Part 1 of EE577A, we were assigned three tasks to be performed using Python scripting. The objective of this lab is to get us familiar with Python scripting which is used in industry for various simulation and automation steps of design and verification.

## Task 1
A Python script (lab1p1.py) that reads the sample input text file text_in.txt. The file includes special characters and numbers. The script then writes every word in text_in.txt into an output file text_out1.txt with the following requirement: for each paragraph in text_in.txt, you should rewrite the words in the paragraph in reverse order.

### Comments of the Code for Task 1
Open the input text_in.txt in r+ mode and read it.
Asssign an empty list 'paragraph' and an empty variable 'para'.
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
Generate the output after using join function in an output file named 'text_out1.txt'.

## Task 2
Analyze all the words, compute the word length distribution in the text file
text_in.txt and generate a format displaying Word Length and Count.
Open the input text_in.txt in r+ mode and perfrom split and read on it.
Use max function to find the maximum word length.
line 46 and 48 includes the representation of a table format.
According to the format showed in question we have taken a padding of approx 20.
Generate the output into a new text file named 'text_out1.txt'.

## Task 3
Encrypt each word of the text in text_in.txt with a simple text encryption scheme
as follows. For each character in the word, find its ASCII code (you may use ord() in your
Python scrypt), denoted by �����%&'(')*+. For example, the ASCII code of the character ‘a’ is 97,
while the ASCII code of the character ‘3’ is 51. The ASCII code of the encoded character, denoted
by �����,)-%.,., follows the formula below:
�����,)-%.,. = 01�����%&'(')*+ − 33 + �6 ��� 94= + 33






Line 48 is https://stackoverflow.com/questions/9989334/create-nice-column-output-in-python
