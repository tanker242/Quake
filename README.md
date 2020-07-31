# fortress

Since you've been invited as a contributor you should have the repository in your GitHub profile, otherwise just clone the URL: https://github.com/tanker242/Quake

Select a location to save the repository directory then open up the Quake folder in an explorer window. Extract Kerney's new QUAKE Release zip then merge the contents of QUAKE Release into the new Quake folder. When you open the GitHub Desktop client you should be able to pull, fetch, commit, then push your updates to an desired branch. Once everyone has set up the branches this way all they have to do is make a fetch and pull request to download the lastest version of that branch then run make to compile and test out the program. It is important to note that when you click ona different branch in the GitHub desktop client files will litterally appear and disappear from the Quake folder depending on if you've added or deleted files. This is why it is important we edit seperate branches, then merge them to master once we've worked out the bugs. I will go over all of this on discord later tonight.

Kerney's QUAKE Release file with updated cfg and readme

https://www.dropbox.com/s/w9tdifgaaeq6qy2/QUAKE%20Release.zip?dl=0



---------------Below is Kerney's Readme file---------------
How to mod CustomTF:

1) The source code is in ./fortress/source code. Open that folder up and look at the files. 
2) Open any of the .qc files, change something, save it.
3) Double click the "make.bat" file there and that compiles your code and deploys it to the right folder.
4) If it failed, go back to step 2.
5) If if succeeded, launch the server (if it isn't open) by running "Launch Server" (from this directory, not the source code directory). If it is open already, type "restart" from the server's console.
6) Launch the client by running "Launch Client" from this directory and test out your code.

If you want friends to play with you, then you'll need to open up the port on your firewall port 27500, and then they should "connect 1.2.3.4" where 1.2.3.4 is your ip address. If you want it to be automatic, edit the ./fte/autoexec.cfg file and put in the ip address to connect to rather than localhost.

Using Visual Studio Code:
1) Download VS Code from Microsoft's Website
2) Install the QuakeC extension (from the file->settings->extensions menu)
3) Set VC Code to automatically detect the character set (from the file->settings->preferences menu, search for "encoding" and either check "auto guess encoding" or set the encoding by default to "iso88591"). This stops VS Code from breaking the extended ASCII codes baked into some of the files that do colored printing.
