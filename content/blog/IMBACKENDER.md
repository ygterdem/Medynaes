---
title: "IMBACKENDER"
date: 2023-09-10T00:00:00+00:00
image: images/blog/MUID.png
feature_image: images/blog/MUID.png
author: Erdem YİĞİT
---
### Making games Connected(!)

Im trying to make my own currency for all MEDYNAES games. Players can gain Medynaesium on every games and spend on every games. In Yandex Games SDK defining the user is a hard job, at least for me it was. Players dont have a Identifier for us to reach. Every player has a "Unique ID" but unique ids are unique(!) for every game. So identifying player for 2 game is not easy.

There is a function called "getIDsPerGame" which returns an array of object that filled with userID's from games that same developer made. 

So I had to use this. I get the App ID's and Unique User IDs. Player Creates a database entry on first time when plays my game and adds all the data to that entry. Then if same user playes my another game, players unique id will be on the db for that game. We check if is exist or not. If is we get the MUID for sync the currency if not we create another database entry.

In the moment there is a problem that i didnt found a solution. If player dont have data on the other games, first entry will be the only the current games unique id. Because of that if player play my other games. Unique id will not be exist on the db.

Thats the problem im currently working on.

seia.


for more information Join the **[Discord]("https://discord.com/invite/6j4KjH7ygV")**
