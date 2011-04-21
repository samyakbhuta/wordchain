A wordchain game using node.js.
==============================

Simple two player game session would be something as follow.
----------------------------------------------------------

	player 1 : elephant
	player 2 : taiwan
	player 1 : nano
	player 2 : orange 
	player 1 : electron
	player 2 : noah
	player 1 : horse

Who is a winner ?
-----------------
##Time based##
The player has to reply back to a challenge in certain time limit. e.g 45 sec. Failing to do so, the challenger is considered won.
Note that, this is simplest of the criteria to determine the winner. The idea is, player who runs out of his personal vocabulary will loose.

Now, consider that session has predefined time limit of 30 min. For that for a long time, both player are extraordinary in reply back to the challange. In that case the scoring has to be employed to determine the criteria.

##Scoring##
Many approaches could be considered where winner is determined by kind of words he brought to play.
### Scoring by length of the word ###
#### Each letter in the word has fixed point units ####
In this case, word elephant would gain player 8 points, while word nano would gain player 4 points.	
#### Each letter in the word has weighted point units ####
Here, each letter has it's own points, much like the game of Scrabble.
	
Wordchain games with ranged vocab 
---------------------------------
Well, here the players agree to use the words only of certain type or from perticular domain. E.g. only the cities of the word.

TODO: Have the code factored in way that such scoping criteria can be introduced as plugin. 

	/
	|-app.js
	|-README.md
	/-test
	/-doc
	/-lib
	/-range
	     |-worldCities.range.wordchain.js
	     |-movieNames.range.wordchain.js
	     |-onlyThreeLetters.range.wordchain.js	
	     |-onlyIfItRhymesWithLastWord.range.wordchain.js	

Players can choose which domain they want to select at the begining of the game session.

Displaying the meaning as well
------------------------------

While exchaning the words back and forth is good a game, it would be really nice, if for each word that get's into the game the meaning is also displayed. We have wonderful dict:// protocol that can be used to fetch the meaning of the words from varied sources. Would love to see how much we can depend on https://github.com/ptrm/dict.json.









