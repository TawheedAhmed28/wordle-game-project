# Tawheed's Wordle

![](./images/WordleEmpty.png)
![](./images/WordleFull.png)
![](./images/WordleFullAccessibility.png)

## Basics of Wordle

Wordle is a common word game (and my favourite 5 minute game!) where the aim is to correctly guess a 5 letter word randomly selected by the computer. You have 6 attempts to do so. For each character in your guess, there is a check:

**If the character is present in the word and is in the right place, the character is highlighted green.**

**If the character is present in the word, but is in the wrong place, the character is highlighted amber.**

**If the character is not present at all, the character is left alone, or in my case, greyed out.**

You win once all 5 characters in your guess turn green i.e. when they are correct.

## Game site and plan

The game can be played [here](https://tawheedahmed28.github.io/wordle-game-project/).

My plan for this Wordle project can be seen below:

![](./images/WordlePlan.png)


The technologies used for this project are **HTML, CSS** and **JavaScript**.


## What's next?

I do find myself checking through this project now and then, and in doing that, I'll probably spot (and hopefully fix) some bugs. As for new features, I would like to come back to this and add different difficulties:

**Nurdle**: For a pellet-sized challenge. 4 letter words.

**Wordle**: For the purists. 5 letter words.

**Hurdle**: For those looking to take a leap. 6 letter words.

I may also look into more accessibility features if required. So far there is only a button at the bottom to highlight the letters differently - amber letters are made bold and green letters are made bold and underlined.

## Anything else?

Just a quick couple of thoughts - some parts of this project were much harder than originally anticipated. For example, checking a submitted guess provided lots of challenges. In particular, situations where the player's guess would contain more of a certain character than is present in the word (e.g. if the word to guess is BUMPY and your guess is MUMMY). At first, all 3 Ms in the guess would be either amber or green. However, since the solution only contained 1 M, the only M in the guess that should be "correct" in some form is the 2nd M, and it would be green (right character, right time). I sorted this problem by creating an object where each character in the soluion was tallied, and then, for each character in the guess, checked if it should be green, then if amber. If either one returned true, I'd take one off of that character's tally in the object.

Another thing to note is that I implemented a feature into my game somewhat unwittingly - that being to reload the game without having to refresh the page. Refreshing the page would have been significantly easier, and if I were aware of the possibility to implement that into my code, I probably would have. But looking back, I'm happier with the way I did code it, as it means it'll be easier to work on in the future if, say, someone wanted to keep track of their gameplay for the duration they had the window open.

### Enjoy the game! <3