---
title: "Corralling Cats"
excerpt: "Mobile Game made in the Unity Engine<br/><img src='/images/Game Releases/Corralling Cats.png'>"
date: 2024-02-10
collection: publications
---

![Corralling Cat App Icon | 324x432](/images/Game%20Releases/Corralling%20Cats.png){: .align-right}
Corralling Cats is my first mobile game launch that I worked on! Corralling Cats came to IOS and android at the start of February of 2024! Made in Unity, Corralling Cats is exactly what you think it is about, you are trying to herd cats! You get your cats into their pens through toys that you can place and traps on the map that help to move them around the map, with your goal being to do it in as few moves as possible. Made as a passion project, our goal was to learn about how deployment to Appstore worked, and to form the LLC of Totally not a Bunch of Cats!

![Title Screen](/images/Game%20Releases/TitleHC.png)
As a programmer I did quite a bit of Front-End work for Corralling Cats. The first thing I worked on was creating the Menu system for our game! The main parts were creating an in-game shop that the user could spend their currency on, and a dynamic level select that would allow for us to add newly created levels to the list and it would update the screen and unlock depending on the amount of earned stars the player has collected.

![Cat Store](/images/Game%20Releases/CatStore.png)
I also created a customization screen that would allow the player to modify how their cats look in game. For this, I pulled from the list of accessories and other unlocks and pulled whether from the user saves they have them unlocked or locked. Then, the player could preview the cosmetics on their cat and determine if they want them and then when it got locked in it would update the prefab to the new cosmetics and would be saved for the player.

![Cat Customization](/images/Game%20Releases/CatCustomization.png)
The other main thing I worked on was making levels for our game! I made about half of the levels in the full release and as a puzzle game it came with a lot of testing and mapping out so that I could write out an average for the amount of moves, items used, and turns the player took to get to the end so it took skill to get 3 stars on a level and not that any solution would get the player the max amount. I did the levels both in the Unity Inspector as well as eventually we set it up where you could run a scene in game that would allow you to create the level then it saves it as a scriptable object that we could add to the levels array on our Game Manager.

![Tooltip Screen](/images/Game%20Releases/TooltipHC.png)
You can check out Corralling Cats on the iOS Appstore or the Google Play Store here: [Corralling Cats](https://play.google.com/store/apps/details?id=com.TotallyNotaBunchofCats.HerdingCats&hl=en_US).
