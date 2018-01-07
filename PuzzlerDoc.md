## Introduction
Puzzler is a memory testing VR application. The game requires the player to repeat the sequence of orbs highlighted in a random order.

The following sections display the final results of the project, explain the design process, illustrate different components of the game, provide conclusions and explore future improvements. 
 
## Results

The game starts with a panel which explains the task that lies ahead for the player.
![](media/vrstart.png?raw=true "Start UI")

Upon clicking on the start button, the player enters a dimly lit room to solve the puzzle.
![](media/vrroomviewcenter.png?raw=true "Room View")

The image below is a link to a video recording of the VR experience on an iPhone. The video shows two rounds of the game:
- First round shows the gameplay when the player is successful on his/her first try
- Second round shows the gameplay when the player is initially unsuccessful

Please click on the image to play the video.

[![](https://img.youtube.com/vi/pZc5vHyaPdE/0.jpg)](https://www.youtube.com/watch?v=pZc5vHyaPdE "VR Experience on iPhone")

## Design Process

Understanding the target audience is important when designing a game. A useful technique for reflecting on and figuring out the target audience for your application is to create a persona. When creating a persona, I tried to answer the following questions:
- What motivates them?
- What is their experience with VR?
- How old are they?
- What do they do for work?

This list of questions is not exhaustive and there may be other factors for consideration when determining the target audience.
 
### Persona

For the puzzler game, I envisioned fun-loving undergraduate students, with a passion for puzzle games. The snippet below is a sample of a potential persona:

![](media/persona.png?raw=true "Persona")

**Jonah**, 19, Undergraduate student

>I am a geek at heart. I love a creative, challenging game.

Jonah is a single, male undergraduate student who loves solving puzzles in his free time. He enjoys music and art, so he likes challenging creative games.

**VR experience**: Beginner

### Sketches

I made sketches of several distinct settings where the puzzler game may be encountered. Some ideas include a cave in a forest, a hidden room in a castle and a deserted barn. Finally, I settled on a cityscape where the game is found in an exhibition room at a museum.

![](media/cityscape.jpg?raw=true "Cityscape Sketch")

I created multiple sketches of the UI which enables the player to transition from the greeting screen to gameplay, and finally, upon successful completion of the game, to restart the game. I decided on a start screen which explains the task of the game so that the player will not be startled by the orbs upon transition of the scene.

![](media/uisketches.png?raw=true "UI Sketch")

I am interested in 3D model building, so I decided to learn SketchUp and designed a simple caged light for my game instead of using the torch prefab. 

![](media/gamelight.png?raw=true "Name")

### User Testing

The most important lesson I gathered from this project is the importance of going in early and often. I performed several iterations of user testing on one trusty test candidate.

The first test involved scaling of the UI canvas. He liked the size and readability of the panel but was annoyed that he had to rotate his head to read the entire canvas. I fixed this issue by increasing the camera distance to the canvas.

Initially, the highlighted color of the ```Start``` button was yellow. He felt that yellow was not a color that indicates forward motion and suggested that the color be changed to green.

When he made a mistake during the game, the failure audio would be played. However, when he solved the puzzle successfully, he was immediately transitioned to the ```Restart``` screen. The immediate transition made the game anti-climactic, so he suggested a success audio to be played upon completion of the game. I implemented a cheering audio clip to be played when the player is successful.

## Scene Breakdown

Upon loading the application, the player is greeted with a ```Start``` panel which explains the game and allows the player to initiate the game.

![](media/startscene.png?raw=true "Name")

After clicking on the ```Start``` button, the player moves through a dungeon gate into a dimly lit room. In VR, the method and rate of movement within the game need to be implemented carefully to ensure that the player does not experience simulator sickness. I experimented with several speeds to allow the player some time to appreciate the surroundings and cheering after successfully completing the game.

The image below shows the dimly lit room where orbs are illuminated in a random order.
![](media/playscene.png?raw=true "Name")

Finally, the player is given the option to restart the game.

![](media/restartscene.png?raw=true "Name")

## Conclusions

I enjoyed the process involved in creating this VR application. I gained a profound understanding of the skills and time required to produce a relatively simple game. These skills include: 
- scene sketching
- 3D model building (SketchUp)
- VR object scaling (Unity and Google Cardboard)
- mood setting with lighting and audio (Unity and Google Cardboard)
- visual and audio feedback to player input (Unity and Google Cardboard)
- UI design sketching
- user testing

Most importantly, I learnt that going in early and often is the most efficient technique to discover and resolve issues. 

## Future Improvements

- Implement a night time cityscape and museum for the background
- Design a modern museum room for the game