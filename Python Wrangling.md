#python #ASCII 

![[Pasted image 20230815165508.png]]

## Quick solution:
![[Pasted image 20230815165609.png]]

## Solution -v:
First step I like to take after downloading the files, is to find out more about these files we're given, so let's run a file command
	$ file ende.py && file flag.txt.en && file flag.txt
![[Pasted image 20230815174325.png]]
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
Paste (*Ctrl + shift + v*) 'ac9bd0ffac9bd0ffac9bd0ffac9bd0ff' & hit enter
And there's the flag:
![[Pasted image 20230815175634.png]]

### Arguments for running python3:
![[Pasted image 20230815175713.png]]

