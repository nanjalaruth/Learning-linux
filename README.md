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

**Navigating upwards in the unix file system**
(..) depicts the parent directory, in case one wanted to move 2 levels upwards, the command would be : **cd ../..**

**Absolute and relative paths**
incase you are working in the /home/learner/learning_unix directory and you then want to change to the /tmp directory, 
the command would be : **_ _learner@:learning_unix$ cd ../../../tmp/_ _** or **cd /tmp** if you are sure of the path.

**Finding your way back home**
**cd ~** or **cd** takes you back to the home directory

### man pages
it gives a manual of how to navigate through the different commands
**space** is used to scroll down a page, **b** to go back a page, or **q** to quit

### removing directories
the **rmdir command** is used.
**N/B** you have to be outside a directory before you can remove it

### tab completion
It is used to complete the names of files and programs on most Unix systems without having to type everything
**up and down arrows** can be used to access any command from your history

### touch command
it is used to create a new empty files
for instance; _ _learner@:learning_unix$ touch heaven.txt_ _ which outputs _ _heaven.txt_ _

### mv command
it is used for moving files to another directory
for instance; "heaven. txt" can be moved to a directory named "temp"
**_ _learner@:learning_unix$ mkdir temp
learner@:learning_unix$ mv heaven.txt temp/
ls temp
heaven.txt_ _**

#### wildcards
asterisk '*' could also be used to move files in one go, it acts as a wild card character which essentially means 'match anything'
for example; **mv *.txt temp/** would mean move anything that has a '.txt' to the directory 'temp'

the character '?' will match exactly one character. so ls ?ouse will match files like house and mouse but not grouse

### renaming files
in order to rename files, the _mv command_ is used 
for example, we could create a new file called _mudibo_ move it to a directory **_rut_** and in the process rename it to _mudib'
**_eanbit6@Bioinfo5_Data$ touch mudibo 
eanbit6@Bioinfo5_Data$ mv mudibo rut/mudi                             
eanbit6@Bioinfo5_Data$ ls rut_**

### moving directories
uses the _mv_ command to move between different directories, that is, moving one directory to another

### removing files
the _rm_ command is still used but with an _-i_ which gives a confirmation message of whether you still want to delete the file
the command would be _rm -i_
**_N/B a directory cannot be removed if it still has files inside_**

### copying files
uses the _cp command_ to make a copy of a file
a file can be copied from one directory to another
**_eanbit6@Bioinfo5_Data$ touch ~/file2                                  
eanbit6@Bioinfo5_Data$ cp ~/file2 .                                   
eanbit6@Bioinfo5_Data@ ls_**

directories can also be copied recursively to another directory using the **_cp -r_** command

### Viewing files with less
the **_less command_** is used
the _echo_ command is used to put texts into files, the text can be redirected into an output file usingg the **>** command
**example**
eanbit6@Bioinfo5_Data$ echo "my name is Nanjala.">rth                 
eanbit6@Bioinfo5_Data$ less rth  
 when using less; _space_ - is used to scroll upwards a page
                  _h_ for help
                  _j or k_ to go forward 
                  _q_ to quit    
                  
### viewing files with cat
