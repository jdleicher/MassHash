MassHash 1.0.1
==============
A set of file hashing tools

[http://jdleicher.github.io/MassHash/](http://jdleicher.github.io/MassHash/)

Programs Included  
------------------------
MassHash 1.0.1 - A set of file hashing tools (command-line)  
MassHash Launcher 1.0.1 - A GTK+ launcher for MassHash

Features
--------
 * Supported algorithms include: MD5, SHA-1, SHA-224, SHA-256, SHA-384, SHA-512
 * Generate a hash for a single file
 * Generate a list (plain text file) of hashes for all files in a directory (and subdirectories)
 * Compare a previously generated list of hashes against the same directory (or mirror)

Dependencies
------------
Note: Other versions may work, but have not been tested.  

 * Python 2.7.6 or 3.4.0
 * GTK+ 3.10.8 (MassHash Launcher)
 * PyGObject 3.12.0 (MassHash Launcher)

Installation
------------
Installation to a specific path is not required.  Versions for both programs are available for both Python 2 and Python 3.  These files are located in the corresponding python2 and python3 directories.  Permissions may need to be altered for these files so they are executable (e.g. chmod u+x masshash).

Python Interpreter Path:  
If either of the programs won't start correctly, it may be that the path and name of the Python interpreter (or symlink to the interpreter) on the system differs from the one specified in the "shebang line" of each file.  To resolve this, alter the line in both files to the correct path and name.

Notes:  
MassHash Launcher, by default, uses set paths to look for the masshash file in the same directory and the masshash-launcher.glade file in the data directory.  For viewing or alteration of these paths, refer to the "same_dir" and "glade_source_dir" variables within the masshash-launcher file.  Also, the masshash-launcher.svg file should always be in the same directory as the masshash-launcher.glade file.

Usage
-----
MassHash is a command-line program which contains 3 subcommands: single, list, and compare.  For usage and version information, change the current working directory to the one containing the masshash file and checkout the following commands:

    ./masshash --version
    ./masshash single --help
    ./masshash list --help
    ./masshash compare --help

For an alternative to using the command-line, use MassHash Launcher.  It's a graphical program which can be used to launch a MassHash command as a subprocess (the masshash file must be present).
