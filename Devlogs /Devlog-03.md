# Devlog 03
23/10/26 | jdo1-des
<br>

<img width="242" height="180" alt="Screenshot 2026-10-23 231236" src="https://github.com/user-attachments/assets/d7c62e26-080b-4c20-a28b-704eca07a1f3" /><br>
<img width="430" height="286" alt="Screenshot 2026-10-23 231310" src="https://github.com/user-attachments/assets/f94eaefa-7d16-4157-813a-a1cabe50011a" /><br>
<img width="283" height="517" alt="Screenshot 2026-10-23 231401" src="https://github.com/user-attachments/assets/86a48add-6c69-40c8-b12f-70d3c779a961" /><br>

TLDR: added locks to some doors and keys to open them<br><br>
I added a lock to the front door as well as the garage and garden doors. To escape the house you must go through the rooms to get the keys to go to the next, befor getting the front door key and escaping. 
I made the lock systme by adding a new function too the selected doors that checks if they have the right key in thier inventory before opening the door. At the start the locks werent working all the time and would only open some times.
But after searching only I found if a item is held in your hand it is stored in a different part of the character then I was checking the key for. This explained the issue as when I wasnt holding the key the door could find the key, but when I was holding it it couldn't.
To fix the problem I added some code to the door's script that checks for a key in the player's hand as well as there inventory.
