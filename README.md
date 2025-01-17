# DevAcadTextBasedAdventure

## Week 2, Assignment 4

## Text Based Adventure Game

### Project Brief
Remember Adventure? Well, we’re going to build a more basic version of that. A complete text
game, the program will let users move through rooms based on user input and get descriptions
of each room. To create this, you’ll need to establish the direction in which the user can move, a
way to track how far the user has moved (and therefore which room he/she is in), and to print
out a description. You’ll also need to set limits for how far the user can move. In other words,
create “walls” around the rooms that tell the user, “You can’t move further in this direction.”

### Concepts to keep in mind:
- Strings
- Variables
- Input/Output
- If/Else Statements
- Print
- List
- Integers

### Deliverables
The tricky parts here will involve setting up the directions and keeping track of just how far the
user has “walked” in the game. I suggest sticking to just a few basic descriptions or rooms,
perhaps 6 at most. This project also continues to build on using user inputted data. It can be a
relatively basic game, but if you want to build this into a vast, complex word, the coding will get
substantially harder, especially if you want your user to start interacting with actual objects
within the game. That complexity could be great, if you’d like to make this into a long term
project. *Hint hint

### Solution
Create an escape room, where you start at a random location in a dungeon and need to find the exit.
Make the size of the dungeon variable, and each room description random for replayability. 
Add loot at random locations for something fun to collect!

### Technicals
Create a 2D grid with rooms from 1,1 to n,n where n is the size of the dungeon as input by the user,
or randomly rolled at the user's discretion. The grid will be implemented as a 2D list.
Fill the grid with random room descriptions, taken from lists of adjectives, nouns etc. similar to the
madlibs assignment. 
Create a separate 2D grid with loot, with a random chance based on the "loot density"
specified by the user or randomly rolled, where 1 = 10% (1 in 10 rooms contain loot) and 10 = 100% 
(all rooms contain loot). Where a room contains loot, randomly generate the amount and store it in the
2D loot array.
Randomly place the exit and start points, ensuring they are not the same so the user must explore!
Define the "edges" of the map based on the co-ordinates of the user, and print that there are walls where
these edges are if they are in a room at an edge.
As the user moves around, print the room description and if there are any walls (edges) blocking their path.
Check for loot in the room, and if there is, print a hint "Something golden glints in the gloom." Also check
if the user has found the exit and ask if they want to continue or flee to safety.
When they flee, print the total amount of loot they've collected.
Add error handling based on variable type and min/max limits where necessary where integers are required, and 
check for valid directions entered by the user based on context (e.g. handle if the user tries to walk through
a wall or collect loot where none exists.)