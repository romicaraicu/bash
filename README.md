## Tips & tricks for bash 
------
### Bash Built-in variables:
I found the $#, $@ & $? bash built-in variables very useful since I knew linux and today I would like to share their usage

* $# = number of arguments. Answer is 3
* $@ = what parameters were passed. Answer is 1 2 3
* $? = was last command successful. Answer is 0 which means ‘yes’
#### Example
```bash
file:test.sh
#! /bin/sh
echo '$#' $#
echo '$@' $@
echo '$?' $?

*If you run the above script as*

> ./test.sh 1 2 3

You get output:
$#  3
$@  1 2 3
$?  0

*You passed 3 parameters to your script.*
```
------
### Repeating an argument
```bash
[root@srv ~]$ mkdir /path/to/exampledir
[root@srv ~]$ cd !$
```
------
