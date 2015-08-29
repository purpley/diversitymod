welcome to diversity mod for linux.
all the hard work was done by duneaught, all i did was change some pathing stuff, convert a .ico file to .xcb or whatever it was, etc, etc.

notes: i'm running ubuntu 12.04, you'll probably need to change some of the pathing stuff if you have a different setup.

your TODO list:

download all the python modules that you need to run TK. for me that was python-tk and python-imaging-tk.
if you're on ubuntu you can do:

sudo apt-get install python-tk python-imaging-tk

make a symlink in your SteamApps/common folder to Steam/ubuntu12_32/ (or wherever it looks for the steam executable) 
yeah, i could have done something more comprehensive/elegant but i'm drunk and no. do it yourself.

for me, this was done by:

cd ~/.local/share/Steam/SteamApps/common
ln -s /home/purpley/.local/share/Steam/ubuntu12_32 ubuntu12_32

obviously change purpley to whatever your username is. unless you are also called purpley. 

then you need to make the diversitymod script an executable:

chmod +x diversitymod.py 

and then you should be able to run the diversitymod.py script by:

./diversitymod.py

you'll need to set the correct path to the isaac executable ( run-x64.sh in "The Binding of Isaac Rebirth" folder ) and then you should be set!
