# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > REPLACE THIS TEXT WITH YOUR RESPONSE

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > ls -- lists the files and directories.
> > ls -a -- lists all files and directories including hidden files, usually stating with "."
> > ls -l -- lists all files and directories in long list format to show specific details.
> > ls -lh -- lists files and directories with sizes in human readable format.
> > ls -lah -- lists all files and directories including hidden files with sizes in human readable format.
> > ls -t -- lists all files and directories sorted based on the file's modification time and date (newest first).
> > ls -Glp -- lists long format directories with "/" appended to the end of directories (shown in different color).

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > ls -a
> > ls -d
> > ls -m
> > ls -p
> > ls -1

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs allows unix to execute certain commands from standard input. For example, "echo"
> > echo 'my_dir1 my_dir2 my_dir3' | xargs mkdir
> > the above command will make 3 new directories named my_dir1, my_dir2 and my_dir3.

 

