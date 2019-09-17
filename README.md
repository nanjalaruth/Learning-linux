# Learning-linux

## why unix?
it is suited to working with text files and has several powerful commands

## Basic commands in linux

### ls command
used to list the contents of any directory.
**ls ../..** can be used to list the directories above you
**ls -l** gives a longer output compared to ls alone
Others include : ls -R
                 ls -l -t -r
                 ls -lh

### pwd command
used to find out where you are

first slash - root directory
the remaining forward slash - delimits the various part of the hierarchy directory.

### mkdir command
used to make a new working directory
for instance : learner@:~$ mkdir learning_unix
#### making subdirectories
the dollar sign ($) is used
for instance : learner@:~$ mkdir learning_unix $ outer
_ _you can then change the working directory to **outer** and then view it

2 subdirectories could be made using an single command, that is
_ _**mkdir -p outer/inner**

### cd command
used to change the working directory
for instance you could change the directory to the root directory and then to the home directory ; _ _**cd /home/learner/**_ _

**Navigating upwards in the unix file system

(..) depicts the parent directory, in case one wanted to move 2 levels upwards, the command would be : **cd ../..**

**Absolute and relative paths

incase you are working in the /home/learner/learning_unix directory and you then want to change to the /tmp directory, 
the command would be : **_ _learner@:learning_unix$ cd ../../../tmp/_ _** or **cd /tmp** if you are sure of the path.

**Finding your way back home

**cd ~** or **cd** takes you back to the home directory

### man pages
it gives a manual of how to navigate through the different commands
**space** is used to scroll down a page, **b** to go back a page, or **q** to quit

### removing directories
the **rmdir command** is used.
**N/B** you have to be outside a directory before you can remove it
