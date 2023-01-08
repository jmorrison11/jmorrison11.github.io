<!-- layout: page
title: "animelist"
permalink: /animelist/ -->

# Scenebuilder with API List (MyAnimeList)

I built this program using the IDE Netbeans in the language of Java. The GUI was built in the JavaFX program called scenebuilder. 

![Here is what the GUI looked like to give an idea of how the project worked](animelist.png)

- I have one instantiable class with:
  - At three fields (instance variables).
  - One constructor.
  - Get / Set / Property methods for each instance variable.
  - A toString method.
  - An equals method.
  - An extractor method.
- A GUI interface created with SceneBuilder.
  - A ListView.
  - A detail section that includes one Label and one TextField for each field.
  - Three buttons that allow the user to Add, Update, and Delete items.
  - Three additional buttons that allow the user to load data from an API, save data to a file, and load data from a file.
- A Controller that:
  - Populates the TextFields (or other controls) when an item is selected in the ListView.
  - Provides code for all six buttons.
  - Bind the buttons so they are appropriately enabled / disabled.
- API functionality:
  - Load data from an API.

- I used an FXML document controller to add functionality to the buttons, list view, and text boxes. 

- It uses an API that is filled with quotes from anime shows, the API is sorted by the title of the anime. Using gson and json I called the API based on the 
name of the anime you would enter into the text box. 

##### [the repository](https://github.com/jmorrison11/MyAnimeList)
###### [back to home](jmorrison11.github.io)
###### [back to project list](https://jmorrison11.github.io/projects)
