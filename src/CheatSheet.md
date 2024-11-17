# Cheat-Sheet
Before you solely rely on this cheat-sheet, **try to gather own information** about the commands with the use of the man-pages or the "help" command (like this: **"\<command\> --help"** or **"man \<command\>"**)
## Commands
#### ssh
`ssh <username>@<ip_address>`

> `-p <port>` Specify a port
> `-i <keyfile>` Use a keyfile for authentication

<sub>Ssh (SSH client) is a program for logging into a remote machine and for executing commands on a remote machine.</sub>
#### exit
<sub>Closes the current shell or ssh connection.</sub>
#### task
`task`
<sub>Prints the task of the current level.</sub>
#### hint
`hint`
<sub>Gives a hint for the current level.</sub>
#### man
`man <command>`
<sub>Provides an in-depth description of a command and its usage.</sub>
#### ls
`ls <directory_path>`

> `-a` Get all files
> `-l` List properties

<sub>List information about the FILEs (the current directory by default).</sub>
#### cat
`cat <file1> <file2> ...`
<sub>Prints the content of a file to the terminal output.</sub>
#### cd
`cd <directory_path>`

> `~` Go to home directory
> `..` Go one directory up

<sub>With this command you can change directories.</sub>
#### find
`find <directory_path>`

> `-name <file/directory name>` Search for name
> `-size <size>[c,b,n]` Search for size [c: Bytes, d: 512-Byte Block, n: default]
> `-user <username>` Search for owner username
> `-group <groupname>` Search for owner group name

<sub>Searches the provided directory (and child directories) for matching parameters (size, owner, name, etc.).</sub>
#### grep
`grep <pattern>`
<sub>Searches for a pattern in a file or from the terminal output.</sub>
#### uniq
`uniq`
<sub>Filters adjacent matching lines from files or the terminal input. (Filters out multiple occurrences)</sub>
#### sort
`sort`
<sub>Sort terminal output/files (alphabetically, numerically, etc.).</sub>
#### base64
`base64 <file>`

> `-d` Decode

<sub>Encode/decode strings/files with base64.</sub>
#### tr
`tr <from> <to>`
<sub>Translate a string from terminal input/files with a given string. (E.g. use a custom alphabet)</sub>
#### john
`john --wordlist=<wordlist> <hashfile>`

> `--show <hashfile>` Show result of cracked hash.

<sub>Crack hashes using a brute force-attack.</sub>
#### strings
`strings <binary_file>`
<sub>Search for printable strings inside a binary.</sub>
#### nc
`nc <address> <port>`
<sub>Network tool to establish connections on a lower layer.</sub>
#### tar
`tar <flags> <file/folder/archive>`

> `-xf` Unpack archive
> `-cf` Pack archive

<sub>Create archive from files/folders or unpack archives to receive files.</sub>
#### gzip
`gzip <file/folder/archive>`

> `-d` Decompress archive

<sub>Compress/uncompress files/folders.</sub>
#### curl
`curl <URL>`

> `-I` Print just the HEADER
> `-i` Include the HEADER

<sub>Network tool for transferring data from/to servers using URLs.</sub>
