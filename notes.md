# /dev/null is a so-called special device. It's a part of the linux OS, and it's a discard device. Everything you send to this /dev/null will be discarded. that can be usefull because now my output is pretty clean.

# man -k user which is searching the man pages on linux for the keyword user.

# man -k user | grep 8 which means that grep 8 is filtering out all the lines that contains an 8 and then, it becomes a little bit more readable.

# help this will get the list of internal commands

# bash will start new bash instance (sup shell). every single command that you are going to run is starting a sup shell by itself.

# if you really want to make sure that you variables are available in all the different shells, include them in the Bash start-up files

# As a best practice, I would recommend not to use alias in shell scripts because alias settings are not universal and might not exist on other computers where the shell script is used. if you are going to use alias in shell script, make sure you definde the alias in the shell scripts themselves.

# A subshell is opened when commands are executed, because every command that is executed on linux starts its own subshell. and in it's own subshell, the command is working with its own environment.

# .bash_logout which can be used to clean up things when users are logging out. this is a file that is often forgotten, by the way. but if you want to make sure that some housekeeping is done when users are logging out, then this is where you need to look.

# If you aim is to optimize and ultimate, using a linux shell, learn bash.

# cut -d : -f 3 cat /etc/passwd
# cut -d : -f 3 cat /etc/passwd | sort
# cut -d : -f 3 cat /etc/passwd | sort -n