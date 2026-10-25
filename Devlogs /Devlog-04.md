# Devlog 04
25/10/26 | jdo1-des
<br>
<img width="1361" height="767" alt="Screenshot 2026-10-25 182525" src="https://github.com/user-attachments/assets/19693123-763a-4123-a4f8-883291fb2f65" />
<img width="1137" height="671" alt="Screenshot 2026-10-25 190001" src="https://github.com/user-attachments/assets/116c1d7f-2d26-4dd9-a9b7-f51f72a78d6d" />


TLDR: changed the lighting added ambient sound and added in a few jumpscares<br><br>
Before my game wasnt very scary, but that has changed. I made the lighting dark and atmosphere thick so it is hard to see far. I also added some ambient music to make the gameplay feel more intense and scary. 
There are now jumpscares when you die and in a few other parts of the game. The jumpscares work by putting an image over the players screen when it is triggered. There was an issue with getting the jumpscares to work when the monster gets the player.
This was because the jumpscare requires a player as the target, but I had set a character as the target which is different, as characters can include rigs such as the monster. I was able to fix this by creating a new player variabel in the monsters script,
made from taking a player from the character variable already present.
