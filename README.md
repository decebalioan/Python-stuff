# Hero_game:
Create a role playing game that will be played on a 6 × 6 grid.
The grid will represent a map and the game hero will start at position (0,0).
Also, upon starting 5 items will be randomly placed on unique positions on the grid.
On each turn the game will ask the user to choose a direction for your hero movement (Left/Right/Up/Down).

The game will continue until the hero’s inventory is full (3 slots).
If the hero steps on a grid block that has an item then the hero must pick it up.
Once the hero’s inventory is full, print the total value of the items in the inventory.
After each turn update the grid and print it to the console. When printing use the following symbols.

1. H - Hero
2. Sword - S (Value - 20)
3. Robe - R (Value 30)
4. Crown - * (100)
5. Empty grid blocks - 

When an item is picked up make sure to provide a meaningful print e.g. ”You have picked up a sword (Value 20).
You have 2 inventory slots remaining.”

# Galaxy_game:
You are asked to build a complex data structure to hold information about
space ships that are sent across 25 different galaxies on research missions. Your
data structure will consist a 2D map of the galaxies where galaxies that are
currently explored are marked ”E” and the rest are marked ”0”. Also it will
contain the total number of ships, a list of crew members (Assume that
each ship is driven by 1 person), a look-up of each crew member and the
coordinates of the galaxy he is currently exploring (E.g. Joe Cooper - (0,0)). In
addition, implement the following two functions.

1. recruit(name,coordinates) - Assume that provided names will be unique.
Coordinates must be a tuple of type (x,y). On each insertion update all
values within your data structure respectively.
2. retire(name) - Assume only names that are currently known will retire.
Update all values within your data structure respectively.
3. printMap(map) - Function that will take your 2D map and print it with
each row on separate line like below

The final requirement is that information is easily retrieved by providing a
key and retrieving the piece of information you need. For example, when queried
with key ”map” your data structure would return the 2D galaxy map.
An example Galaxy Map where galaxies with coordinates (0,0), (4,4) and
(1,0) are being explored would look like this.

E 0 0 0 0
E 0 0 0 0
0 0 0 0 0
0 0 0 0 0
0 0 0 0 E

Do the following function calls then show the result to the demonstrator.
1. recruit(”Joe Cooper”,(1,1))
2. recruit(”Amelia Brand”,(1,2))
3. recruit(”Kevin Doyle”,(1,3))
4. recruit(”Murph”,(2,2))
5. recruit(”Tom Cooper”,(3,1))
6. recruit(”John Brand”,(3,2))
7. recruit(”Nikolai Romilly”,(3,3))
8. recruit(”Donald Doe”,(4,4))
9. retire(”Donald Doe”)

To show each element you might want to do something like this. You are not
obliged to use the same keys with your data structure or variable name.
1 printMap(myGalaxyDS[”map”])
2 print myGalaxyDS[”ships”]
3 print myGalaxyDS[”crew”]
4 print myGalaxyDS[”crewCoords”]
