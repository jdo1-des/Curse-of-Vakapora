# Devlog 08
1/11/26 | jdo1-des
<br>
<img width="577" height="482" alt="Screenshot 2026-11-01 181719" src="https://github.com/user-attachments/assets/53adf161-0dc0-47a5-b6e2-6cd35733c0b1" />
<img width="1472" height="755" alt="Screenshot 2026-11-01 181746" src="https://github.com/user-attachments/assets/e3fc820a-e629-4e95-b5fc-1abe974cc3be" />
<img width="1198" height="757" alt="Screenshot 2026-11-01 112457" src="https://github.com/user-attachments/assets/14fb0088-6d40-4833-81ad-5e50369a42aa" />
<img width="1117" height="717" alt="Screenshot 2026-11-01 181629" src="https://github.com/user-attachments/assets/79676789-ebff-4497-8408-128b126a6189" />



TLDR: added a second ending based around the car in the garage, also added flashlights to improve visibility<br><br>
I added a second ending to my game, where you escape in the car. I had trouble here as I wanted it so you had to refill the car and find a key for it. 
The problem was it wasn't checking if both requirements were met. I tried several different methods to achieve this such as using server events to keep track of what has happened.
What I found works best is a boolean value in the server storage that can be changed when the car is fueled. The other script can then check this value to see if both requirements are met.
I also added flashlight tools to the map, these help players look aorund them. To make them I added a spotlight effect to the modle, and made it so players can pick them up to look around.
