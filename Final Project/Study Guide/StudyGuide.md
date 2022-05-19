
---
Name: Menna Elgayar
Class: Cis 106
Semester: Spring 22
---

# STUDY GUIDE

-----

## Command name

**date**

### Description

is used to display the current time in the given FORMAT, or set the system date.

## Syntax

`date + OPTIONS `

## Example

* Display time described by string
  * `date -d`
* Display the last modification time of FILE
  * `date -r`
* Print or set coordinated universal time (utc)
  * `date -u`


## Command name

**uname**

### Description

Is used to print certain system information

## Syntax

`uname + OPTIONS `

## Example

* Print all information in the following order
  * `uname -a`
* Print the operating system
  * `uname -o`
* Print the kernel name
  * `uname -s`


## Command name

**du**

### Description

Summarize disk usage of the set of FILEs, recursively for directories.

## Syntax

`du + OPTIONS + FILE `

## Example

* print sizes in human readable format
  * `du -h ~/Documents/`
* scale sizes by SIZE before printing them
  * `du -B Documents/`
* skip directories on different file systems
  * `du -x Documents/`


## Command name

**free**

### Description

Can be used to show total memory, used memory, free memory, shared memory, and available memory about RAM and swap space.

## Syntax

`free + OPTIONS`

## Example

*  show output in bytes
   * `free -b`
* show total for RAM + swap
  * `free -t`
*  show human-readable output
   * `free -h`


## Command name

**echo**

### Description

Is used to display a line of text that is passed in as an argument.

## Syntax

`echo + OPTIONS `

## Example

* Do not output a trailing newline.
  * `echo -n`
* Enable interpretation of backslash escape sequences
  * `echo -e`
* Disable interpretation of backslash escape sequences 
  * `echo -E`


## Command name

**apt**

### Description

Is a command line package manager and provides commands for
searching and managing as well as querying information about packages.


## Syntax

`apt + OPTIONS`

## Example

* search in package descriptions
  * `apt search`
* install packages
  * `apt install`
* update list of available packages
  * `apt update`


## Command name

**pwd**

### Description

Print the name of the current working directory.


## Syntax

`pwd + OPTIONS`

## Example

*  print the value of $PWD if it names the current working directory
   * `pwd -L`
* print the physical directory, without any symbolic links
  * `pwd -P`



## Command name

**cd**

### Description

Is used to change the shell working directory.


## Syntax

`cd + DESTINATION`

## Example

* to go to your home directory
  * `cd $home`
* to go to your previous directory
  * `cd `
* to go to your documents file
  * `cd ~/Documents/`


## Command name

**ls**

### Description

List information about the files

## Syntax

`ls + OPTIONS + FILENAME `

## Example

*to list contents of a directory or given file itself 
  * `ls ~/Documents/`
* to list all the files inside a current working directory
  * `ls -a`


## Command name

**tree**

### Description

Is a recursive directory listing command or program that produces a depth-indented listing of files

## Syntax

`tree + DESTINATION`

## Example

* All files are listed
  * `tree -a`
* List directories only.
  * `tree -d`
* Print the full path prefix for each file.
  * `tree -f`



## Command name

**man**

### Description

Is used to display the user manual of any command that we can run on the terminal

## Syntax

`man + OPTIONS + SECTIONS`

## Example

* search for text in all pages
  * `man -K`
*  use manual pages from other systems
  * `man -m`



## Command name

**mkdir**

### Description

Is used for creating a single directory or multiple directories

## Syntax

`mkdir + DIRECTORY NAME`

## Example

* create a directory in a present working directory
  * `mkdir wallpapers`
* create a directory in a different directory 
  * `mdkir wallpapers/ocean`
* create multiple directories
  * `mdkir wallpapers/cars wallpapers/sunsets`



## Command name

**touch**

### Description

this command is used to create files

## Syntax

`touch + FILE NAME`

## Example

* to create a file called flowers
  * `touch flowers`
* to create several files
  * `touch cars sunsets`



## Command name

**rm**

### Description

this command is used to remove files and also directories only with (-r)

## Syntax

`rm + FILE NAME`

