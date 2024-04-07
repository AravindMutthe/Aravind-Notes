# 1. General Purpose Utility commands in Linux

- **cat**: Concatenate and display file content.
- **date**: Display or set the system date and time.
- **echo**: Display a line of text/string.
- **printf**: Format and print data according to specified format.
- **bc**: Basic calculator utility.
- **script**: Record a terminal session.

# 2. Email Basics

- **mailx**: Command-line utility for sending and receiving emails.
- **passwd**: Utility for changing user password.
- **who**: Display information about users who are currently logged in.
- **username**: Command to display the current username.
- **tty**: Print the file name of the terminal connected to standard input.
- **stty**: Change and print terminal line settings.

# 3. File management commands

#### File handling

- **cat**: Concatenate and display file content.
- **cp**: Copy files and directories.
- **rm**: Remove files or directories.
- **more**: Display file content one screen at a time.
- **file**: Determine file type.
- **wc -l, -w, -c**: Count lines, words, or bytes in a file.
- **od**: Dump files in various formats.
- **cmp**: Compare two files byte by byte.
- **comm**: Compare two sorted files line by line.
- **diff**: Compare files line by line.
- **gzip & gunzip -r, -d**: Compress and decompress files recursively.
- **tar -c, -x, -t**: Create, extract, or list files from a tar archive.
- **zip & unzip**: Compress and decompress files in ZIP format.
- **find**: Search for files in a directory hierarchy.
- **unmask**: Set default file permissions.

# 4. Create a file in Linux

- **touch**: Create an empty file or update file timestamps.
- **cat >**: Create or concatenate files and redirect output.
- **vi**: Text editor for creating or editing files.
- **vim**: Improved version of vi editor.
- **nano**: Simple text editor for creating or editing files.

# 5. Filters (to search)

##### Filtering using Regular Expressions

1. **grep**:

- Search for patterns in files.
- used to find words, text strings, number strings, or any other information in a single file or multiple files.

> **syntax :**  grep [options] word|”string” filename1 filename2

- options
    -i Ignore case in search results.
    -w Find only the whole words.
  - -n Display line number for matching lines.
  - -r Perform recursive search.
  - -l Print only the file names.
  - -c Show only a count of the number of matches.
  - -color Highlight matched string in different colors.

    > **ex: grep Linux sample.txt**

2. **egrep**: Extended version of grep with more powerful regex support.
3. **sed**: Stream editor for filtering and transforming text.

# 6. Advanced Filters

#### 6. awk

- Powerful text processing tool for manipulating data and generating reports.
- awk is a command-line utility as well as a scripting language.
- that is used to manipulate data and format output reports.
- This command supports several variables, functions, and logical operators to get the desired output.

    >  ***awk [options] 'selection_criteria {action}' input-file > output-file***

# 7. Filters

- **pr**: Paginate or format files for printing.
- **head**: Display the beginning of a file.
- **tail**: Display the end of a file.
- **cut**: Extract sections from each line of files.
- **paste**: Merge lines of files.
- **sort**: Sort lines of text files.
- **uniq**: Remove duplicate lines from a sorted file.
- **tr**: Translate or delete characters.

# 8. Linux commands classified into 2 categories

##### Internal (Shell) commands

- Built-in commands of the shell.
- Accessed directly from the shell environment.

##### External (Kernel) commands

- Executable programs stored in specific directories (/bin or /sbin).
- Accessed via the shell by searching the directories listed in the PATH variable.

***"type" is used to find out whether a command is internal or external?***
> **Example: type cd**

# 9. How to control System and Services on a system running systemd

- **systemctl**: Utility for controlling systemd system and service manager.
- **Systemd**: A collection of system management daemons, utilities, and libraries serving as a replacement for System V init daemon.

# 10. Mounting

Mounting refers to making a group of files in a file system structure accessible to users by attaching a root directory from one file system to that of another. It can be local or remote, where local mounting connects disk drivers to behave as a single logical system, and remote mount uses NFS (Network File System) to connect directories on other machines.

# Ubuntu:

* Ubuntu is an open source Linux operating systems that runs on desktops, laptops, server and other devices…

* On Ubuntu, applications are available in two formats:

    1. Snap packages
    2. Debian packages.

* If an app is available in both formats, Ubuntu Software list the snap apps first.


# Uninstall Packages via Command Line

1. list all installed package
 >  sudo apt list --installed
2. To remove a package you find on the list
 >  sudo apt remove package_name
3. To uninstall multiple packages
 > sudo apt remove package_name_1 package_name_2
4. To completely remove packages and their configuration settings file
 > sudo apt purge package_name
5. to list snap packages
 >snap list
6. to remove snap packages
 > sudo snap remove package_name

