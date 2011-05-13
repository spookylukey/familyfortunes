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

Simply download all the files into a folder, and open up 'index.html' in the web
browser. Put browser in full screen mode. Then use the following keys.

 n - next question
 p - previous question
 1 - 5  - correct answer (press again to remove toggle)
 x - wrong answer
 z - remove a wrong answer
 Space - wrong answer, without losing a life
        (if there is a wrong answer in the first deciding phase)

=== Questions ===

Questions and answers are stored in the file data.json. (To avoid XHR
restrictions on localhost, it is strictly javascript, not json). The format
is obvious:

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

== Licence ===

A number of files from differnt sources are bundled:

data.json - includes questions scraped from free questions here:
            http://www.pub-quiz.net/Family-Fortunes-quiz.htm

jquery-1.6.js - MIT/GPL licence

Sound effects - recorded from TV program, assumed "fair use".

BPDots.otf - Font from http://www.backpacker.gr/
             Creative Commons Licence

The remaining file (game.html) is original, and free to use and modify
under the MIT licence.