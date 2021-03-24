# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Ricardo Fuentes

Time spent: **7** hours spent in total

Link to project: https://glitch.com/edit/#!/adorable-six-comet?path=README.md%3A64%3A991
## Required Functionality

The following **required** functionality is complete:

* [Yes] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [Yes] "Start" button toggles between "Start" and "Stop" when clicked. 
* [Yes] Game buttons each light up and play a sound when clicked. 
* [Yes] Computer plays back sequence of clues including sound and visual cue for each button
* [Yes] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [Yes] User wins the game after guessing a complete pattern
* [Yes] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [Yes] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [Yes] Buttons use a pitch (frequency) other than the ones in the tutorial
* [Yes] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:

Winning Game: http://g.recordit.co/oCedEOnkRb.gif  
Loosing Game: http://g.recordit.co/T8nrtez70c.gif


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

[https://www.techotopia.com/index.php/JavaScript_Variable_Types, https://www.techotopia.com/index.php/JavaScript_Variable_Types,https://www.rapidtables.com/web/css/css-color.html]

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it?

While working on this project, one of the challenges encountered was with the Document Object Model (DOM) as I have not seen this technique before. Only being familiar with C++ I had to read more into this command from the assignment and the resources provided. With this research I was able to comprehend the purpose of this line of code which helped me understand the rest of the functions used when implementing the DOM. Another challenge I came across was understanding the sound synthesis functions since they included functions not so familiar. To tackle this, I broke the code line by line making it more readable to myself. For example this line of code “g.gain.setTargetAtTime(volume,context.currentTime + 0.05,0.025) “ found on the function startTone(btn). 
It was unfamiliar to at first but with the knowledge I have learned in class I was able to put pieces together. Like how g represents the volume, gain represents the context of the button being pressed, and the setTargetatTime correlates with the currentTime + .005,0.025. After understanding this line of code, I went back to the top and began reading line by line to better understand how all the functions are working together. Breaking down the code for me gives me a better understanding and makes me more comfortable when editing the code to help debug if any issues occur. For example, I went ahead and added two extra buttons and when adding a specific frequency to each button under the freqMap I was presented with an error. It was helpful to pay close attention to the syntax and realized that the last button should not have a comma included. A very small error could have prevented me from adding these two new buttons, but I was able to debug and resulted in implementing two new game buttons. 


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

 After completing this project, I did have some questions regarding the web development. As far as web development what are some of the common mistakes new developers make? After finishing a webpage does this require maintenance and if so which part of the code must be updated? Also, how do you make a webpage secure and reliable? Do web developers work in teams and divide the project into sections? What are some of the most helpful tools web developers use to increase productivity? I noticed we made a GitHub account as well as glitch, will these be the main tools we would be using when intern? 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

With a couple more hours of work I would have liked to spend it on adding all the optional features. I was able to add two new game buttons and change the color of the start button. The next feature I would have liked to add is the random pattern by using a (math.random) function. This would allow for the pattern to be shuffled around every new game which would be great so that the player does not memorize the pattern. An additional feature I would have liked to implement is the timer. This would make the game more challenging by setting a limit on the time a player takes to repeat the correct pattern. As I was reading on this function, it would require HTML code to add an additional visual of the clock. Then I would imagine this would require a DOM in java script to link both functions together. This would also require if-else statements. For example, if a player repeats the pattern within 5seconds the game continues. Else, if the player goes over 5seconds the game will end. 



## License

    Copyright [Ricardo Fuentes]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.