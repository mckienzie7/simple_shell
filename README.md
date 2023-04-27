This is a project done by Lawrence Mupakurirwa from Zimbabwe in partnership with Talent Paul Paul from  Nigeria. This project is part of the required Cohort 12 ongoing practical learning.

Project main goal
1. Writting a simple UNIX command interpreter

General information 
1. Unix; trademarked as UNIX) is a family of multitasking, multiuser computer operating systems that derive from the original AT&T Unix, whose development started in 1969 at the Bell Labs research center by Ken Thompson, Dennis Ritchie, and others. (source Wikipedia).
2. Kenneth Lane Thompson (born February 4, 1943) is an American pioneer of computer science. Thompson worked at Bell Labs for most of his career where he designed and implemented the original Unix operating system. He also invented the B programming language, the direct predecessor to the C programming language, and was one of the creators and early developers of the Plan 9 operating system. Since 2006, Thompson has worked at Google, where he co-developed the Go programming language (source Wikipedia)

How does Shell work?
1. A Shell provides you with an interface to the Unix system. It gathers input from you and executes programs based on that input. When a program finishes executing, it displays that program's output.

Shell is an environment in which we can run our commands, programs, and shell scripts. There are different flavors of a shell, just as there are different flavors of operating systems. Each flavor of shell has its own set of recognized commands and functions
2. The prompt, $, which is called the command prompt, is issued by the shell. While the prompt is displayed, you can type a command.

Shell reads your input after you press Enter. It determines the command you want executed by looking at the first word of your input. A word is an unbroken set of characters. Spaces and tabs separate words.
3. In Unix, there are two major types of shells −

Bourne shell − If you are using a Bourne-type shell, the $ character is the default prompt.
C shell − If you are using a C-type shell, the % character is the default prompt.
The Bourne Shell has the following subcategories −

Bourne shell (sh)
Korn shell (ksh)
Bourne Again shell (bash)
POSIX shell (sh)
The different C-type shells follow −

C shell (csh)
TENEX/TOPS C shell (tcsh)

SHELL SCRIPTS
The basic concept of a shell script is a list of commands, which are listed in the order of execution. A good shell script will have comments, preceded by # sign, describing the steps.

There are conditional tests, such as value A is greater than value B, loops allowing us to go through massive amounts of data, files to read and store data, and variables to read and store data, and the script may include functions.

a. Assume we create a test.sh script. Note all the scripts would have the .sh extension. Before you add anything else to your script, you need to alert the system that a shell script is being started. This is done using the shebang construct. For example −

#!/bin/sh
This tells the system that the commands that follow are to be executed by the Bourne shell. It's called a shebang because the # symbol is called a hash, and the ! symbol is called a bang.

To create a script containing these commands, you put the shebang line first and then add the commands −

#!/bin/bash
pwd
ls

SHELL COMMENTS
You can put your comments in your script as follows −

#!/bin/bash

# Author : Zara Ali
# Copyright (c) Tutorialspoint.com
# Script follows here:
pwd
ls

WHAT IS A PID AND PPID
PID stands for Process ID, Which means Identification Number for currently running process in Memory. 2. PPID stands for Parent Process ID, Which means Parent Process is the responsible for creating the current process(Child Process). Through Parent Process, The child process will be created.


How to manipulate the environment of the current process?
A process is an instance of a program currently running in the form of thread(s). Depending on the environment, a process can be uni-threaded (comprising of a single thread) or multithreaded (comprising of multiple threads). A process is an active entity as opposed to a program which is a passive entity.

In Linux, there are various commands which are used for process manipulation. There are commands which enable the user to view the list of processes and their information, commands which allow the user to delay the start of a particular process and commands which terminate or stop a process from further execution. These commands enable the user to manipulate running processes according to his/her needs. All these commands have many options that can be used along with them.

A few commands that are used for process manipulation are:
1. ps - The ps command is used to list all the currently running processes in the system and information related to them. This information consists of the process name, user, memory consumption, CPU consumption, process ID, etc.
2. sleep - The sleep command is used in Linux to delay a running program by a certain amount of time. The amount of time to be delays can be specified in seconds, minutes, hours, and even days. The suffix values for minutes, hours days are m, h, and d respectively. If no suffix value is specified, then, by default, the value is taken in seconds. 
3. jobs - The jobs command in Linux is used to list the status of all the jobs currently running in the terminal along with their job number. This lists only those processes which started running in this session. Job numbers always start from 1 and are always displayed inside
4. bg - The bg command is used to push a suspended process into the background where it can continue to run. The syntax for this command is bg %n where n is the job number of the suspended process the user wants to push to the background

What is the difference between a function and a system call?
A typical processor executes instructions one by one. But there may be occasions where the processor has to stop current instruction and execute some other program or code segment (residing in some other place). After doing this the processor returns to normal execution and continues from where it left off. A system call and a function call are such occasions. A system call is a call to a subroutine built in to the system. A function call is a call to a subroutine within the program itself.

What is a System Call?

System calls provide programs running on the computer an interface to talk with the operating system. When a program needs to ask for a service (for which it does not have permission to do that by itself) from the kernel of the operating system, it uses a system call. User level processes do not have the same permissions as the processes directly interacting with the operating system. For example, to communicate with and external I/O device or to interact with any other processes, a program uses system calls.

What is a Function Call?

