# Welcome to Foundations of Computing for Biologists

pounds for headings (1) and subheadings (2)

file format use most often in class = plain text file
	- word saves metadata, formatting etc --> hard to use for coding
	- plain text files are simpler (ex: csv)
sublime lets you use plain text files-download!
	-will colorcode markdown files for you
.rtf not same as plain text
*always double check that it's plain text file before saving/using
Using Terminal a lot this semester
	-download gitbash

~ = home directory
[username@mike ~]$ = **command prompt**
username computer logged into directory

working directory=whatever window currently working on - need to be aware of where we are

on terminal write ctrl +c to make new line 
cys-help@loni.org helps with login stuff

clear = clear whole screen 
logout = log out of terminal 

- Introductions

- Syllabus Overview and Questions
	
- Survey

- Overview of Operating Systems
  aka OS
  - Windows = propriotory
    	-bc no unix have to use GitBASH
  - Mac = propriotory
   	-based on unix (older operating syst that its based on)
  - Linux = crowd sourced (anyone can modify source code, unlike other 2)
   	-"flavors" = different versions (ex: RedHat)
    -based on unix

	differences dont matter thru the mike terminal website

- Some fundamentals
  - Memory (RAM)
    - amount space computer has to for you to work on what youre doing now (short term; "desk")
    - fluid, changes a lot depending on what working on 
  - File storage (hard drives)
    	-all older files
    	-more storage, but takes longer to find
    	-different types (solid state=more expensive, less moving pieces)
  - CPU
    -thing thats doing the work on the computer
    - = central processing unit
    - fast
    - indiv CPUs hitting plateau with speed => computers now have multiple CPUs 
  - GPU
    - = graphics processing unit
    - started with graphics, now used for AI
    - 1000s tiny processors, allows for a lot of computing in a short amnt of time
    - parallel computing-lots of computing happening at once [vs serial computing-one after the other]

- Unix Filesystem
	- [Filesystem overview](https://github.com/FoundCompBio-Spr26/Intro_Week1/blob/main/Filesystems.md)
 	- The Unix root (/)
   		- The very base of the filesystem
       	- single folder that holds everything (bottom container)
       	- JUST a slash
  path=route to files
	- Absolute paths
		- All absolute paths begin at the root- **start with /**
    	- full address ex. 123 main st
	- Relative paths
		- Don't start with /
		- Working directories
		- Shortcuts for current and parent directories
    	- relative to where are rn, this is path you take, only works if starting in that spot
       	-shorter, but depends on starting in particular location
	- Hidden files and folders
		- Names begin with `.`
		- Usually used for configuration files

- [Practical Computing Tips](https://github.com/FoundCompBio-Spr26/Intro_Week1/blob/main/ComputingTips.md)

```
Assignment 1


pwd = print working directory
	- use to redirect self to where are
	- shows paths

cd = change directories
	type cd [space] where we want it to go
			(extra info after command=argument) always specific to command
	if type first letter then click tab to get it to fill in full file name
	double tap tab to show all folders with that name
	can be as specific as want
		-if know full path type full path folder/folder/folder
		- can type /folder/folder to make sure it always works (absolute)

cntrl c cancels out

3 ways to get to home directory
	cd
	cd + path
	cs + ~

ls = list
	shows what is in
	can also use ls ./folder
	ls -a
		-a = flag (optional settings)
		-a shows "hidden files/folders" [they all start with a period]
			.bashprofile = text file, helps modify command line etc (ex: customize how command prompt looks)
			.bash_history = stores all of your history
		ls -l = long list; gives list but with more info
			human readable units = ls -lh (lets you check permissions) 
		can put the flags together
		on the left hand side = 10 unit codes, start=tells you what kind of file;
			the next 9 give different permissions read (r), write(w), run the code(x) repeated x3; 1st set=creator, 2nd set=anyone in users group, 3rd=anyone on particular user system
		
commands have a lot of options, man = manual pages, so do man [command] to help give you the flag options
	case sensitive, maybe 2 dashes when longer commands 



records all previous commands - use up and down arrows

NEVER use spaces in names of files/folders
	-camel case = capitalize first letter in file name
	-underscores

to create empty text file = touch FileName.txt or FileName.md if know it will eventually be a markdown file
	-doesnt pull something up right away, can check using ls
	-only in HPC; can see on hpc website (ondemand.mike one)
	-should include file extension to be helpful

folders = directories

mkdir = make directory
	mkdir name

cd .. = takes to previous (parent) directory you were in; "move down in file system"- move backwards along path towards root; 1 down
	- can string together ../../../.. can do as many as want bc will stop at root
	-relative path

. = shortcut to where am right now; look where I am right now in particular 

(1) Sign up for an account on GitHub and send your username to me.
(2) Apply for an LSU HPC account:
    https://accounts.hpc.lsu.edu/login_request.php
    When you do, list me as your sponsor. 
    Once your account is created, send me your username.
```
