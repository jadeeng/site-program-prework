# site-program-prework
# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Jade Eng

Time spent: 4 hours spent in total

Link to project: https://glitch.com/edit/#!/site-prgram-prework?path=index.html%3A15%3A11

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [x] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories: 

ezgif.com-video-to-gif(1).gif![image](https://user-images.githubusercontent.com/51209243/112430590-99350200-8cfb-11eb-8d52-7e08f45fbeec.png)





## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.

https://programminghead.com/how-to-play-audio-in-html-using-javascript/
https://www.w3schools.com/css/ 
https://stackoverflow.com/questions/4589451/documentation-for-javascript-audio-methods


2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words)
I had difficulty getting the game to continue past the first tone. I decided that it would be best to check the outcome through console log responses and then work backwards from what responses I did and did not see. First, I made sure that the rest of the console log responses in the web developer window displayed the correct responses, e.g. "user guessed:x" when pressing all four numbers. Since all of the game buttons worked correctly, I moved to the winGame() and loseGame() functions, as these were the functions that called the alert box telling the user that the game ended. I found no error with these functions. 
After determining that the last portions of the game’s logic wasn’t the issue, I moved backwards through the functions until I finally realized that I mistakenly wrote two guess(btn) functions, the first one with an empty body. Deleting this unnecessary section allowed the game to proceed as intended. 


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words)
As I started working on the add ons for this game, I wondered how I could transform this into a multiplayer game with players in different areas. How can I make this game cross-platform, so that users can play it from any device of their choosing without having to rewrite code in different languages? How would I go about hosting this game on a webpage versus and application? I’ve also gotten more interested in how front end and back end languages communicate with each other, how data is stored so that it can be accessed for later use.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)
I would add the following features to the game:

The user can pick from different uploaded songs to play back in their entirety. The songs are preplanned and short.
In order to do this, more buttons would have to be created. Maybe a piano like appearance?
This would definitely help with the overall functionality of the product. Memorizing music pieces line by line is a technique that I used when I was younger, so maybe for shorter pieces and new players, learning to play back a song note by note would be beneficial.

The game has points.
Each successful turn adds x amount of points. When you’re on a “streak”-- getting correct answers consecutively— more points are added.
Instead of automatically ending the game, the user has to start over from one tone and build themselves back up. 
The game can either end on a timer, when the user decides to press “end,” or the user can determine how many tones would count as a win in the beginning.

A user can play against another user in alternating turns. 
Whoever makes the first mistake loses.
The amount of time each user takes on a turn can be added up into points?






## License

    Copyright Jade Eng

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
