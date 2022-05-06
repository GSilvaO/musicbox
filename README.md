# Project Description
 The goal of this set of "mini-programs" is to consolidate concepts such as Serialization, File I/O, Network and Threads in Java. The final program is a simple Software Synthesizer with a chat that enable users to load and play tracks from other users. I'm using <strong>JavaSound API</strong> to implement the synthesizer as well as the mini-programs.


## Project Organization
 This project is organized in such a way that each branch represents a little development step. In the next lines is a brief description of what is implemented on each branch:

 > <strong><i>1-miniminimusic</i></strong>: In this first branch are the initial steps with <i>javax.sound.midi</i> package. When this program is executed, it plays a piano note for a short period of time.
<br>

> <a href="https://github.com/GSilvaO/musicbox/tree/2-minimusiccmd"><strong><i>2-minimusiccmd</i></strong></a>: This program have the same goal as the program in the first branch. The key difference is that an user can enter on commandline two arguments: <br>
    - The first one informing what instrument the user wants a note to be played on <br>
    - The second being the note to be played

> <a href="https://github.com/GSilvaO/musicbox/tree/3-minimusicplay"><strong><i>3-minimusicplay</i></strong></a>: In this branch the MIDI events creation was abstracted to a method, and an event was associated to a note so that each time a note is played, an event is registrated within this note. With that, an event is created, and the inner class <i>MyDrawPanel</i> listens the created event and draws a random square on the screen each time a note is played.

> <a href="https://github.com/GSilvaO/musicbox/tree/4-beatboxGUI"><strong><i>4-beatboxGUI</i></strong></a>: This is where the synthesizer program starts to take shape. The interface with the instruments and checkboxes to select which instruments should be played in a certain beat, as well as buttons to control the music flow was developed here. 

> <a href="https://github.com/GSilvaO/musicbox/tree/5-beatboxSerialization"><strong><i>5-beatboxSerialization</i></strong></a>: It was added options of serialize and deserialize beats patterns.

> <a href="https://github.com/GSilvaO/musicbox/tree/6-finalBeatboxProgram"><strong><i>6-finalBeatboxProgram</i></strong></a>: The final version of the synthesizer (BeatBox) program. It was added the chatbox and with that the network logic, as well as some code refactoring. An image of this final version can be viewed bellow:

![Final Program Image](/.github/images/beatbox.JPG?raw=true "BeatBox Final Version")


## How to run this project

> 1 - You can clone this repo (by using ``` git clone ```) or download and extract this repo files.
<br>

> 2 - Ensure that you have Java installed and configured (version >= 1.5).
<br>

> 3 - On the project's main folder, run ``` javac <filename.java> ```  to compile the source file.
<br>

> 4 - Run the compiled file using the ``` java <filename> ``` command.




 