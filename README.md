## Simple shell Colaboration projects

## Description

Simple Shell project is a joint project between Taiwo Abiodun and Abiodun Ogunremi.

This Simple_shell program can be compiled and launched from the command line, where its main function is to execute commands read from the standard input.

## Files
Description of the files used:

| Files | Description             |
| --------- | ------------------- |
| _calloc.c  | Function that allocates memory |
| _cd.c    | Function that changes to the directory of the process |
| _ex.c    | Function that finds if input is esit, therefore terminates process |
| _fork.c | Function that creates process and executes |
| _getline.c | Function that reads what the user writes |
| _signal.c | Function that handles the SIGINT signal |
| _writerr.c | Function that gets each error |
| checkbin.c | Function that checks if commands exits in the PATH |
| gridfree.c | Function that free an array of arrays |
| parser.c | Function that creates an array of pointers depending on the delimit characters used |
| sshell.c | Main function that starts the shell |
| shell. h | Header file with all the functions prototypes |

## Shell Compilation
	$ gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
## Shell execute
	./hsh

## Commands on shell
	cd - Change directory
	env - List the current enviroment variables
	exit - exit the shell
	pwd - Print the absolute pathname

## Examples

Below are some of the examples of this shell project working process:

cd:

	^_^ pwd
	/home/vagrant/simple_shell
	^_^ cd
	^_^ pwd
	/home/vagrant
	^_^

cd error:

	^_^ cd hola
	./hsh: 1: cd: can't cd to hola
	^_^

exit:

	^_^ exit 123
	vagrant@vagrant-ubuntu-trusty-64:~/simple_shell$ echo $?
	123

exit error:

	^_^cisfun$ exit hola
	./hsh: 2: exit: Illegal number: hola
	^_^

## Authors
- `Taiwo Abiodun` taiwobiodun@gmail.com
- `Abiodun Ogunremi` @gmail.com
