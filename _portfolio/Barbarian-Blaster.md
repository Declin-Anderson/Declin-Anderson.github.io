---
title: "Barbarian Blaster"
excerpt: "Tower Defense game made in Godot using GDScript<br/><img src='/images/Portfolio/GamePreviewBarbarianBlaster.png'>"
collection: portfolio
---

![Game Preview](/images/Portfolio/GamePreviewBarbarianBlaster.png){: .align-right}
Barbarian Blaster was a tutorial into creating a tower defense game! Barbarian Blaster was created in Godot using GDScript for the language, the goal was to learn about creating pathing for enemies, the grid map node to learn about how to create a tile-based games, and exploring different tools you could use to adjust game elements. Working off a tutorial on GameDev.tv I was able to learn about these new skills in Godot!

![Difficulty Manger](/images/Portfolio/DifficultyManagerBarbarianBlaster.png)
For the difficulty manager I used the Curve property for nodes to set the spawn time and health of enemies to scale with the curve as the game goes on. I the curve starts out low then increases as the game goes on to make it where more enemies spawn as the game goes on and the amount of hits it takes to kill the enemy goes up. This also handles the time of the game to start spawning enemies as the game goes on and when the timer ends it stops the spawn of enemies.

![Enemy Info](/images/Portfolio/EnemyInfoBarbarianBlaster.png)
For the enemy info script, it handles all the logic of the enemies you face in Barbarian Blaster. It handles the current health of the enemy by changing the health as the turrets shoot the enemies, and when they run out of health it adds money to the player bank allowing them to spawn more turrets in the game. It also handles spawning the enemies to the new health the difficulty curves set the enemies to. Lastly, it keeps track of the progress the enemy has made along the lane to the end of the game which if its progress all reaches max it then damages the player's base.

![Enemy Pathing](/images/Portfolio/EnemyPathingBarbarianBlaster.png)
For the enemy pathing script, it handles the logic of the spawning the enemies and seeing if the game has ended. When spawning an enemy, it instantiates the new enemy using the difficulty manager's curve for enemy and adding the enemy to the scene as a child of the node. This also handles stopping the timer for spawning the enemies when the difficulty manager is done spawning enemies. Lastly, it checks to make sure that when an enemy is defeated if the timer has stopped for the game and there no other enemies child to the node.

![Raycasting](/images/Portfolio/RaycastingBarbarianBlaster.png)
Lastly is the Raycast script that handles the mouse clicking on the tiles to spawn turrets. First, it gets the position of the mouse on the screen and generates a raycast to the position of the mouse on the screen. Then, it checks if the raycast is colliding with any objects in the scene and if the player isn't colliding with any object or doesn't have enough money for a turret sets the cursor to its basic icon. Otherwise, if the player has enough money for the turret, then the cursor changes and the player can click on the tile and spawn a turret in its place, spending the money to buy them.