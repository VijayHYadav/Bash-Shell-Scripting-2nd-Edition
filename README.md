## Note on #!/bin/bash or #!/usr/bin/env bash
Some people like use bin/env,but really, it's not a big difference.The difference is a littlebit of background about thefile system handling standard,in the old days of the fhs,the default location forbash was in /bin/bash,now /bin is not anordinary directory anymore.And everything that previouslywas in /bin should nowbe in /usr/bin.And that includes bash, sothere's a theoretical chance,if you are using /bin/bash,that at some point in time,your script doesn't work anymore.So now the nice way ofreferring to your scriptis by using a usr, bin,env, for environment bash,what is that doing?That is taking bash from your environmentand it'll find thevariable that points you tothe correct bash shell.And that means that nomatter where your bash shellis installed, it will always work.So if you really want to do itthe nice way usr, bin , env,
is probably the best way of doing it.


## About the Script Location
Then there is a script location,because of Linux pathvariable restrictions,scripts can not be 
executedfrom the current directory.That's a security fee here.The thing is that anintruder might
benefitfrom the fact that in some directory,the intruder has right access.And then if by accident,
you run a command that is, ina reality, an evil command,that destroys your system,but it has the
same nameas a common utility.Well, there's a risk andfor that reason in Linux,by default scripts
cannot be executedfrom the current directorywithout doing anything specific.So you should consider
usingscripts to a bin directoryto store scripts for personal use.If you do that, make surethat
you modify your path.On Red Hat and Favily,homedirectory/bin is in the path,on Ubuntu that's not the case.
You can also consider usingit to usr, local, bin,for scripture to beavailable for all users.But of course, 
in order to puta script and use a local bin,you need to sudo privileges.
