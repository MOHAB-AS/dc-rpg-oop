# Player.cs

## Class Diagram
![PlayerClass](https://user-images.githubusercontent.com/115721045/201091070-c3eb58bc-7c45-4184-b06b-264b2cb9a999.svg)

## Attributes Description
All `private` attributes in this class should have a private backing variable and a public variable in which the getter returns the value of the backing variable and the setter sets its value and calls the `OnPropertyChanged(nameof(Var))` function. **ex:**
```
        private string _name;
        public string Name
        {
            get { return _name; }
            set
            {
                _name = value;
                OnPropertyChanged(nameof(Name));
            }
        }
```
- `_name`
  - Represents the name of the player.
- `_characterClass`
  - Represents the class of the player's character.
- `_hitPoints`
  - Represents the health of the player.
- `_experiencePoints`
  - Represents the number of exp points the player has.
- `_level`
  - Represents the level of the player.
- `_gold`
  - Represents the amount of gold the player has.
- `Inventory`
  - Represents the list of game items the player has. Auto getset.
- `Quests`
  - Represents the list of quest status the player has. Auto getset.
- `Weapons`
  - Represents the list of weapons the player has. Use lambda expressions `=>` and `ToList()` LINQ method to create a list from the Inventory that consists of game items that are of the `Weapon` subclass.
  
## Constructor
- `public Player()`
   - Initializes Inventory and Quests attributes by creating new `ObservableCollection`s.

## Methods Description
- `public void AddItemToInventory(GameItem item)`
  - Adds a game item to the player's Inventory list and notifies the Weapons attribute of change.
- `public void RemoveItemFromInventory(GameItem item)`
  - Removes a game item from the player's Inventory list and notifies the Weapons attribute of change.
- `public bool HasAllTheseItems(List<ItemQuantity> items)`
  - Checks whether the player has all the items needed for a quest in his Inventory list.
