# Devlog 07
1/11/26 | jdo1-des
<br>
<img width="722" height="679" alt="image" src="https://github.com/user-attachments/assets/18cbdd85-925d-4879-ab9d-9b99e262fb62" />
<img width="1503" height="770" alt="image" src="https://github.com/user-attachments/assets/0cd08079-09fc-44f3-acd6-79cbc953f99a" />


TLDR: added a starting lobby area for players to wait while friends join<br><br>
I added a mew area where players spawn, this is so they can wait for others to join before starting the game. To start the game players just go through the door in the room. I had some issues with actually teleporting the player to the game map.
The problem was the event to start the game, could be called before the game had fully loaded. This means the game would try teleporting the player to a place that hasnt beeen loaded. To fix this, I made the event wait for the rest of the game to load before it could be called.
This way players are always teleported.
