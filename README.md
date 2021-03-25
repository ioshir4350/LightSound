# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Isfar Oshir**

Time spent: **3** hours spent in total

Link to project: https://github.com/ioshir4350/LightSound

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

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [X] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
https://i.imgur.com/jzUgKKD.gif


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
I used VS code to create the app instead of glitch. I used Stack Overflow
to solve one warning that came up.

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
While creating this submission, everything seemed pretty streamlined. But I wasn't using glitch to develop it because I'm more used to using VS Code to work on web development related projects, so I used that instead. Now, I'm not sure if this was the reason why I had the following problems but it could potentially be it. There was an issue with my browser finding the JS and CSS files even tho I had the same file tree as the GIF on the pre-work instructions. But it was an easy fix: I just had to get rid of "/" from "/style.css" and "/script.js" in the src. I was having another problem with the audio section of the code. When I used the provided code, my browser's console had a warning saying "The AudioContext was not allowed to start. It must be resumed (or created) after a user gesture on the page." Therefore, I pasted the warning in to Google and went on to Stack Overflow, and found out Google has a new policy where after playing the audio, you have to call the resume method. Therefore, I called the resume method after the play function was called. Besides those two errors, everything else seemed fine.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
After completing my submission, I didn't have the type of questions one would expect to have since I already learned how to use HTML/CSS/JS and have used it for quite some time now. But the audio portion of the project was new to me. I've implemented audio before in one of the previous versions of my personal website (I have now removed the audio because thought it was unnecessary), but I did it with React. I havent done it with vanilla javascript before, so this was new. So I suppose my question is how does the AudioContext work? Besides this project, I've had a few questions such as how would one program the backend with more traditional languages like C++ and Java? I know how to do it with more modern stacks such as node.js, flask, and django, but I want to learn how to do it with C++ and Java just as an interest, even though I hear companies aren't really doing that anymore. When I find more time, I will probably try to learn implementing those. I also want to learn more about asynchronous functions and how we can use them to run concurrent requests. 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I was able to find a bit more time, I'd be able to continue making the project better. First, I would include all of the optional features. Then, I would probably add more multiplayer features. For example, a leaderboard system can be implemented if we incorporate a back end. I could also add more multiplayer features where one player can have a turn matching, and another player can have the next turn. To make that live and not make it mandatory for the next player to keep manually reloading, I would have to use Socket.io, a node.js dependency I used in the passed to make a live messaging app.



## License

    Copyright Isfar Oshir

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.