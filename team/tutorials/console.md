---
layout: content
---

TODO 

Describes how to use the console. 

See [curriculum](/frc-survival-guide/aa-handbook/curriculum/coding-curriculum).

### What and where is my profile folder?
{: name="profiles"}
A profile folder is the directory where all of your user specific information is kept. It is often
configuration information for different applications, but it can be custom commands, or just stuff
you've downloaded. Typically your desktop icons, documents are stored underneath your profile 
directory.

#### Linux/MacOSx
Gettin to your profile folder in Linux is as simple as going to 

Also the $HOME environment variable holds the path of the current user.

#### Windows
When you start `cmd`, you are in your profile directory.

THe %HOMEPATH% environment variable contains the path of the current user.

### Reading the manual for a command line program
{: name="reading-the-manual"}

In order to understand how a command line program works, you want to read the manual. There are a number of ways to do this. First is to
get the basic usage by querying the command with no arguments.

    git

For git, it just returns the available flags that can be used. GIT is the epitome of properly written software, so it makes it very
obvious how to get more help. 

    git --help

For other program -? is common. On windows it is /? for most commands.

However, for more detailed information, you can also do:

    man git

This provides a real manual about how the command works from top to bottom. Sometimes a man page won't be found. At this point it's
up to the internet and looking there for additional help.
