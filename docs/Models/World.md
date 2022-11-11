# World.cs

## Class Diagram
![World](https://user-images.githubusercontent.com/115721045/201363084-f5b2463e-bdff-4114-b027-ed2dc0f08cd2.svg)

## Attributes Description
- `_locations`
  - A private READONLY list of locations that exist in the world.

## Methods Description
- `internal void AddLocation(int xCoordinate, int yCoordinate, string name, string description, string imageName)`
  - Creates a new location object, populates the location's attributes using the arguments, then adds the location to the list of locations. Use ` $"/Engine;component/Images/Locations/{imageName}";`.
- `public Location LocationAt(int xCoordinate, int yCoordinate)`
  - Returns location that exists at (xCoordinate, yCoordinate) from the list of locations, or null if not found.
