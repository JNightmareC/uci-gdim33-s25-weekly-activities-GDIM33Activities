# GDIM 33 In-Class Activities
## W1
### Activity 1
[Here is my link!](https://docs.google.com/drawings/d/1LMMwPd_Ti7B1PqYQi6EVztdJUvoHxm6a_c0Ajw76yFw/edit?usp=sharing)

1. The gameplay mechanics that are really emerging from my sourcesa cant really be quantified yet, but what I can already think of are probably exploring, collecting, and talking to NPC's! In terms of genre, I get th eemergent value that this game is going to pick up a very cozy, casual, exploration, and even a bit of calming and cute adventure. And with an overall aesthetic and style that I am super interested in delving into is something more cutesie, and colorful, away from what I usually make.
2. Our personal styles and interests are similar (me and Geo), in the fact that we both really enjoy the horror genre, and especially psychological horror. Another thing that we tend to have in common is the art style that we both like to see and use, which is a grungier, and darker artstyle more common with serious themes. The only difference in our builds this time is that I am deciding to tackle a much happier approach.
3. Like my LA, we both are into rythem games right now! It's the game genre we like in common, and they gave me a suggestion of a game, and it was Rock Band 3.


### Activity 2
<img width="960" height="720" alt="My breakdown" src="https://github.com/user-attachments/assets/92d06c0e-b874-4ff6-ab33-bc22badaee9a" />



## W2
Finshed in class activity

## W3
### Activity 1
<img width="1522" height="949" alt="My breakdown #2" src="https://github.com/user-attachments/assets/2b3ae8c3-f614-461f-9597-435227623ca4" />

### Activity 2
1. It is adventageous to save the event name as a scene variable in order to make it easier to call from different scene graphs in the main scene. It makes sure that there would be no typos when invoking that event across scripts, and the name will always change if the coder decides to change the name anywhere else (if the name for the the variable is changed at it's root, it will reflect everywhere else).
2. One debug node that helped me the most was the one on the Button_OK game object. It helped me to realize that my transition wasn't being moved out of in order to get the walrus back into the idle state. Because my Debug wasn't going off, I was able to check that transition node, I fixed the typo, and then The debug log worked and stated that I had clickeed the ok button, and that it exited out of the speach box, signifying everthing working correctly.
3. I think it would be releveant to my verticle slide as I need to make sure players are able to stop moving, and interact with the UI dialouge prompts. I don't want players to be able to move away from the NPC while they are still technically talking to them, it would ruin the atmosphere.
4. The game state is super relevant to me, specifically to animate the player moving, collecting an item, and talkig to NPC's. It would control the ability for the player to actually move when certain states are active, that's how I persive me using game states at least. I need it to be able to scale and organize my code better, and so I can intertwine multiple graphs together to get an interconnected network (like how player states will effect and be effected by NPC states, and Items). 


 ## W4
 
 ### Activity 1
 
 Current features: Currently the player can move, hover over objects to highlight them, collect a cube, and talk to an NPC that has multiple states for a conversation based on how many times a player has talked to them, and what they are holding. 
 
 Playtesting goal: To figure out if there are any bugs for the dialouge on the NPC. 
 
 Playtesters: Giovanni Alexander Solorio, Joshua Paxton

 PLaytesting notes:
 
- I figure now that I need an indicator for what keys to use, as playtesters instinctually went to arrow keys instead of WASD.
- Players seemed to really enjoy the small prototype, they thought the visuals were fun, and the dialogue silly.
- There needs to be a blocker to stop player from moving off the world plane, as they tried to walk off of a mountain, and were able to sucseed. 
- The players got a bit confused at the fact they could move in all directions, so perhaps I could add a better camera angle to indicate that players can move in all planes other than the X axis. 
- They noticed that after you collect the cube, then talk to the NPC after already talking to them with the cube in their inventory one time already, it reverts to telling them that the need to go get the object again, the dialogue only had a small bug and that is it. 

### Activity 2
1. A writer would be able to just add more dialouge without writing any code. They would just need to keep adding more nodes to connect to that NPC text's reply options, and responces. The only thing they would probably need to have coded for them is it they want multiple NPC lines in one Node. 
2. Realistically there is no limit of dialouge nodes that writers can make, they would just need to be able to keep track of responces, but logistically they could just keep going, interweving responces as long as they want.
3. Regenerate nodes basically just adds new "packages" you want to use with your code, those packages are new nodes you want to use, so your scripting graph knows what functions you want to acsess and use, and where to find it. It updates the options you have at your disposal, it's just happening manually every time you need to add a new option.
4.<img width="3024" height="4032" alt="IMG_6823" src="https://github.com/user-attachments/assets/335d93ad-8cf5-424e-9e88-218048adfb2d" />
<img width="3024" height="4032" alt="IMG_6824" src="https://github.com/user-attachments/assets/1bc0c6ac-c7cd-49cc-b797-c49357c1c8bb" />




 
