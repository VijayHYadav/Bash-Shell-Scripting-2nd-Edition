# Variables
I type bash, I use echo $color,
and we can see in a subshell
it is available as well.
Now, a subshell is a shell
that is defined as a child
of the current shell.
It wouldn't be available in a Perl shell.
Let me open another tab,
and let's use echo $co,
and you can see Tab
completes doesn't work.
And even if I type it completely,
the variable just doesn't exist.
Export is for subshells
and subshells only.
If you want it to be
available in all shells,
you should put it in some
starter files like .bashrc
which is probably the
most appropriate location.
In your Home directory,
that will make sure that
at least for your account,

# images/Screenshot from 2022-09-05 06-47-44.png
So, which direction do you want to go to?
I would advice for demonstration purposes.
Use the directory that
doesn't contain too much false
or directory, so I'm going to slash home.
Now, the interesting thing is that we see
is really isn't slash home.
And it is sprinting the contents
of slash home directory,
which contains directory
with the name student.
And then, I'm getting back
to the original position
where I was.
Now, what is this problem?
Oh, this thing is that
if you start a script,
the script starts subshell.
And everything that's
happening in that subshell,
well, it's happening in that subshell.
And at the end of the script,
you're getting out of the subshell.
And that's something
to be really aware of.
We'll talk about it
further in the next video.
