COMP86
Assignment 11
Maxwell Anavian and Anju Ishizaki
December 8th, 2019

Important Note:
We have decided to alter our initial design and program from the Assignment 9 that we submitted. Our original plan was to create a number guessing game using TensorFlow.js. One of the biggest problems that we faced was using this API because in order for it to work feasibly and successfully, we needed to train the model by showing it various and numerous numbers of inputs and examples, which was something that we were unable to do in such a short time. Thus, we decided to create an interactive game  speech recognition in an interactive game. 

Challenges:
Some challenges that we faced in creating 'Voicy Bird' include that the word 'up' does not get recognized. (Methods in how we faced this problem are described in the section below).
Another difficulty occured when the command gets called too many times even if the user only says a command once. When the speech recognizer works, it parses through various possible outcomes and chooses the one it thinks is best. Taking the best word was a bug we encountered early on. We were using an interim transcript as well as a final transcript, so taking this out allowed us to more quickly and only get the best guess/
another challenge was getting accurate words. if the recorder is set to on, it is hard to test and background noise often causes it to have trouble analyzing words. by having the user click on the screen to start recording every time, it promises a more accurate recording



User Interface Design:
First, we have made our design simple and clear. Our main goal or purpose of our project is the speech recognition game, so other designs should be kept simple and limited to bring focus and attention to our game. So, the only features that are placed on the website are the canvas and the control buttons (up, down, etc), as well as the score. The control buttons are placed in proximity to each other, increasing proximity compatibility. Since our game is a speech recognition simple version for the game 'flappybird,' a mobile application that aims to control the bird without hitting the green columns We have utilized familiar icons for coins and the game icon to be flappybird. 
Furthermore, we implemented an 'instructions' page so that the user knows what to say, and hence what phrases will bring upon which actions. This can be accessed through saying 'how to play' or 'instructions.' Not just the action commands, but if the user wants to restart or start a new game, they can even do so through the speech recognition by saying 'restart.' 
There are four commands 'up,' 'down,' 'left,' and 'right' to move the game icon, namely, flappybird to move in those respective directions. However, through user testing, we realised that the speech recognition has difficultly recognizing the word 'up'. Since this word is only a two-letter word and has one syllable, it only takes the user minial time to say this phrase. So, when the user says 'up,' the speech recognition sometimes either thinks that nothing was said (because the word is too short) or it recognizes as a different word such as 'app.' Thus, in order to decrease possible user errors in which the program might recognize a different word, we implemented our code so that it registeres 'go up' and 'above' and 'move up' to bring the same result as saying (and the computer recognizing) 'up.' Furthermore, even if the user mistakenly says a random phrase, the program would still recognize and display the phrase/word, but will not do anything because we only have specific commands that would result in moving the bird. 

How to play:
 CLICK anywhere on the screen to start voice recording. The program will not work unless the user clicks on the body to start the voice recording. 
 say the command

 move up / go up
 move down / go down 
 move left / go left
 move right / go right

 'restart' or 'restart game' to restart the game once you hit an obstacle

 'how to play'  or 'instructions' for instructions
