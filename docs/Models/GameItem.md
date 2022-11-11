# GameItem.cs

## Class Diagram
![GameItemClass](https://user-images.githubusercontent.com/115721045/201144333-d3c568d5-3114-40fa-bdce-7edc21127951.svg)

## Attributes Description
- `ItemTypeID`
   - Unique ID for each type of item. Auto getset.
- `Name`
   - Name of item. Auto getset.
- `Price`
   - Price of item. Auto getset.

## Constructor
- `public GameItem(int itemTypeID, string name, int price)`
   - Sets initial values for the attributes.

## Methods Description
- `public GameItem Clone()`
   - Uses the GameItem constructor to return a deep copy of the current game item.