## Example

* remove a file names sunsets
  * `rm sunsets`
* remove a file with confirmation
  * `rm -i sunsets`
* remove a non empty directory
  * `rm -r Downloads/games`



## Command name

**cp**

### Description

Copy a source to a destination, or multiple sources

## Syntax

`cp + OPTIONS + SOURCE + DESTINATION `

## Example

* to copy a directory to a destination
  * `cp -r Downloads/Books Documents`
* to copy a file
  * `cp Downloads/wallpaper.jpeg Pictures/`



## Command name

**mv**

### Description

Is used to move and rename directories

## Syntax

`mv + SOURCE + DESTINATION`

## Example

* to move a file from a directory to another
  * `mv Downloads/cat.jpeg Pictures/`
* to rename a file
  * `mv dracula.jpeg alucard.jpeg`
* to move and rename a file in one command
  * `mv Downloads/dracula.jpeg Pictures/alucard.jpeg`



## Command name

**stat**

### Description

Display file or file system status.

## Syntax

`stat + OPTIONS + FILE`

## Example

* display file system status instead of file status
  * `stat -f ~/Wallpapers`



## Command name

**Wildcards (*,?,[])**

### Description

wildcards represent letters and characters used to specify a file name for searches



## Command name

**Brace expansion**

### Description

Is used to create a whole directory structure in a single command


## Example

`mkdir -p Videos/{dogs,cats}/{breed,adoption,names}`



## Command name

**cat**

### Description

Concatenate files to standard output

## Syntax

`cat + OPTIONS + FILE`

## Example

* display the content of a file located in the pwd
  * `cat horses.jpeg`
* display the content of a file with line numbers
  * `cat -n ~/Documents/horses`



## Command name

**head**

### Description

Print the first 10 lines of each FILE to standard output.


## Syntax

`head + OPTIONS + FILE`

## Example

* display the first 10 lines of a file
  * `head ~/Documents/resume.txt`
* display the first 5 lines of a file
  * `head -5 ~/Documents/resume.txt`



## Command name

**tail**

### Description

Print the last 10 lines of each FILE to standard output

## Syntax

`tail + OPTIONS + FILE`

## Example

* display the last 10 lines of a file
  * `tail ~/Documents/resume.txt`
* display the last 5 lines of a file
  * `tail -5 ~/Documents/resume.txt`



## Command name

**cut**

### Description

Print selected parts of lines from each FILE to standard output

## Syntax

`cut + OPTIONS + FILE`

## Example

* display a list of all users from your system
  * `cut -d ":" -f1 /etc/passwd`
* display a list of all users from your system with their login shell
  * `cut -d ":" {print f1,7} /etc/passwd`



## Command name

**tr**

### Description

Translate, squeeze and/or delete characters from standard input

## Syntax

`Standard Input | tr + OPTION + SET + SET `

## Example

* Translate one character to another
  * `cat file.txt | tr ',' '.'  `


## Command name

**paste**

### Description

write lines consisting of the sequentially corresponding lines from each file

## Syntax

`paste + OPTIONS + FILE`

## Example

* merge two files
  * `past cake.lst guests.lst`
* merge two files using a different delimeter
  * `paste -d ":" cake.lst guests.lst`
  * 


## Command name

**wc**

### Description

is used for printing the number of lines, characters  and bytes in a file 

## Syntax

`wc + OPTIONS + FILE`

## Example

* display a number of characters in a file 
  * `wc -m ~/Downloads/Books/HarryPotter`
* display the number of lines in a file
  * `wc -l ~/Downloads/Books/HarryPotter`
* Display the number of words in a file
  * `wc -w ~/Downloads/Books/HarryPotter`



## Command name

**grep**

### Description

Is used to search a text in a given file

## Syntax

`grep + OPTIONS + search criteria + FILE`

## Example

* search for any line that contains the word "harry" in the given file
  * `grep 'harry' ~/Downloads/Books/HarryPotter.txt`
* search for any lime that contains the word "harry" regardless of the case
  * `grep -i 'harry" ~/Downloads/Books/HarryPotter.txt`