A function call is also called a subroutine call. A subroutine (also known as a procedure, function, method or routine) is part of a larger program that is responsible for carrying out a specific task. The larger program may execute a heavy workload, and the subroutine may be performing just a simple task, which is also independent of the remaining program coding. A function is coded in such a way that it may be called multiple times and from different places (even from within other functions). When a function is called, the processor may go to where the code for the function is residing and execute the instructions of the function one by one. After completing the functions, the processor will return to exactly where it left off and continue the execution starting from the next instruction. Functions are a great tool for code reuse. Many modern programming languages support functions. A collection of functions is called a library. Libraries are often used as means of sharing and trading software. In some cases, the whole program could be a sequence of subroutines (e.g. threaded code compilation).

What is the difference between System Call and Function Call?

System call is a call to a subroutine built in to the system, while a function call is a call to a subroutine within the program. Unlike function calls, system calls are used when a program needs to perform some task, which it does not have privilege for. System calls are entry points in to the operating system kernel and are not linked to the program (like function calls). Unlike, system calls, function calls are portable. Time overhead of a system call is more than the overhead for a function call because a transition between the user mode and the kernel mode must take place. System calls are executed in kernel address space, while function calls are executed in user address space.

How to create processes
1. Identify the process
2. Outline the Scope of the Process
3. Identify Process Inputs 
4. Identify Process Outputs 
5. Research Process Needs 
6. Consider the stages in the process
7. Identify the Process Operatives 
8. Order your process
9. Digitize the process
10. Communicate the process
11. Monitor process perfomance 

How does the shell use the PATH to find the programs
Essentially, the shell uses a list of directories in which commands may be found. This list is specified in your PATH variable in your . profile file. The list could be called your search path, because it tells the shell where you want to search.
Command interpreters usually have to search for a file that contains the command you want to run. When you are using the shell, you tell the shell where to search for a command. Essentially, the shell uses a list of directories in which commands may be found. This list is specified in your PATH variable in your .profile file. The list could be called your search path, because it tells the shell where you want to search.

The shell then searches the directories in the following order, when looking for commands or shell scripts:
/bin
/usr/bin
/usr/etc
/usr/macneil/bin
/usr/games
/usr
As soon as the shell finds a file with an appropriate name, it runs that file.

How to execute another program with the execve system call?
1. execve() executes the program pointed to by filename. filename must be either a binary executable, or a script starting with a line of the form "#! interpreter [arg]". In the latter case, the interpreter must be a valid pathname for an executable which is not itself a script, which will be invoked as interpreter [arg] filename.

2. argv is an array of argument strings passed to the new program. envp is an array of strings, conventionally of the form key=value, which are passed as environment to the new program. Both argv and envp must be terminated by a null pointer. The argument vector and environment can be accessed by the called program’s main function, when it is defined as int main(int argc, char *argv[], char *envp[]).

3. execve() does not return on success, and the text, data, bss, and stack of the calling process are overwritten by that of the program loaded. The program invoked inherits the calling process’s PID, and any open file descriptors that are not set to close-on-exec. Signals pending on the calling process are cleared. Any signals set to be caught by the calling process are reset to their default behaviour. The SIGCHLD signal (when set to SIG_IGN) may or may not be reset to SIG_DFL.

How to suspend the execution of a process until one of its children terminates?

The wait() function will suspend execution of the calling thread until status information for one of its terminated child processes is available, or until delivery of a signal whose action is either to execute a signal-catching function or to terminate the process.

A call to wait() blocks the calling process until one of its child processes exits or a signal is received. After child process terminates, parent continues its execution after wait system call instruction. 
Child process may terminate due to any of these: 

It calls exit();
It returns (an int) from main
It receives a signal (from the OS or another process) whose default action is to terminate.

What is EOF / “end-of-file”?
In computing, end-of-file (EOF) is a condition in a computer operating system where no more data can be read from a data source.

GENERAL REQUIREMENTS FOR THE SIMPLE SHELL PROJECT
Allowed editors: vi, vim, emacs
All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
All your files should end with a new line
A README.md file, at the root of the folder of the project is mandatory
Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
Your shell should not have any memory leaks
No more than 5 functions per file
All your header files should be include guarded
Use system calls only when you need to (why?)
Write a README with the description of your project
You should have an AUTHORS file at the root of your repository, listing all individuals having contributed content to the repository. Format, see Docker

List of allowed functions and system calls

_exit (man 2 _exit)
fflush (man 3 fflush)
fork (man 2 fork)
free (man 3 free)
getcwd (man 3 getcwd)
getline (man 3 getline)
getpid (man 2 getpid)
isatty (man 3 isatty)
kill (man 2 kill)
malloc (man 3 malloc)
open (man 2 open)
opendir (man 3 opendir)
perror (man 3 perror)
read (man 2 read)
readdir (man 3 readdir)
signal (man 2 signal)
stat (__xstat) (man 2 stat)
lstat (__lxstat) (man 2 lstat)
fstat (__fxstat) (man 2 fstat)
strtok (man 3 strtok)
wait (man 2 wait)
waitpid (man 2 waitpid)
wait3 (man 2 wait3)
wait4 (man 2 wait4)
write (man 2 write)
access (man 2 access)
chdir (man 2 chdir)
close (man 2 close)
closedir (man 3 closedir)
execve (man 2 execve)
exit (man 3 exit)

Compilation
Your shell will be compiled this way:

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
