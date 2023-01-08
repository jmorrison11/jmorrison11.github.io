<!-- layout: page
title: "addressbook"
permalink: /addressbook/ -->

# Loading and Using Binary/IO Files (Address Book)

I built these address programs using text files in the IDE Netbeans. 
I chose an address book because it is one of the easiest ways to demonstrate a use of methods, use of objects, and use of loading in text files. 
This is nothing visually interesting about this project nor does it play music.

- Contact Object
  - This is the empty contact file that I made to build the generic “person” in my address book. 
  Using simple variable types such as strings and a long to represent name, email, and phone number. 
  I created all the setters and getters by hand in this program (though I do know how to do the “shortcut”) as well as an example of a toString().
- Main Method
  - There are quite a few methods within the main class. The two that are most important here are the “loadFromFile” and “saveContactsToFile.” 
  - The “loadFromFile” takes the information from the file name “AddressBook.txt” and loads it into an Arraylist that is being used by the program. 
  I had to parse the long variable into a token so it would be usable by the file. 
  - The other method “saveContactsToFile” takes the ArrayList() 
  that I created (that takes inserting different contacts in from the previous save file) and saves it onto the AddressBook.txt file so you can look at them again.  


##### [the repository](https://github.com/jmorrison11/AddressFile)
###### [back to home](jmorrison11.github.io)
###### [back to project list](https://jmorrison11.github.io/projects)
