# cheeseball-games
<--Important guide for anyone invited to work on the project-->
Here is your full guide on how to work on the project.
If you want to add games, you must first go to index.html and go to the Navigation Links section. Then, make an entry following this format:

<a href="games/game(whatever number this game is).html">What you want the game to appear as in the sidebar goes here</a>

Then, scroll down to Navbar. The end of the Navbar secion is where the footer begins. Then, go to the end of the FIRST(NOT THE SECOND) </div> and skip a line. Then, to make a game card, make an entry of the following format:

<div class="game-card">
  <h3>Whatever you want to call the game(must be same in letters, emojis are fine as long as previous entry letters are same)</h3> 
  <a href="games/game#.html" class="btn">Play</a>
</div>

See the last </div> you just made? Notice how the second </div> from before is below this one. Therefore, the one you just typed is now the first one of the two.
An entry like this should never be below or on the same line as the second </div>. Commit changes.
Now, click on the games folder, and once you see file options, above the file options there is a dropdown menu to add files.
Click "create new file" and name it "game#.html"(in this case replace the # with whatever game number this is, rename it using the textbox at the top of the screen in the directory path). Commit changes.
Go down to literally any of the other games files within the folder and copy everything. Paste it into the newly made file.
Go to line 6. Change the first part of the name(this is the name of the game you copied the code from) to the new name, which must be the same as the one you typed in as whatever you wanted to call the game back when you made a game card.
On line 19, there is a thing that says "PASTE YOUR GAME CODE HERE". Below that, there will be an <iframe> element which ends at </iframe>.
Change ONLY the SRC to either the URL of the game OR, if you're running the game off of another unblocked games website, follow these steps:
-Go to the unblocked game site
-2 finger click/right click with mouse outside of game window
-click inspect
-a button on the top left corner will say something like "select an element to view code" when hovered over with the cursor. click it.
-click the part of the game interface(so the part that actually runs the game on the website, perferrably aiming for the entire game display rather than just a play button or something.
-search around in the inspect menu until you find the iframe lines of code(they begin with "<iframe" and so on, and always end in </iframe>
-once you find the iframe html, two finger click/right click on it and select "edit as html"
-cmd + a(or whatever your select all text command is on your keyboard)
-copy all the highlighted text
-come back to the game folder you're working on, and delete the entire code between "PASTE CODE HERE" and "END GAME CODE" and paste the new code you just copied in
-maybe seperate lines to make different aspects(src, id, width, height, etc.) look more organized(messy code is hard to work with)
-you might see something after allowfullscreen like '="" data-wg-content="true"', just delete that. it's unnecessary and doesn't do anything
-IMPORTANT - find the 'id' attribute. it should say 'id="somethingsomething"'. delete whatever is set as the id(keep the quotations) and replace it with "myFrame"
-doing this allows the fullscreen functionality to work

Once you've done all that, finally, go to search.html. Just go to the very end of the most recent entry under "list all your games" and enter.
following the same format, which is shown below, make an entry.

{ name: "name of game, must be same as everything else", url: "games/game#.html" },

yes, even the comma at the end matters.

once you've done this, your game should be on the site. if the iframe(our game display) doesn't load the game, it could either be a device issue, syntax error, or an anti-iframe code set by the developer for security reasons.
  
