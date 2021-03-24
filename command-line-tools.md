# Shell command line tools

`pwd`       - Print working directory  
`cd`        - Change directory
`ls`        - List directory  
`ls -lS`    - Sorted by size (descending)  
`ls -ltr`   - Sorted by modification date (oldest first)  
`~`         - Shortname of /home/$USER  
`cd ..`     - CD upper directory  
`.`         - Means the current directory where you are in  
`touch`     - Create a file or change the times for existing file  
`cat`       - Concatenate several files into the target file  
`mkdir -p`  - Create directories recursively  
`mv -i`     - Move or rename files and directories  
`rm -rv`    - Remove files/dirs recursively in verbose mode  
`man -k`    - Search for manual containing a search string  
`cp -viR`   - copy file/dir recursively in interactive & verbose mode  

echo "`man nano`" > nano-manual.txt - Saves formating (tabs and spaces)

## vi shortcuts

ESC:w (to save doc)  
ESC:q (just quit)  
ESC:wq (save and quit)  
ESC:wq!  

## Pipes and Redirection  
program_1 | program_2  
"|" - Pipe takes the STDOUT(0) from program_1 and redirects to program_2 STDIN(1)  
`ps aux | less`




```bash
:~$ echo "hello world" # "hello world" passed to STDIN channel of the echo program
hello world <-- STDOUT channel
```
Every linux running process has 3 channels with corresponding numbers (file descriptors)  
STDIN  --> 0  
STDIN  --> 1  
STDERR --> 2  


`>`  - write to (same as `1>`)  
`>>` - append to  
`<`  - redirection to STDIN  
```bash
ls notexistingpath 2> error.txt # (redirection of STDOUT to file)
cat err.txt
ls: cannot access 'nonexist': No such file or directory
```
  
