# CDAC Batch Feb-25-COS-Assignment-1.

//This repository contains solutions for Linux OS practical problems, covering **file management, directory handling, permissions, networking, and text processing**.

----------     ----------       ----------       ----------      ----------     ----------     ----------      ----------     ----------    -------

Problem 1: Linux File and Directory Operations

a) Navigate and List**  
1. Navigate to the home directory and list its contents:  
   ```bash
   cd ~
   ls -l
2.Move into the LinuxAssignment directory (create if it doesn't exist):
mkdir -p LinuxAssignment
cd LinuxAssignment

b) File Management
Create a new file file1.txt and display its contents:
touch file1.txt
cat file1.txt

c) Directory Management
Create a new directory docs:
mkdir docs

d) Copy and Move Files
Copy file1.txt into docs and rename it to file2.txt:
cp file1.txt docs/file2.txt

e) Permissions and Ownership
-Change permissions of file2.txt (Owner: Read, Write, Execute; Others: Read only):
chmod 744 docs/file2.txt

-Change the owner of file2.txt to the current user:
chown $(whoami) docs/file2.txt

f) Final Checklist
-List contents of the LinuxAssignment directory:
ls -l LinuxAssignment

List the root directory contents:
ls -l /

g) File Searching
Search for all .txt files in the current directory and subdirectories:
find . -name "*.txt"

Display lines containing a specific word (example) in file1.txt:
grep "example" file1.txt

h) System Information
Display the current system date and time:
date


i) Networking
Display the IP address of the system:
ipconfig | grep "inet "

Ping a remote server (e.g., Google):
ping -c 4 google.com


j) File Compression
Compress the docs directory into a zip file:
zip -r docs.zip docs

Extract the contents into a new directory:
unzip docs.zip -d extracted_docs


k) File Editing
Open file1.txt in a text editor and add text:
nano file1.txt

Replace a specific word (oldword → newword) in file1.txt:
sed -i '' 's/oldword/newword/g' file1.txt

Problem 2: Text Processing and File Handling

a) Display the First 10 Lines of data.txt






