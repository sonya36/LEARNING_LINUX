# Day 1 
## COMMAND:
- A command is a software program that when executed on the CLI (command line interface), performs an action on the computer. When you type in a command, a process is run by the operating system that can read input, manipulate data and produce output. A command runs a process on the operating system, which then causes the computer to perform a job.
- Case-Sensitive
    ### Syntax
    ```
    command [option..] [arguments]
    ```
    - options : to alter the behavior of the command. 
    - arguments : are items or values for the command to act upon.

## List of Command
- ls : to return a list of files contained within the current directory.
    - no options and arguments, only command.
        ```
        ls
        ```
    - with argument,  list the content of the directory provided as an argument. 
        ```
        ls Documents
        ```
    - with option, -l :  which results in a "long display" output, meaning the output gives more information about each of the files listed
        ```
        ls -l
        ```
    - By default, the ls command prints the results in alphabetical order, so adding the -r option will print the results in reverse alphabetical order.
        ```
        ls -r
        ```
    - Multiple options can be used at once, either given as separate options as in -l -r or combined like -lr. The output of all of these examples would be the same:
        ```
        ls -l -r
        ls -rl
        ls -lr
        ```

   
- aptitude : pacakage management tool avilable on some linux distributions. This command will accept moo as an argument.
    - argument : moo
        ```
        aptitude moo
        ```
    - option : -v
        ```
        aptitude -vv moo
        aptitude -v moo
        ```
- pwd : prints the working directory, your current location within the filesystem.
    ```
    pwd
    ```

- cd : to change directory
    ```
    cd [options] [path]
    ```
    
    - Directories are equivalent to folders on Windows and Mac OS. Like these more popular operating systems, a Linux directory structure has a top level. It is not called "My Computer", but rather the root directory and it is represented by the / character. To move to the root directory, use the / character as the argument to the cd command.
        ```
        cd / 
        ```
    - The argument to the cd command is more than just the name of a directory, it is actually a path. A path is a list of directories separated by the / character. For example, /home/sysadmin is the path to your home directory:
        ```
        cd /home/sysadmin
        ```
        Note : 
        - An absolute path allows us to specify the exact location of a directory. It always starts at the root directory, therefore it always begins with the / character. The path to the home directory /home/sysadmin is an absolute path. The path begins at the root / directory, moves into the home directory, and then into the sysadmin directory.
        - A relative path gives directions to a file relative to your current location in the filesystem. Relative paths do not start with the / character, they start with the name of a directory. 
            ```
            cd Documents
            ```
    - .. Characters : Regardless of which directory you are in, .. always represents one directory higher relative to the current directory, sometimes referred to as the parent directory.
        ```
        cd ..
        ```
    - . Character : Regardless of which directory you are in, the . character always represents your current directory. For the cd this shortcut is not very useful, but it will come in handy for commands covered in subsequent sections.
    - ~ Character : The home directory of the current user is represented by the ~ character. As stated above, you always begin as the sysadmin user, whose home is located at /home/sysadmin. To return to your home directory at any time execute the following command:  
        ```
        cd ~
        ```
