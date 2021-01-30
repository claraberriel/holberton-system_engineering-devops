I/O Redirections

Standard output (stdout) = 1
Standard error (stderr) = 2
Standard input (stdin) = 0

2 and 1 linked to the screen and not saved into a disk file
0 attached to the keyboard

* 1 — > to redirect, >> to append. It rewrites so if nonexistent source, file will be empty

* To redirect stderr, use notation 2 before >

* To redirect both 2 and 1 use (older versions): 
[command] [source] > [filename] 2>&1
Here the order is important, 2 before 1
Or (bash):
[command] [source] &> [filename]

* To suppress error messages:
[command] [source] 2> /dev/null

* Stdin <
