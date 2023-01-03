---
layout: content
---

This video provides a good base:
[GIT in 15 minutes](https://www.youtube.com/watch?v=USjZcfj8yxE&t=326s)

[Quiz questions help to reinforce the material.](git-quiz)


### Learning
##### What is version control or Source Control Management (SCM)? 
Lets take a very practical example. You're writing robot code in a project. You change 5 java files of the 300 java files in the project.
You want to share it with other team members. But you don't want to mess up what they are already working on because they have their
own changes to the project. `Source Control Management` or `SCM` is exactly what you are looking for. 

In this example, you want to `PUSH` your code somewhere else. Your teammates want to `PULL` your code onto their computer.

##### Starting GIT
GIT is an application that does Source Control Management. It is a very popular tool, for many good reasons.

It is important to understand that `git` is to github as your iphone is to the icloud.

You use `git` locally to push your code and store it on github. Unlike the iphone, you can use `git` with multiple clouds or server environments.
You can even push from one computer to another if you understand how to set it up. 
[//: ] This is called distributed version control.

We will stick to simple examples.

If you've installed git correctly, you should be able to goto a command line, type in "git" and get something along the following lines:

```
cgp@computer:~/git/frc$ git
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
        [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
        [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
        [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
        [--super-prefix=<path>] [--config-env=<name>=<envvar>]
        <command> [<args>]        
```


GIT manages collections of files and folders called a `repository`.  When you `clone` something, you are copying a repository to your
local hard drive. 

Lets start by cloning a sandbox we can play in:

    git clone git@github.com:Automated-Amphibians/git-sandbox.git

You can find the SSH version under the code button:

![](git-assets/git-copy-url.png)

You should see something like:

```
cgp@computer:~/tmp$ git clone git@github.com:Automated-Amphibians/git-sandbox.git
Cloning into 'git-sandbox'...
remote: Enumerating objects: 19, done.
remote: Counting objects: 100% (19/19), done.
remote: Compressing objects: 100% (14/14), done.
remote: Total 19 (delta 2), reused 7 (delta 0), pack-reused 0
Receiving objects: 100% (19/19), done.
Resolving deltas: 100% (2/2), done.
```

Change your `working directory` to the sandbox.

    cd git-sandbox

##### Starting to working with a GIT repository
A git repository is nothing more than a single folder that happens to have your files alongside a .git folder which is used to
manage the GIT related data. 

Often the first thing we do when we enter a git repository folder is check the status. Sensibly, the command is:

    git status

You should see something like:

```
cgp@computer:~/git/frc/git-sandbox$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

If you see something like:

```
fatal: not a git repository (or any of the parent directories): .git
```

then you aren't in a git repository folder. You will need to try the clone again, or ask someone for help.

If you want to see how GIT stores your SCM data in files, you can always explore the .git folder under the repository directory.

It should look something like this:
```
cgp@computer:~/git/frc/git-sandbox$ ls -las
total 20
4 drwxr-xr-x  4 family family 4096 Jan  2 10:54 .
4 drwxr-xr-x 17 family family 4096 Jan  2 10:52 ..
4 drwxr-xr-x  8 family family 4096 Jan  2 17:39 .git        <<-- your git data
4 drwxr-xr-x  3 family family 4096 Jan  2 10:54 java
4 -rw-r--r--  1 family family  224 Jan  2 10:52 README.md
```

If you do a file listing in the .git directory, you'll see lots of interesting files. I encourage you to explore these on your own time, 
as curiousity is a great way to learn new features.
```
cgp@computer:~/git/frc/git-sandbox/.git$ ls -las
total 60
4 drwxr-xr-x  8 family family 4096 Jan  2 17:39 .
4 drwxr-xr-x  4 family family 4096 Jan  2 10:54 ..
4 drwxr-xr-x  2 family family 4096 Jan  2 10:52 branches
4 -rw-r--r--  1 family family   14 Jan  2 17:39 COMMIT_EDITMSG
4 -rw-r--r--  1 family family    8 Jan  2 17:39 COMMIT_EDITMSG.bak
4 -rw-r--r--  1 family family  272 Jan  2 10:52 config
4 -rw-r--r--  1 family family   73 Jan  2 10:52 description
4 -rw-r--r--  1 family family   21 Jan  2 10:52 HEAD
4 drwxr-xr-x  2 family family 4096 Jan  2 10:52 hooks
4 -rw-r--r--  1 family family  370 Jan  2 17:39 index
4 drwxr-xr-x  2 family family 4096 Jan  2 10:52 info
4 drwxr-xr-x  3 family family 4096 Jan  2 10:52 logs
4 drwxr-xr-x 18 family family 4096 Jan  2 17:39 objects
4 -rw-r--r--  1 family family  112 Jan  2 10:52 packed-refs
4 drwxr-xr-x  5 family family 4096 Jan  2 10:52 refs
```

#### Branching
Now we want to make our changes. But we don't want to make changes that will bump up against someone else. So we take our code,
and we branch it. In other SCMs, the main branch is called trunk. In GIT it happens to be called main. So we create a branch
from main using the following command:

    git branch <YOUR_BRANCH_HERE>

The name of the branch is up to you, but there are usually strategies to naming a branch. There is a method called feature branching
where the name of the branch matches the type of feature being implemented. If you were implementing a drivetrain, you'd call it drivetrain.
Another strategy might be to simply use your own name. Sometimes a combination of strategies might be needed. Maybe you are working on multiple features,
so you have multiple branches, so you might name one branch *bob-drivetrain*, and another *bob-arcade-driving*. Remember! Branch names
cannot have spaces in them!

*What if I make a mistake?*

Delete the branch with:

    git branch -d <YOUR_BRANCH_HERE>

#### Checkout and start working
We're ready to start working right? Not quite, we need to be "on the branch" to safely edit without bumping into anyone else. This is easy.

    git checkout <YOUR_BRANCH_HERE>

We should always verify that we're on the branch 


* git branch
* git merge
* git push
* git pull
* git add
* git log        
* git checkout 
* git status



### Other References
####  References
* [GIT cheatsheet](https://www.jrebel.com/blog/git-cheat-sheet)
* [Another GIT cheatsheet](https://ihatetomatoes.net/git-cheat-sheet/)
* [GIT Handbook](https://git-scm.com/book/en/v2) - This is all the gory details. GIT is a beautifully designed system put together by none other than
the benevolent dictator of Linux, [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds). It is simple but powerful.

#### More Tutorials
* [https://frc3512.github.io/ci/intro-to-git/](https://frc3512.github.io/ci/intro-to-git/)
* [https://learngitbranching.js.org/](https://learngitbranching.js.org/)
* [What is version control](https://www.perforce.com/blog/vcs/what-source-control#:~:text=These%20two%20terms%20are%20used,binary%20files%20and%20digital%20assets.)
* [Learn git concepts, not commands](https://github.com/UnseenWizzard/git_training)
* [GIT Immersion](https://gitimmersion.com/index.html)
* [Links to other git tutorials](https://github.com/git/git-scm.com/issues/1239)

### Notes for later
* Why use the command line version of git?
    * It works everywhere.
    * It has all the commands
