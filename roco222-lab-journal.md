Lab session 1
Software engineering for roboticists
Step 1 - Write your first Markdown document

The text below is our first attempt at using the markdown syntax.
ROCO222
Introduction to Sensors and Actuators

This is an example of bold text

This is an example of italics

Strikethrough

    Item 1
    Item 2 ..* Sublist of item 2
    Item 3

Step 2 - Command-line 101

opened the terminal amd tried a few commands

$ ls

This command gives us a list of directories.

cd /tmp

This command changes directories, in this case to tmp.

cd $HOME

cd is used to change a directory.In this case, the home directory. The dollar sign means a normal user as opposed to a 'root' user.

mkdir

mkdir is for making new directories.

echo "hello" > hello.md

echo is a built in command that writes its arguments to standard form. This writes "Hello" in a markdown document named hello.md

cat hello.md

cat is short for concatenate. cat allows use to create single or multiple diles , view contents of a file, concatenate files and redirect the output in terminal or files. Using this command, the terminal ouput "Hello", thereby showing what we wrote in the markdown document.

cp hello.md hello-again.md

This copies the contents of hello.md into a new markdown named hello-again.md

mv hello-again.md hello-hello.md

This renames "hello-again.md" to "hello-hello.md"

rm hello.md

This has deleted the hello.md directory.

rm -rf the rm -rf is the same as rm -r -f the -r meaning "remove directories and their contents recursively" the -f will "ignore nonexistent files and arguments, never prompt"

cat /proc/cpuinfo

This command lists characteristics of the computer's cpu, incluidng number of cores.

Step 6
For this module, we have used github to create a lab journal using the markdown syntax. We have learned the basics on git repositories, including the master branch and practised making additional branches. The text in these branches can be merged with the master branch. We have also begun to commit changes to a repository, adding a description on the updates made.
