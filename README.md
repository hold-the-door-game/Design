# Design
This repo is intended to collect up to date design decisions across architecture, game mechanics, and aesthetic concerns

Brainstorm document can be found here: https://docs.google.com/document/d/1yXbnOIgItcJdBx7NQhTvKmST8pfrpTZdCWM-wNcKHlw/edit#

**Elements of Prototype VS01**
*Stage*: The walkable distance of a walker.
*Door*: A door at either end of the stage. It can be closed, at some distance of open, or full open. The less open, the more endurance is required to open it to full.
*Crossing*: Crossing is when a walker enters an open door. One point is rewarded for each walker that crosses.
*Walker*: A character that walks across the stage. If the user holds the action button when a walker is within range, they can interact with the door by opening it / holding it.
*Holder*: A walker who holds the door open (i.e. they pause their progress across the stage but the door remains open).
*Passing*: When the door is being held open by walker-W1 and there is walker-W2 in range, if the user lets go of the action button and presses it again, W2 becomes the holder and W1 crosses.
*Range*: Some smaller distance of the whole stage, close to the door, that a walker needs to be within to interact with the door. When passing the hold, if the pass happens at the widest part of the range it eats a decent amount of W2's endurance as the door has closed the most, medium range eats some as it's still almost open, and close range eats none as the door has essentially remained full open.
*Endurance*: A finite, consumable attribute of a walker. It is consumed quickly by opening a door, slowly by holding a door, slightly restored when a crossing walker acknowledges the holder, and slightly subtracted when a crossing walker does not acknowledge the holder
*Reach*: An attribute of a walker. (the longer the reach, the longer the range)
*Acknowledgement*: A walker can give or not give a holder acknowledgement, which effects the holder's endurance.
*Speed*: An attribute of a walker determining how fast it moves from one side of the stage to the other
*Story Node*: A portion of the level's story that is revealed each time a walker crosses when there is a holder

