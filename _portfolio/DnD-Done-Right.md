---
title: "DnD Done Right"
excerpt: "A large program that has all the information for the game Dungeon's and Dragons in one place <br/><img src='/images/DanddDDDoneRight/main.png'>"
collection: portfolio
---

This is a large scale application me and a friend have been working on for a while. It is ann all encompassing application to streamline the process of making a character and collecting all of the data for the game dungeons and dragons. Currently the project is on hold since we are both at different colleges and our free time has been limited, but we have plans to continue it in the future.

The program was designed to use all the data from all the current books that had been published for the games. with this data the goal was to have a all in one program to look up anything about the game, be it rules, items, abilities, or different monsters. The main purpose of the program though was to create characters and store those characters whenever you wanted. This way you would have a database of sorts of all your characters on a local save.

Current functionality was fairly simple, with a large focus on UI in the early development process. Below is an image of hte main screen. WIth top left showing a selected character. bottom center showing stats and then the left navigation bar allowing the user to select different menus.

![Start Screen](/images/DanddDDDoneRight/main.png)

On the left we made a simple navigation pane that expanded on click allowing for a seamless always accessible navigation system.

![Navigation](/images/DanddDDDoneRight/menu.png)

The first functionality we decided to add was the list of spells and a search feature to look up different spells. Below shows and image of the spell handbook. This takes spells from all sources including UA. All data was scrapped off various websites with a web scrapper i built. You can read more about that [HERE](https://tkketron.github.io/portfolio/Web-Scraper/).

![Spells Searcher](/images/DanddDDDoneRight/spells.png)

This allowed a nice list to be created using C#'s built in datatable class. Every spell was added in with different data types, this allows for sorting the spells in different methods with an intractable table. Shown below is an example of sorting by level, then an addition constraint looking for any spell containing the work fire.

![Sorting](/images/DanddDDDoneRight/sort%20spells.png)
![Searching](/images/DanddDDDoneRight/search%20spells.png)

Some of the spells needs some cleaning up because all of the data is parsed from HTML on different websites. any spell form the search above can be clicked on and it loads up a sub form that shows the data parsed form the HTML. This needs to be cleaned up but the functionality is still there

![Spell Example](/images/DanddDDDoneRight/spellex.png)

The last thing we worked on before we stopped working was the character classes ability and the added functionality of making a character. We didn't get far into to actually add visual updates, but we added sub menus to start the functionality. This including a load character and create character menu with the options to make a random character for things like NPCs.

[Character Creation Menu](/images/DanddDDDoneRight/characterselect.png)

Overall this project was fun and I do plan on continuing it when I have more free time. This project allowed me to expand my abilities and it taught me new skills. Making nested forms was a new technique that allowed me to add a lot of functionality, like easily changed modes from different portions of the handbook to character select and so on.

Check out the code [HERE](https://github.com/TKKetron/DandDDoneRight).