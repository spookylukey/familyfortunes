== Family Fortunes ==

(a.k.a. Family Feud)

A simple implementation of the LED score board for Family Fortunes, with
sound effects.  It needs a human to read questions and make judgements about
whether an answer is right or not. A simple set of keyboard controls is used
to control it.

=== Requirements ===

All that is needed is a modern web browser. Tested in:

 Firefox 4
 Chrome 10
 Opera 10

Assumes a screen size of about 1024 x 768 or bigger.

=== Use ===

* Download files: https://bitbucket.org/spookylukey/familyfortunes/get/tip.zip
* Extract the files into a folder somewhere
* Open up 'index.html' in a web browser.
* Put browser in full screen mode.
* Then use the following keys:

 n - next question
 p - previous question
 1 - 5  - correct answer (press again to remove toggle)
 x - wrong answer
 z - remove a wrong answer
 Space - wrong answer, without losing a life
        (if there is a wrong answer in the first deciding phase)


=== Playing the game ===

Based on extracts from Wikipedia about the original game show, with
modifications.

Each round begins with a member of each team (in rotation, meaning all players
do this at least once) approaching the podium. As the question is read, the
first of the two nominees to hit a buzzer (or put up their hand) gives an
answer. If this is not the top answer, the other nominee is asked. The team with
the higher answer then chooses whether to "play" the question, or "pass" control
to the other team (in reality, teams rarely choose to pass).

[The person controlling the computer presses 1 - 5 for a correct answer, space
for a wrong answer]

The host then passes down the line of the controlling team, asking for an answer
from each. After each answer, the board reveals whether this answer featured. If
not, a "life" is lost.

[The person controlling the computer presses 1 - 5 for a correct answer, X for a
 wrong answer]

Every time someone gives an answer that is not on the board, the team lose a
life, accompanied by a large "X" on the board with the infamous "uh-uhh"
sound. If they lose all three lives, the other team is given the chance to
"steal" by coming up with an answer that may be among the missing answers. If
this answer was present, the other team win the round and was said to have
"stolen" the points; if not, the team who had given the three incorrect answers
win however much points their other answers had accumulated.

The scores are 5 points for the top answer, down to 1 for the bottom answer.

=== Questions ===

If you want to add more questions/answers, they are stored in the file
data.json.  (To avoid XHR restrictions on localhost, it is strictly
javascript, not json).  The format is simple:

 [
  ["Question 1",
   ["Answer 1",
    "Answer 2",
    "Answer 3",
    "Answer 4",
    "Answer 5"],
  ],
  ["Question 2", ...
  ]
 ]

I used a program to generate this data from sources found online (link below).

== Licence ===

A number of files from differnt sources are bundled:

data.json - includes questions scraped from free questions here:
            http://www.pub-quiz.net/Family-Fortunes-quiz.htm

jquery-1.6.js - MIT/GPL licence

Sound effects - recorded from TV program, assumed "fair use".

BPDots.otf - Font from http://www.backpacker.gr/
             Creative Commons Licence

The remaining file (index.html) is original, and free to use and modify
under the MIT licence.


== Simplified instructions for person controlling computer ==

For initial face-to-face between two contestants:

- press 1 to 5 for a correct answer

- press SPACE for an incorrect answer

Once the question goes to the team, they now have 3 lives

- press 1 to 5 for a correct answer

- press X for an incorrect answer (makes an X appear on the screen)


If a number is pressed accidentally, press the number again to cancel.
If X is pressed accidentally, press Z to cancel it.

To move to the next round, press N.
To go back, press P.

