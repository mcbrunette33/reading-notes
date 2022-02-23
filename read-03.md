## Read 02 ##
**Git** is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

- Loss of Data- Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

- Git Installation- Git can be installed in three ways:

- Install as a package
- Install via another installer
- Download and compile the source code
- check settings- To check settings, use the git config --list command

*git help command - git help / git command --help*

*Cloning*-You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

**Repository Structure: The local Git repository has three components:**

1. Working Directory: The actual files reside here.
2. Index: The area used for staging
3. Head: Points to the most recent commit