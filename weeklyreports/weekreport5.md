# Week report 5

## A summary of the presentation
This week's presentation was about creating files and directories as well as how to move them, copy them or delete them using both the relative and absolute path.

## definition, usage, and example of the following commands:


| **Command** | **Usage** | **Example** |
|-------------|-----------|-------------|
| **mkdir**   | this command is used to create a single directory or multiple directories | mkdir + wallpapers |
| **touch** | this command is used for creating files | touch + flowers |
| **rm** | this command is used to remove a file  | rm + flowers |
| **rmdir** | this command can be used to remove an empty directory (to remove a non empty directory use rm -r) | rmdir + wallpapers |
| **mv** | this command is used to move as well as rename files/directories | *to move* > mv + Downloads/page1 Documents *to rename* > mv + report cis106report |
| **cp** | this command is used to copy files and directories from a source to a destination | cp + cis106hw cis106file |
|**ln** | this command is used to create a hard link or symbolic links to an existing file or directory | ln + file ~/Downloads/tes_file *symbolic link* > ln -s test_file1 test_file2 |
|**man** | this command displays the manual of a certain command, its executable programs, system calls etc. | man + ls |

## Brace expansion and how to use it

Brace expansion **{}** is a helpful method for generating lists of strings for usage in scripts, aliases, and the Linux command line. It helps you avoid errors and saving time by typing less. 

*COMMAND EXAMPLE*
**creating a whole directory structure in a single command**

mkdir -p + videos/{dogs,cats}/{breeds,adoption,names}


