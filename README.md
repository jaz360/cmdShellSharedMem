# cmdShellSharedMem
Creating custom command shell on Linux using System class and shared memory 
This project takes standard Linux commands eg. ls -l 
a child process is then created to run that command using shared memory as communication channel between parent and child process.
When the parent process receives the command from the user, it will create a buffer in the share memory area. 
The child process will copy the output of the command in the shared memory area and displays it to the user via Y/N to display the output.
