# Feb-25-COS-Assignment-1
Assignment-1
a. Start by navigating to your home directory and list its contents. Then, move into a  directory named "LinuxAssignment" if it exists; otherwise, create it.  
Last login: Thu Feb 27 09:01:10 on console
vaishnavikulkarni@Vaishnavis-MacBook-Air ~ % cd ~

vaishnavikulkarni@Vaishnavis-MacBook-Air ~ % ls -l
total 0
drwx------+  5 vaishnavikulkarni  staff   160 Feb 14 17:27 Desktop
drwx------+  6 vaishnavikulkarni  staff   192 Feb 27 09:13 Documents
drwx------+ 19 vaishnavikulkarni  staff   608 Feb 27 09:58 Downloads
drwx------@ 97 vaishnavikulkarni  staff  3104 Feb 24 17:45 Library
drwx------   4 vaishnavikulkarni  staff   128 Nov 29 16:24 Movies
drwx------+  4 vaishnavikulkarni  staff   128 Nov 29 16:18 Music
drwx------+  4 vaishnavikulkarni  staff   128 Nov 27 15:29 Pictures
drwxr-xr-x+  4 vaishnavikulkarni  staff   128 Nov 27 15:27 Public
vaishnavikulkarni@Vaishnavis-MacBook-Air ~ % LinuxAssignment
zsh: command not found: LinuxAssignment
vaishnavikulkarni@Vaishnavis-MacBook-Air ~ % mkdir LinuxAssignment
vaishnavikulkarni@Vaishnavis-MacBook-Air ~ % cd LinuxAssignment
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % pwd
/Users/vaishnavikulkarni/LinuxAssignment

b) File Management: 
a. Inside the "LinuxAssignment" directory, create a new file named "file1.txt". Display its  contents.  
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % touch file1.txt

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l

total 0
-rw-r--r--  1 vaishnavikulkarni  staff  0 Feb 27 12:25 file1.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % cat file1.txt

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % echo "Hello,This is a test file for LinuxAssignment." > file1.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % cat file1.txt

Hello,This is a test file for LinuxAssignment.
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % echo "Hello, I am Vaishnavi Kulkarni, This is anew file in LinuxAssignment names as file1.txt" > file1.txt

c) Directory Management: 
a. Create a new directory named "docs" inside the "LinuxAssignment" directory.  

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % cd ~/LinuxAssignment

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % pwd

/Users/vaishnavikulkarni/LinuxAssignment
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % mkdir docs

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l

total 8
drwxr-xr-x  2 vaishnavikulkarni  staff  64 Feb 27 12:35 docs
-rw-r--r--  1 vaishnavikulkarni  staff  88 Feb 27 12:29 file1.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -ld docs

drwxr-xr-x  2 vaishnavikulkarni  staff  64 Feb 27 12:35 docs

d) Copy and Move Files: 
a. Copy the "file1.txt" file into the "docs" directory and rename it to "file2.txt". 

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % cd ~/LinuxAssignment

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % pwd

/Users/vaishnavikulkarni/LinuxAssignment
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % cp file1.txt docs/file2.txt

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l docs

total 8
-rw-r--r--  1 vaishnavikulkarni  staff  88 Feb 27 12:40 file2.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % cat docs/file2.txt

Hello, I am Vaishnavi Kulkarni, This is anew file in LinuxAssignment names as file1.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % 

e) Permissions and Ownership: 
a. Change the permissions of "file2.txt" to allow read, write, and execute permissions for  the owner and only read permissions for others. Then, change the owner of "file2.txt" to  the current user.  

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % cd ~/LinuxAssignment

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % chmod u=rwx,g=r,o=r docs/file2.txt


vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l docs/file2.txt

-rwxr--r--  1 vaishnavikulkarni  staff  88 Feb 27 12:40 docs/file2.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % 

f) Final Checklist: 
a. Finally, list the contents of the "LinuxAssignment" directory and the root directory to  ensure that all operations were performed correctly.  

vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l docs/file2.txt

-rwxr--r--  1 vaishnavikulkarni  staff  88 Feb 27 12:40 docs/file2.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l ~/LinuxAssignment

total 8
drwxr-xr-x  3 vaishnavikulkarni  staff  96 Feb 27 12:40 docs
-rw-r--r--  1 vaishnavikulkarni  staff  88 Feb 27 12:29 file1.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l ~/LinuxAssignment/docs

total 8
-rwxr--r--  1 vaishnavikulkarni  staff  88 Feb 27 12:40 file2.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l ~/LinuxAssignment/docs/file2.txt

-rwxr--r--  1 vaishnavikulkarni  staff  88 Feb 27 12:40 /Users/vaishnavikulkarni/LinuxAssignment/docs/file2.txt
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % ls -l /

total 10
drwxrwxr-x   9 root  admin   288 Feb 27 10:00 Applications
drwxr-xr-x  66 root  wheel  2112 Feb 24 09:08 Library
drwxr-xr-x@ 10 root  wheel   320 Nov 15 10:29 System
drwxr-xr-x   5 root  admin   160 Dec  4 15:33 Users
drwxr-xr-x   3 root  wheel    96 Feb 27 08:59 Volumes
drwxr-xr-x@ 39 root  wheel  1248 Nov 15 10:29 bin
drwxr-xr-x   2 root  wheel    64 Jul 11  2023 cores
dr-xr-xr-x   4 root  wheel  4792 Feb 27 08:59 dev
lrwxr-xr-x@  1 root  wheel    11 Nov 15 10:29 etc -> private/etc
lrwxr-xr-x   1 root  wheel    25 Feb 27 08:59 home -> /System/Volumes/Data/home
drwxr-xr-x   2 root  wheel    64 Jul 11  2023 opt
drwxr-xr-x   6 root  wheel   192 Feb 27 08:59 private
drwxr-xr-x@ 77 root  wheel  2464 Nov 15 10:29 sbin
lrwxr-xr-x@  1 root  wheel    11 Nov 15 10:29 tmp -> private/tmp
drwxr-xr-x@ 11 root  wheel   352 Nov 15 10:29 usr
lrwxr-xr-x@  1 root  wheel    11 Nov 15 10:29 var -> private/var
vaishnavikulkarni@Vaishnavis-MacBook-Air LinuxAssignment % 

g) File Searching: 
a. Search for all files with the extension ".txt" in the current directory and its subdirectories.  b. Display lines containing a specific word in a file (provide a file name and the specific  word to search).  


