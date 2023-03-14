# Nottebot
![Image of Notte from Dragalia Lost](https://yvsdrop.github.io/dl-assets/storysprites/100007_10/100007_10.png)

---

## Video Demo

---

## Description
Nottebot is a Discord Bot made using Python that retrieves adventurer and dragon data from the Dragalia Lost Wiki(dragalialost.wiki) in order to display it within the Discord application itself. It contains the files 'abilities.py', 'advList.txt', 'data.py', 'dragonList.txt', 'skills.py', 'stats.py', 'unit.py', and 'main.py'.

Vio Rhyse Alberia!

### advList.txt
This file contains the list of Adventurers added to the game, with each initialization of the bot updating the list.

### dragonList.txt
This file contains the list of Dragons added to the game, as with advList.txt, this list updates with each initialization of the bot.

### data.py
This file contains the base link for opening specific pages of a given adventurer or dragon. This file also contains a dictionary pertaining to each of the game's elements and a color value related to said element. This is used in order to color code a specific adventurer or dragon.
![Farren, a light elemental adventurer, has the given color code.](https://cdn.discordapp.com/attachments/876171522614652940/1058587365469343874/image.png)

### unit.py
This file contains a class Unit that contains the properties 'Stats', 'Skills', and 'Abilities'. These values are obtained through the files 'abilities.py', 'stats.py', and 'skills.py'. This class acts as a container for these data for easy parsing.

### stats.py
This file parses the wiki page for a given adventurer for their given stats such as HP, Atk, Weapon Type, and Element. This also retrieves their portrait based on their story sprite on (https://yvsdrop.github.io/dl-assets/storysprites/)

### skills.py
This file parses the wiki page for a given adventurer or dragon through BeautifulSoup. The data is split into two arrays containing the name, and description of each of an adventurer or dragon's skill. This allows easy setup for arranging the data as an embedded message on Discord. Alongside that, extra formatting is added in order to match the in game's formatting of a given skill description, alongside with assisting with readability for the more verbose skill descriptions

### abilities.py
This file parses the wiki page for a given adventurer or dragon through BeautifulSoup. The data is split into two arrays containing the name, and description of each of an adventurer or dragon's ability. This allows easy setup for arranging the data as an embedded message on Discord.

### main.py
This file is the main executable, initializing the bot on an added Discord Server. Initialization also checks for any newly added adventurer or dragon and adds it on their given list. Commands are ran by the use of "dl!<advName or dragonName>", such as "dl!The Prince".

![Data Obtained about Euden, The Prince.](https://cdn.discordapp.com/attachments/876171522614652940/1058591228201017374/image.png)

The data fetched is formatted in order of their stats, skills, co-abilities, and abilities.
