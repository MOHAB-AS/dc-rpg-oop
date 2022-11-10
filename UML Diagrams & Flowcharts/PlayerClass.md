# Engine/Models/Player.cs

## Class Diagram
![PlayerClass](https://user-images.githubusercontent.com/115721045/201091070-c3eb58bc-7c45-4184-b06b-264b2cb9a999.svg)

## Method Descriptions
- `public void AddItemToInventory(GameItem item)`
  - Adds a game item to the player's Inventory list and notifies the Weapons attribute of change.
- `public void RemoveItemFromInventory(GameItem item)`
  - Removes a game item from the player's Inventory list and notifies the Weapons attribute of change.
- `public bool HasAllTheseItems(List<ItemQuantity> items)`
  - Checks whether the player has all the items needed for a quest in his Inventory list.
