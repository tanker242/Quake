# fortress

Since you've been invited as a contributor you should have the repository in your GitHub profile, otherwise just clone the URL: https://github.com/tanker242/Quake

Select a location to save the repository directory then open up the Quake folder in an explorer window. Extract Kerney's new QUAKE Release zip then merge the contents of QUAKE Release into the new Quake folder. When you open the GitHub Desktop client you should be able to pull, fetch, commit, then push your updates to an desired branch. Once everyone has set up the branches this way all they have to do is make a fetch and pull request to download the lastest version of that branch then run make to compile and test out the program. It is important to note that when you click ona different branch in the GitHub desktop client files will litterally appear and disappear from the Quake folder depending on if you've added or deleted files. This is why it is important we edit seperate branches, then merge them to master once we've worked out the bugs. I will go over all of this on discord later tonight.

Kerney's QUAKE Release file with updated cfg and readme

https://www.dropbox.com/s/w9tdifgaaeq6qy2/QUAKE%20Release.zip?dl=0

---------------         Proposal              ---------------

Gun Game Classic (Submitted version)
Our group is creating a game mod for Quake called Gun Game which is based on the popular Counter-Strike mod. Gun Game is a classic mod you can add to your server that will provide players with hours of fun as you and your friends race to the final weapon and back stab your way to victory. In this mod players will not be overwhelmed by gun choices because they will have the opportunity to use every weapon. It’s a deathmatch type game where each player will be given the same stats, a gun, and a knife; however, once they’ve made a frag with the appropriate weapon they’ll progress to the next levels’ loadout until they are left with only a knife. Players will continue to compete until one player progresses through every level with each gun before claiming victory in the final level with a knife kill. BUT WAIT! Players can knock down their competition a peg by backstabbing them with the knife which forces them back to their previous gun. Gun Game will cause players to change tactics on the fly when their guns change, making for an exciting and unique deathmatch experience. 
        	To make the game balanced and fun, the guns in the lower levels are generally stronger so it becomes progressively harder to frag people and progress through the game. In this mod players can catch up to others and prevent a one-sided game or snowballing player. This leaves the door open to high amounts of skill-based gameplay since players will need to kill someone with a hard-to-use weapon while trying to avoid enemies who want to backstab them with the knife. This will allow games to get more intense and competitive as the match progresses. Even though this game mode can get intense, it is not repetitive, and by starting off with stronger guns newer players can catch up and learn how to play the mod quickly. The mod will be built on the Custom Team Fortress code base to maintain compatibility but will disable most other features when the mod is enabled.


Add Gun Game to votemap (Hunter Osborn)
Disable Starting Class/Custom menu (Aaron Fong)

Mechanics for Weapon levels, de-level with knife kill, and misc gun modifications (Chris Vienna)

Turn off Capture the Flag and Disable doors and backpacks (in the starting areas) (Edward Collins)

Health regen after leveling up (Testing needed to verify balance) (Aaron Fong)

Add global sound effect for level up, grenade level, knife level (Chris Vienna)

Enable deathmatch style spawn points (Edward Collins)

Select fun and competitive map rotation (Hunter Osborn)


Group Members:
Chris Vienna	Edward Collins
Aaron Fong	Hunter Osborn

--------------- Below is Kerney's Readme file ---------------
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
