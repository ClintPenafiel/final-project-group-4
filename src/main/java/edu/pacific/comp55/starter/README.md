###Overview of the feature###
The feature i'll be implementing is to give the "public item Ransack()" function in Partygoer.java the ability to store data into files. 
Initially the function would return the item to the inventory, and to change this so that we can store the item in a file, we would have to 
utilize java libraries to be able to create and write to files. 
The libraries we are using are:
import java.io.File
import java.io.FileWriter
import java.io.IOException
Additionally, we want to represent the rooms and items, so we should use HashMap for this feature.

###Pseudocode###
Map<house, List<item>> Items = new HashMap<>(); //Initialize the hashmap
Items.put(house.DiningHall, Array.asList(item.BRIMSTONE, item.BISMUTH, item.BROKEN_KEY, item.COFFEE)); //Store the items to the rooms in the map repeat this for each room. 
//Decided to use Array.asList so that the original Array it has the flexibility to be modified in the future.

public item Ransack(){
busynum = 3 //this function cost the NPC or player a busy number of 3
List <item> Items = Items in the room //get item list in the current room
TODO: When function gets called, we get random item in the room 
Save the resulting item to the file
