Notes for Linux bash crash course

[Link]([Link](https://youtu.be/oxuRxtrO2Ag)


### ls

liststorage

### ~

represents your home folder

### $

indicates you are a standard user ie to don't have adminstrative privileges

### pwd

print present working directory

### Absolute path

### Relative path

 How to get somewhere from where you are now

### ls<pathname>

### options for ls

#### -a
list all files

#### -l
gives a long list with more details like file permissions

### cd
cd with no arguments goes to home directory.
if you hit tab twice after cd <some path> you will get the options for auto completion

### pushd and popd
to go another directory with ab reference to current directory. After working in the new directory you can use popd to come back.

    $ pushd /etc
after working in etc

    $ popd


### file

will give the details of file

### locate

    $ locate fstab

to find files.
locate takes its data from a database. so you have to update it.

    $ sudo updatedb

### which

to find out whether a command is installed or where it is

    $ which cal

### history

last 1000 unique commands


## Getting Help
### whatis
### apropos

    $ apropos time

### man
    $ man man

will give manual for man command

### mkdir

    $ mkdir Junk Junk1 Junk2

### touch

creates a file if it does not exist.
updates date modified if the file exists

    $ touch file1 file2 file3

### cp
     
     $ cp ~/.bashrc bashrc

### mv
to move and rename files
### rm
    
    $ rm *
to remove everything in the folder
    
    $ rm file*
to remove all files with file in them
    
    $ rm -r
to remove directories

### rmdir

Removes directories without files

### cat

shows contents of a file

    $ cat file1

    $ cat  >>  file
now you can enter the contents.

Ctrl+d to exit while done.

cat is short for concatenate. You can cat two files.

### more

to see files page by page
you can use q to exit before end

### less

let you do more stuff, scroll line by line, search for text etc

### nano

text editing

### redirection

    $ cat > file  
to create a file and a add content.    

    $ cat >> file  
to append to a file  
### piping  
taking output from one programme and putting into another 

    $ history | less

### Redirection

    $ ls -al / > lsout.txt
### sudo


to retain super user privileges for some time

sudo -s  
$  will change to #
exit to exit

### su
su - user
su user
su
don't do this in Ubuntu due to security issues

### users
gives uses logged in
### id
### File Permissions
Read write and execute permissions

    $ chmod +x filename

chmod stands for change mode

there is one number system for changing file permissions. Dig that deeper for understanding it.

## Killing Processes
Ctrl c kills a command

### killall
    $ killall firefox

### to exit bash
exit
Ctrl d

## For clearing screen
Ctrl l
may be this will work only an emulator

## to make text bigger
Ctrl +  
to make smaller  
Ctrl -









