# Devlog 02
22/10/26 | jdo1-des
<br>
<img width="338" height="452" alt="Screenshot 2026-10-22 233338" src="https://github.com/user-attachments/assets/1166364e-0ecc-41ab-89e3-22d2df1e48ed" />

TLDR: added enemy that chases player around <br><br>
I decided to take a break from the designing models to do some coding. I created a roblox rig and added a script to it, so it can find and move toward players. 
It uses a simple pathfinding loop where it searches for the nearest player and moves toward them.
I had trouble getting it to path through the doors because I wanted it to be able to pass through them and not get stuck.
To fix this I changed the door scripts so the enemy could open them. However, this still didnt work as the enemy could see through the doors and path to players on the other side.
To fix this I had to add code to the door script to make them appear invisible to the enemy so it would move through them and thte dsoor opening code would ensure the doors actually open.
