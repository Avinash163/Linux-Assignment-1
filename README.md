1. Creating and Renaming Files/Directories
Create a directory named test_dir using mkdir.
Inside test_dir, create an empty file called example.txt.
Rename example.txt to renamed_example.txt using mv

mkdir test_dir                                             # Created directory test_dir using mkdir
cd test_dir                                                # changed directory to test_dir using cd
touch example.txt			                                     # Created empty file(example.txt) using touch
mv example.txt renamed_example.txt                        # renamed file using mv



2. Viewing File Contents
Use cat to display the contents of /etc/passwd.
Display only the first 5 lines of /etc/passwd using head.
Display only the last 5 lines of /etc/passwd using tail.

Cat /etc/passwd                            #displayed content using cat
Head -n 5 /etc/passwd 		                 #Used head to show only first 5 lines
Tail -n 5 /etc/passwd                     #Used tail to show only last 5 lines



3.Searching for Patterns
Use grep to find all lines containing the word "root" in /etc/passwd.

cat /etc/passwd | grep "root"             
#output of cat command gives to grep using pipe and it filter out the line containing “root”



4. Zipping and Unzipping
Compress the test_dir directory into a file named test_dir.zip using zip.
Unzip test_dir.zip into a new directory named unzipped_dir.

zip -r test_dir.zip test_dir          # command for zip test_dir directory

Explanation
Zip : command to compress files/folders.
-r : Recursively zip the entire directory.
Test_dir.zip : Output zip file.
Test_dir: The directory you want to compress.
mkdir unzipped_dir                           # Create a directory to extract into.
unzip test_dir.zip -d unzipped_dir 
#Extracts the contents of test_dir.zip into the folder unzipped_dir.


5. Downloading Files
Use wget to download a file from a URL (e.g., https://example.com/sample.txt).

wget https://example.com/sample.txt
#wget command to download a file from the web, followed by the file URL


6. Changing Permissions
Create a file named secure.txt and change its permissions to read-only for everyone using chmod.

Chmod 444 secure.txt
#It will give only read(4) permission to all, not write(2) or execute(1)


7. Working with Environment Variables
Use export to set a new environment variable called MY_VAR with the value "Hello, Linux!".

export MY_VAR="Hello, Linux!"
#sets an environment variable named MY_VAR with the value "Hello, Linux!"
