# Devlog 06
30/10/26 | jdo1-des
<br>
<img width="1204" height="715" alt="image" src="https://github.com/user-attachments/assets/5a41abc6-4a18-4789-b636-81a0ac61a852" />

<img width="1291" height="757" alt="image" src="https://github.com/user-attachments/assets/ccaedfc6-6755-4041-9bcd-c3b34647dafc" />

TLDR: added a cutscene and end area for when the player escapes<br><br>
I made a cutscene that triggers when the player makes it out the front door. I made this using the tween function and changing the players camera to look from a part in the workspace.
The way it works is the players camera is set to look form a part in the workspace, then using tween I move the camera to another part in the workspace. This took a while to make due to the complexity of getting it to all trigger write.
A mistake I made was making my cutscene a script rather than a local script, as only local scripts can affect the players camera. And then when getting the monster model to appear behind the player I need to use a regular script instead of local script. 
This was because a local script cant affect the server and so the changes wont apply to all players. I also added an end room where players get teleported to after escaping. 
This room is pretty simple at the moment but as I add more to the game I will add more to this room.
