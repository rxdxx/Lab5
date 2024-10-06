# CLI(Command Line Interface)-2

### I/O Redirection : Standard Output
- By default, standard output is screen.
- You can redirect output using ">" after a command (e.g., ls) to Create an save the output in a file.
- Commad "cat" displays the content of text file.
- Using ">>" appends output to an extising file(if it already exitsts), or create and write to a new file if it doesn't exist.
- By default, standard input is from keyboard.
- You can redirect input from a file using "<".
- You can mix "<" and ">" together in a single line.

### Pipelines "|"
- Pipeline feeds output of previous command to input of next command
- command1 | command2 | command3 | ...
*Press "q" key to exit the screen.

### Expansion
- Special characters expand its meaning when given to shell commands.

### Permissions
- Linux is a multi-user system.
- Files and directories have a permission assigned differently to owner/group/others.

### Changing Permission
- "chmod" changes permissions.

|Value|Meaning|
|:---|:---|
|777|**(rwxrwxrwx)** No restrictions on permissions. Anybody may do anything. Generally not a desirable setting.|
|755|**(rwxr-xr-x)** The file's owner ay read, write, and execute the file. All others may read and execute the file. This setting is common for programs that are used by all users.|
|700|**(rwx------)** The file's owner may read, write, and execute the file. Nobody else has any rights. This setting is useful for grograms that only the owner may use and must be kept private from others.|
|666|**(rw-rw-rw-)** All users may read and write the file.|
|644|**(rw-r--r--)** The owner may read and write a file, while all others may only read the file. A common setting for data file that everybody may read, but only the owner may change.|
|600|**(rw-------)** The owner may read and write a file. All others have no rights. A common setting for data files that the owner wants to keep private.|

### Superuser
- A superuser has all system administation authority.
- Some commands needsuperuser's privilleges.
- Put "sudo" before the command if you are a superuser.
- Type "exit" to get out of a superuser session.
---
- wget : download files from the internet directly to your active directory.
- curl : fetching, uploading, and managing date over the Internet curl [options][URL].
- 'grep'(Global Regular Expression Print) for searching text within files.
- grep "search_term" file.txt
  - Searches for the exact "search_term" within "file.txt" and prints matching lines.
- **Common Options : **
  - '-i' : Case-insensitive search (finds "apple" and "Apple").
  - '-v' : Invert the match (finds line *not* containing the search term).
  - '-n' : Display the line numbers along with matching lines.
  - '-r' : Recursive search (searches through all files in a directory and its subdirectories).
- 'grep' supports powerful regular expressions for more complex searches.
  - '.\*' : Matches any character ('.') zero or more times ('\*').
  - '\\d' : Matches any digit (0-9).
  - '[abc]' : Matches any single character within the brackets.
  - '^' : Matches the beginning of a line.
  - '$' : Matches the end of a line.
---
### Tip :
- Backslash; Backslah can be used to ignore line change in command ("enter"), to enter a long command in multiple lines.
- History; Type "history" to see previous command history or, save it to a text file.
