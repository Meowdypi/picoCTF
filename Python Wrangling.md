#python #ASCII 
# Python Wrangling

![Pasted image 20230815165508](https://github.com/Meowdypi/picoCTF/assets/122643833/f12fbc72-2a43-4869-a303-8b97c4037b25)

## Quick solution:

![Pasted image 20230815165609](https://github.com/Meowdypi/picoCTF/assets/122643833/0cea8a6a-a784-4ce1-9b84-e70494df04ce)

## Solution -v:
First step I like to take after downloading the files, is to find out more about these files we're given, so let's run a file command:
	
	$ file ende.py && file flag.txt.en && file flag.

![Pasted image 20230815174325](https://github.com/Meowdypi/picoCTF/assets/122643833/dd1febc1-5964-4ea3-b9d2-bfc04bbb77a8)


We're can see we're given: 
1. ende.py - a Python script that executes ASCII
2. flag.txt.en - an ASCII text file
3. flag.txt a text file containing the password.


To find the password we can cat the pw.txt file:

	$ cat pw.txt
	
Copy the output 'ac9bd0ffac9bd0ffac9bd0ffac9bd0ff' (using *ctrl + shift +c*)
![[Pasted image 20230815175514.png]]


Next, we can run ende.py, with -d for 'debug', and add flag.txt.en as the ASCII target file 

	$ python3 ende.py -d flag.txt.en


Paste (*Ctrl + shift + v*) 'ac9bd0ffac9bd0ffac9bd0ffac9bd0ff'

And there's the flag:
![[Pasted image 20230815175634.png]]


### Arguments for running python3:
![[Pasted image 20230815175713.png]]

