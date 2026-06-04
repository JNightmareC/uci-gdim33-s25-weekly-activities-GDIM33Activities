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



## W5 

### Activity 1
Basic steps:

1. Make a state machine that has 2 states to move into and two transitions to move in and out of each state
2. make animations on a key machine in Unity (squash and stretch)
4. add transition conditions and animations into the transition nodes and main block nodes

Detailed step:
1. make a state machine on the NPC's graph with two states labeled idle and talking
2. connect two transitions to and from each other that transition states
3. in the idle state, attach a debug log to make sure that that node is a constant
4. in the talking state, add a debug log to make sure this state is also being entered when the state is transfered out of
5. in the node going from idle to talking, attach nodes that check conditions from a C# script called Full Dialouge in the AdvanceDialouge() meathod to check a variable called "_talking"
6. if talking is true, the graph machine will trigger the talking node and send messages to the console 
7. if talking is false, it will go from talking state, back to idle and send messages back to the console
8. go onto the unity animation tab, and create a new animation, squashing and stretching horizontally for the idle animation, add it to the idle node to play animation
10. do the same thing for the talking animation, in the verticle, then hook it up to the idle node to check if it works and looks correctly
11. then move the talking animation to the talking state node.


### Activity 2

Today I was able to make a new scripting machine to make two new animations states for my NPC. I created a talking animation in unity and hooked it up to the machine, and a idle animation also animated in unity, and added to the machine as well. Another thing I was able to acomplish was the fixing of the player state machine in order to allow them to play a "pickup" animation whenever the player clicks on a collctable object, practically just adding a new state to that state machine. Overall, I made a lot of progress. 


## W6

### Activity 1
 
 What's new: I have expanded the enviroment, 2 new "trinkets", added new dialouge, added a rudimentary gate, and a way to pass that gate with the complicating feature. 
 
 Playtesting goal: To see if there are any bugs with the dialoluge branches when you pick up multiple items and talk to NPC

 Link: https://jnightmarec.itch.io/my-darling-star-milestone-2-vertical-slice
 
 Playtesters: Giovanni Alexander Solorio, Joshua Paxton

 PLaytesting notes:

- Player liked the vibes a lot
- camera clips through the walls a little bit (not really a concern for now)
- Arrow keys still work, which they shouldn’t 
- Need to be more intuitive 
- Play a little text when trying to walk up to the barrier without a gift
- Players are forced in bounds, which is good
- No game breaking issues 
- The state machine works 
- They thought it was peak 
- They needed more direction to click the gate once getting the gift
- there were no bugs with the dialouge system


### Activity 2

1. The multiply setting makes te=he resulting color darker because the values of the RGB (0-1 for each value) will be multiplied to eacha other, and if they're percentages, or in this case decimal fractions, multiplyinga number by a decimal it will get closer to 0 (essentially you are dividing). The closer you get to 0, the closer you are to black, hence the color multiply is applied to is darker. 
2. If you apply it to transperancy, then it works the same as an RGB change in multiply. It will divide the opacity of the Alpha values it was applied on when combining. The closer it gets to 0, the more transperent the object it, the closer to 1 the more opaque.
3. Those shaders get UV values from each vertex on the models mesh,which all each hold some sort of UV position data that has a pixel of that texture maped out to it.
4. I am not really into math very much, but I do agree that this is really interesting to me, especially since I want to get into 3D modeling and I really want to get to know how to do this so I can make my own shaders or textures and maps. It's pretty cool. 

## W7 

### Activity 1
1. The data from vertex color node came from each vertext of a mesh, which has color data baked onto it.
2. I can only assume it's blended at the edges because the vertex edges are being interpolated over the distance of the mesh.
3. It is less detailed because instead of sampling from a texture with set pixel colors it can pool from, it is simply blending colors between vertexes relitive to each other. The reasone we would use Vertex Color to either debug, like in the activity, or we would use it for very simple objects that need colors, mainly because of storage space in a game as textures take a lot of space, and not every object needs a texture.
4. From what I can see, there is an area on the shibas left flank where there is a green patch in th eblue randomly. This can only mean that is is pointing in a different direction than all the other faces around it.
5. Another way you could debug and test is to input the UV map to see if anything looks off. 
6. There is a lighting error there because the face of that specific area is facing in the wrong direction in comparison to all the other faces of that part of the model.
7. I think the reason addative is used is because it blends the colors of the texture, with the colors of the world around it, this completely negates the color black, and because the "background" of the texture is black, it won't show up anymore.



## W8 

### Activity 1
1. In the build I have recently added a new NPC with new dialouge, an end screen, and added a new sprite for the gummy worm object.
2. https://jnightmarec.itch.io/my-darling-star-milestone-3
3. Does the art seem consistent and cute vibrent.

Playtesting notes:

