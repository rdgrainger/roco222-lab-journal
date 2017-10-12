# Lab session 1
## Software engineering for roboticists

### Step 1 - Write your first Markdown document

The text below is our first attempt at using the markdown syntax.
ROCO222
Introduction to Sensors and Actuators

**This is an example of bold text**

*This is an example of italics*

~~Strikethrough~~

  1. Item 1
  2. Item 2 
  ..* Sublist of item 2
  3. Item 3

### Step 2 - Command-line 101

opened the terminal amd tried a few commands

**$ ls**

This command gives us a list of directories.

**cd /tmp**

This command changes directories, in this case to tmp.

**cd $HOME**

cd is used to change a directory.In this case, the home directory. The dollar sign means a normal user as opposed to a 'root' user.

**mkdir**

mkdir is for making new directories.

**echo "hello" > hello.md**

echo is a built in command that writes its arguments to standard form. This writes "Hello" in a markdown document named hello.md

**cat hello.md**

cat is short for concatenate. cat allows use to create single or multiple diles , view contents of a file, concatenate files and redirect the output in terminal or files. Using this command, the terminal ouput "Hello", thereby showing what we wrote in the markdown document.

**cp hello.md hello-again.md**

This copies the contents of hello.md into a new markdown named hello-again.md

**mv hello-again.md hello-hello.md**

This renames "hello-again.md" to "hello-hello.md"

**rm hello.md**

This has deleted the hello.md directory.

**rm -rf the rm -rf**

is the same as rm -r -f the -r meaning "remove directories and their contents recursively" the -f will "ignore nonexistent files and arguments, never prompt"

**cat /proc/cpuinfo**

This command lists characteristics of the computer's cpu, incluidng number of cores.

### Step 6
For this module, we have used github to create a lab journal using the markdown syntax. We have learned the basics on git repositories, including the master branch and practised making additional branches. The text in these branches can be merged with the master branch. We have also begun to commit changes to a repository, adding a description on the updates made.

## Hacking into a robot.

The task asked us to interface with a robot using the Linux terminal and some python code. The first step was to connect to the robot itself (named chapman). I used 

*ping chapman.local*
and then
*ssh nao@192.168.0.184*
I entered the required password and was now connected to the robot. The next step was to find a way to send it a message.

I created a python file (named hack4.py) in the terminal and copied the code given:

*from naoqi import ALProxy
tts = ALProxy("ALTextToSpeech", "localhost", 9559)
tts.say("I've hacked you, robot!")*

Then I ran the executable hack4.py with:

*nano hack4py*

# Lab session 2
## Build a DC Motor

We have been tasked with building a DC motor, testing it and then creating a better iteration. The initial design included one coil of wire with 118 turns, copper tape as a commutator, a cork to function as a core and a suppport structure.

### The original motor:




One of the issues we had with this motor was the small size, only allowing for one coil. It was also difficult to wind around. The commutator was fragile and crumpled too much to use effectively.

### Improving the design

There were a few ways to improve on this:

1. Add more coils of wire
2. Change the material of the core
3. Create a more stable commutator
4. Create a sturdier base to hold the new design
5. Use a larger core so more coils can be wound


We decided to use 8 coils of wire, each with 100 turns. The commutator has 16 segments to accomodate this. The wire is coiled around an airbed pump.


Calculations:

