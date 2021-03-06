# Bagpipe Hero v1.0.0
#### A 15-112 Term Project by Tate Mauzy


## Project Description 
Bagpipe Hero is a game similar to Guitar Hero 
in its basic concepts and mechanics. The general concept
is as follows: while music plays in the background, the 
player hits notes on some sort of controller device (in this 
case, the keyboard), attempting to hit notes on the 
screen that correspond to those in the song. However, 
the catch in Bagpipe Hero is that the game is bagpipe- 
and Scottish-themed. That is to say, not only does it 
have an aesthetic layout that is Celtic in nature, but 
it also features bagpipe music as its available default
songs and incorporates components of playing bagpipes 
specifically into the game, such as having nine notes 
to play (as this is the entire range of the Highland 
Bagpipe) and having to “blow” into the bag (by 
pressing a button) to refill the air to keep the drones
and chanter playing, among other differences. Bagpipe
Hero also incorporates note analysis of music audio 
files such that music files can be uploaded and 
analyzed, allowing for the generation of game levels.


## How to Run the Program
Firstly, Ensure that all files are present and in the
corrrect places. Look and make sure that the directory 
'Code and Relevant Files' contains the python files
'bagpipeHero1.0.0.py', 'gameData.py', and 
'musicAnalysis.py'. Do not move these files from their
position if they are in place. Next, download the 
'Music' folder exactly as it is from the Google Drive
link, and place that folder in the 'Code and Relevant 
Files' directory, too. So long as no directories or
Files have been moved or tampered with, the code should
be able to run after this. Run the file
'bagpipeHero1.0.0.py' to play the game. 

PLEASE NOTE: 
Unfortunately, the audio analysis libraries used in this
project are not compatible with versions of Python 3.7
and later UNLESS you download the Microsoft Visual 
C++ build tools from
https://visualstudio.microsoft.com/visual-cpp-build-tools/. 
You will need to run this project with Python 3.6 or earlier 
if you don't want to download any extra software on your machine.

If you wish to add new bagpipe music to play, add the
music as a .wav file to the directory 'Code and Relevant 
Files > Music > PlayableSongs'. You will then be able to
select this song by entering the title the next time you
run the code.


## Libraries Required
math, random, os, aubio, pydub, pygame, and wave
OPTIONAL: ffmpeg (to remove warning message in terminal)


## Program Shortcuts
- In game mode, press F1 to skip ahead to instantly 
complete the level and go to the score screen with your
current score
- In game mode, press F2 before finishing level to make 
your score ridiculously high (30,000) and guarantee 
yourself a chance to go to the high score screen
- In title mode, press F3 to reset the high score board

## Optional Additional Steps for Improving Program Run Quality

#### Running the Program on later versions of Python
As briefly mentioned in the instructions for how to run
the program, if you want to run Bagpipe Hero in Python
3.7 or later, you'll need to download the Microsoft
Visual C++ Build Tools at
https://visualstudio.microsoft.com/visual-cpp-build-tools/.
They are required for the Aubio module to work on newer
versions of Python.

#### Getting rid of the ffmpeg warning message
Normally, when this program is run, Python will display 
the following warning message:

```
RuntimeWarning: Couldn't find ffmpeg or avconv - defaulting to ffmpeg, but may not work
```

This is because some functions in PyDub (not any used in
Bagpipe Hero) require ffmpeg, an audio processing program 
that can be downloaded from the ffmpeg website at
http://ffmpeg.org/download.html. Please note that you will
want to download it using one of the "Get Packages &
Executable Files" options for your operating system.

After downloading the zip file, you will want to unzip it
(probably using a program like 7-Zip, which you will need
on your machine to do this if you don't have it already) and add the folder's bin directory to your system and user Path variables.

After adding ffmpeg to your path, you will need to install the 
ffmpeg module to your version of Python using pip. 
After that, the game should run without any warning
messages.

I know this is A LOT of work to get rid of one little warning 
message, but if you're a perfectionist like me, this is how
you can take care of it. A patch update will be released at some point to remove PyDub entirely from the implementation.


## Citations for Images, Music, and Font Files
###### Music: All music used in this project was purchased
###### from iTunes. The songs can be found at the following web
###### addresses:
	- MacGregor of Rora: https://music.apple.com/qa/
album/with-purpose/544492272
	- Bagpipe Drone Audio (for training the game): 
https://music.apple.com/ca/album/bagpipe-drones-tuning-
practicing-improvising/1287935155
	- Drum Salute (for training the game): https://
music.apple.com/us/album/re-charged-live/290900495
	- Medley starting with Father Michael McDonald's
Silver Jubilee (playable song and part of theme song): 
https://music.apple.com/bw/album/world-pipe-championship
s-highlights-2000-2005/921061103
	- Medley starting with Tommy MacDonald of 
Barguillan: https://music.apple.com/us/album/world-pipe-
band-championships-2008-vol-1/289664973

###### Images:
	- Bagpipe Silhouette image acquired from 
https://i.pinimg.com/originals/60/1f/bb/601fbb72f76c81f8
c19fe2a6b0e886af.jpg
	- Bagpipe Diagram image acquired from 
https://www.pinterest.com/pin/191614159115761302/
	- Keyboard Diagram image acquired from 
https://en.wikipedia.org/wiki/QWERTY
	- CMU Tartan Plaid image (for video) acquired 
from  https://www.qatar.cmu.edu/event/blelloch/
	- 15-112 Dragon image (for video) acquired from
https://www.cs.cmu.edu/~112/staff.html
	- Steve the Dinosaur image (for video) acquired
from  https://apps.apple.com/us/app/t-rex-steve-widget-
web-game-offline-dinosaur-in-internet/id1128357876

###### Fonts:
	- Roman Unical Modern Font acquired from 
https://www.fontspace.com/george-williams/roman-uncial-
modern