- Player was trying to climb on everything
- Player can open gate right after getting the ring, need to fix that 
- There’s clipping issues, but I can’t fix that necissarally
- lower planes players walk on 
- Liked animations
- liked character designs
- vibrancy was good
- players enjoyed it overall
- change gate area to be a full gate so players cant clip the ground
- dialouge works perfectly, so does end game state, overall it is much more polished than last time



### Activity 2
1. We are using them to compare values in the stencil effect by saying, first for the shiba object, that when it renders before anything else, it needs to to always be drawn and replace other things that may pass on it or around it (specifically for the outline). For the outline, it is only able to be drawn when there is not an item or object (shiba) on top of it, and will only doraw on the area around where it is supposed to be drawn. It uses the less than funciton, when there is less object/ pixels there.
2. The shiba is being respawned twice specifically. The reason it is being redrawn twice as an opaque object, and as a stencil, is to make sure that it is always drawn before the outline stencil so the outline can verify the points where it needs to render.
3. We don't want to multiply the color of the shadow and the value of the base texture, because we don't want to dampen and bring down the color of the actual texture itself, just it's shadow. If you multiply the two together the resulting texture is just black.
4. It enablesand disables the effect because the effect only effects the Shiba when it is on the outline layer, so if it's on any other layer, it won't do anything at all. 



## Week 9

### Acrivity 1
We chose Minecraft


We chose these two:

Potion of nausea 
- we would probably get a noise gradient
- and multiply the scrollomg of its UV's by time delta time, and the speed for however fast you want it to go
- they you want it to interpolate randompy so it warps viably in random directions smoothly
- You also want to have the effect to have a timer dependant on how long you want it to effect for, then when its done, have a curve ease out of it
- you could enable and disable this volume soflty to make it ease in and out from scripting graph once it's done

Outline
- we get the normal vector and want to multipky it to a thickness
- once you do that, then you need to add it to a world position based on the item hovered over
- and you input that to the position vertex with a color node on base color
- when it comes to changing it when its being hovered over, you can have the shader only effect a certain layer (which could be outline)
- so when its hovered over (the block), the outline layer will be switched to, and the mesh material can be set as active
- when its hovered off of, it is turned back to the default

### Activity 2

Since I was able to finish my shader, and hook it up to be usable, I was able to work on something else from my game. I improved the gameplay a bit by making one of the items a bit harder to find, by adding the ability to move a wooden block. I had to use a raycast and was able to snap the position of the gameobject to the mouse. This is just to add more chalenge to the "secret" item since it's supposed to be harder to find compared to the other items. 

https://github.com/JNightmareC/VerticalSlice/commit/ef7c86d1b993b9e0dc9e516514837bd82dad3a9d


## Week 10

### Activity 1

What's new: 


I had to change the ability for how the player is able to grab onto and move the wooden box. Another thing I added was the togled sound effect, and music in the overworld.


[Itch](https://jnightmarec.itch.io/my-darling-star)


Playtest goal:

- Testing shaders for bugs 


Playtest notes: 


- Noticed a bug where the gummy worm doesn't give you the correct dialogue node 
- She liked the outline shader 
- She liked the crayon vibe that it brought
- She noticed no other bugs aside from the worm issue
- 
- I asked another playtester to look at my game and they found an issue when grabbing the worm first, it soft locked the game
- I found two small errors that caused this, and they will be fixed this class

### Activity 2

#### Planning Strategy

I would say in general, breaking down your game into bubles would work best, along with making a comprehensive breakdown of how to set up the main systems of the main mechanics help a lot. Game designers can use the bubbles to lay down the most complex systems or game objects they might have, and in those bubbles, they give very breifly what each would need in order to function. If bubbles seem to big, they should separate them even further to be more specific after writing the base down. Then after, players should make arrows with notes that lead into other bubles that interact with the main. After this, I would say using a step by step breakdown of the main unity systems you would need to use would be beneficial, but of the main mechanics only to get a gauge of how intesnsive the meat of your work will be. You can see how long your plan for that mechanics will be based on how long his steps are. 

#### How planning effects scope

Planning effects scope by showing you, the designer, how much time you actually have to complete everything you have to do. If you are able to plan, you are able to refect and see if all things you have are reasonable to complete. That is via seeing the steps you'd need to go through, the ammount of bubbles you'd need to make and add content to, and the ammount of connections through the whole system. 



### Activity 3

Today, I fixed three errors on my slice. My the first fix of the day was re-checking an issue with grabbing the gummy worm so that now the dialouge nodes work and enter correctly. The next issue I fixed was one where players could climb onto an object they weren't suposed to climb onto. The last thing I fixed was a button UI issue that was stopping players from hovering over them so now they highligt and track correctly.

[Here is the github link](https://github.com/JNightmareC/VerticalSlice/commit/1cf2fa9f5d67cf050c74341aa3d879230772e153)




 
