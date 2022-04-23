# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Cashin Woo**

Time spent: **8** hours spent in total

Link to project: (insert your link here, should start with https://glitch.com/edit/#!/neat-shade-button)

## Required Functionality

The following **required** functionality is complete:

* [ ] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [ ] "Start" button toggles between "Start" and "Stop" when clicked. 
* [ ] Game buttons each light up and play a sound when clicked. 
* [ ] Computer plays back sequence of clues including sound and visual cue for each button
* [ ] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [ ] User wins the game after guessing a complete pattern
* [ ] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](https://media.giphy.com/media/4eHYAoHNmrlUdTU95U/giphy.gif)

![](https://gfycat.com/smugabsolutearabianwildcat)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
I used stack overflow. 

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
One challenge I encountered in creating this submission is implementing a timer so that the user loses the game if they reach below 0 seconds on the timer every turn. To overcome this problem I firstly planned out what I needed to change on each file to implement the timer: for instance, adding the timer to the html file, resetting the timer on every turn, figuring out the necessary functions to decrement and update the timer The biggest bug/error I encountered was when I was figuring out how to calculate the time I should delay or wait in between each turn before adding a new, resetted timer; I realized I had to add 1 second for the pause in between rounds, plus the time in between each clue (333 ms) multiplied by the number of clues for that round multiplied by thenumber of clues. The reason why this was complex at first to comprehend was I had to consider the fact that I had decreased the time in between clues as the rounds progressed as a feature to the game. The method I utilized to approach this problem (I realized something was wrong with my code when the timer was going down at the wrong times) was by analyzing what times were involved in between rounds (the tile lighting up animation and the time in between tiles lighting up) and implementing the clueHoldTime, which decreases every round, and multiplying it by progress(# rounds or # tiles) to represent the delay. 

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
After completing this submission I have questions about how important collaboration is to web developers and how exactly they cooperate to create projects on a larger scale. Even doing the project by myself I found myself going back and forth among the html, css, and Javascript documents and I can’t fathom doing so on a larger scale; how are multiple people organized to most efficiently progress in a project when everyone has to utilize functions made by each other? From a cognitive aspect, how do you approach problems, especially when you get stuck on a specific problem? 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I had a few more hours to work on this project I would spend them firstly improving the randomization of the pattern sequence and the number of “levels” in the pattern by scaling the size of the array that represents the different tiles. Moreover, I would improve the visuals and aesthetics of the game, and add a strike counter with “lives” so the user could have multiple tries before losing. 



## Interview Recording URL Link

[My 5-minute Interview Recording](https://www.loom.com/share/61c53ea5d6254ca396ef2821a0716767)


## License

    Copyright [Cashin Woo]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
