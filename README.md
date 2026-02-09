## Creating an animation using rectangles that is based on Donkey Kong
The animation is primarily using rects as the primitive in the model
The beginning requires text to instruct the viewer to start the video and there is text at the end.
Additionally when Donkey grabs a vine, the rects turn into lines. This makes it a little easier to rotate a line with a fixed start and end position.
Alternatively, I could have used quads for this instead of rects which would have prevented the need for lines. But by the time I realized this issue, I didn't want to drastically change the code.

## Background on the code
The music comes from a restoration of the Island Swing music from Donkey Kong Country on the SNES. 
In the original DK country there were ropes instead of vines. I chose to use green vines since I was first introduced to donkey Kong through Donkey Kong 64. Getting the swing animation was challenging. I initially wanted to use simple kinematics to model the swing and jumping. I didn't like the resulting look of the animation, and found that a simple modified pendulum motion based on triginometry worked best.
Picking up the bananas is a simple pythagorean formula to determine the distance from Donkey to the bananas.
If I was continuing to update this I would have the banaas be a variable of the Vine, which would make it so they wouldn't float around after the vine moves. I would be interested in programming something so the vine moves back slowly to its original state after Donkey releases it instead of it snapping back.

## Connection between the sound and animation
I started by having the trees tied to the amplitude of the music. Since the trees only spawned on the edge of the screen, this made it not as noticeable that there was a relationship to the audio.

I tried to get a connection to the BPM/Tempo of the music that I could use to control the scroll rate of the screen. I couldn't get the functions to work, so I decided to hard code the changes to scroll rate based on my percieved change in tempo.

I added a simple connection between the amplitude and the size of the bananas. This made the bananas pulse on the screen, which I thought looked fun. 


[P5js code](https://editor.p5js.org/gmadhivanan/sketches/zWhSdt1i2)
