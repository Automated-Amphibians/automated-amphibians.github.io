---
layout: content
---

### Filesystems

Computers need ways to store and organize your data. Most [Operating Systems](#test) systems use a filesystem, 
including those on phones, controllers like the roboRIO, and computers. While the technical details of the 
filesystems often differ, the essentials remain the same: data is stored in files and folders.

Typically you can think of data as being organized at three levels:

* Drive or Mount 
    * Folder
        * File
            * Metadata and other Attributes
            
Files are the most basic unit of storage an operating system has. Files can be just about anything. It is often easy 
to tell what type a is from the "extension" appended to the end of the filename. 

Some examples of file types include: 

* `Text Files`
    * Source Code (.java, .py, .c, .cpp, .h, .js)
    * Text Data Files (.json, .xml, .yml, .html, .rtf)
    * Configuration Files (.ini)
* `Binary Files`
    * Multimedia such as movies, photos, music (.jpg, .gif, .png, .mov, .mp4)
    * Documents (.doc, .docx, .rtf, .xls, .ppt)
    * Executables (.exe, .sh)
    * System Libraries (.jar, .dll, .so)
    * Archive Files (.zip, .tar.gz, .rar)
    * Binary Data Files ()
* `Other`
    * Special System Files

Most operating systems make it easy to find files on your system by providing a file browser. On windows, the default file browser is called
explorer. On a macintosh, it is called Finder. Linux has many, many options for file browsers. On Ubuntu, it is called Nautilus.

On windows, the file browser has the option to hide or disable showing the extension of a filename, because it is "simpler". [You should disable
this feature](https://www.google.com/search?q=show+file+extensions+in+windows). While it does cut down on clutter, it still hampers our 
ability to see what type a file is.

In the above list of file types, we categorized files into three "super-types" of files. This has to do with how the data is stored within 
the file itself. The important distinction between text, binary and system file pertains to what we as the end user can do with them and
how different programs treat text files vs. binary files.

#### Text Files
Text files can be viewed and modified by ANY text editor (Notepad, TextEdit) or a typical programming tool (Microsoft Code). There are many
[text editor programs](https://en.wikipedia.org/wiki/List_of_text_editors), and they all come with different capabilities. 

Some text files have a structure that has to be respected to keep them valid. Good examples of these are text data files like HTML and JSON files.

Some text files are meant to be used with specific programs. HTML files are meant to be used with a browser.  

Text files also can have different [line endings](#line-endings). Line endings are a special "character" or that tells the operating 
system to advance to the next line for the following text. Your text editor (or SCM such as GIT) will try to maintain the correct 
line-endings for each file type, but sometimes this is a trucky file.

Text files are the good guys of the operating system world. They are easily modified by any program designed to work with text files.
TODO: Talk about piping, such as in linux systems

#### Binary Files
Binary files store their data in such a way, that they

Technically speaking, almost all files are binary, including text files. TODO: Talk about encoding

#### Other or Special System Files
We'll get this "super-type" out of the way first because it's the most unusual, and while it is good to know about, 
you won't typically have to deal with it. 

TODO: Talk about symbolic link files, files that point to hardware, and /dev/null

### Folders (and Paths)
TODO

### Drives
Drives can be typically thought of as physical pieces of hardware. There are MANY types of drives:

* USB Flash Drives
* Hard Drive or Solid State Disk
* Flash Card
* Floppy Drive

Drives can also be 

TODO


#### References
* https://www.computerhope.com/jargon/f/file.htm

#### Glossary
* `Operating System`{: id="operating-system"} - [Wikipedia](https://simple.wikipedia.org/wiki/Operating_system)
* `line-endings`{: id="line-endings} - More info to follow later
* `character-encoding`{: id="character-encoding"} - More info to follow later