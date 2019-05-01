## Construction Company Challenge

### Different Types of Buildings
1. Create four new classes to represent different types of buildings. They should all inherit from the building class. Give each derived class at least one property or method that's unique to that type of building. For example, if you make a class called `ApartmentBuilding`, give it a property called `numberOfApartments`.

1. Give your `Employee` class the ability to construct different buildings. It should write to the console a confirmation that the building is under construction. This method should have different behavior based on what type of building it recieves as an argument. For example, if you pass it an instance of the `ApartmentBuilding` class, it should write something to the console like "Now building {x} number of rooms in the apartment building!" (Hint: google method overloading).

### Maintenance Requests
1. Create a new class to represent a maintenance request. Maintenance requests should have:
        - A description of the problem to be fixed (string)
        - A property to tell us who filed the report
        - An `assignedEmployee` property of type `Employee`
        - A property that tells us which building the report was filed for
        - A property called `Completed` that holds a boolean

1. Create a new property on your  `Employee` class called `AssignedRequests`. This should be a list of type `Maintenance Requests`. 

1. Create a new class called `Supervisor` that inherits from `Employee`. A supervisor should be able to create a maintenance request and assign a maintenance request to an employee. When they assign a maintenance request, it should be added to that employee's list of assigned requests and alter the `assignedEmployee` property on the request itself.
1. Use Linq to figure out which employee has completed the most maintenance requests, and which one has completed the least.


### Adding rooms to a building
1. Add a method on the building class to add a room. This method should assign the `Building` property on the given room and add the given room to the building's list of rooms.
1. Add a property on your `Building` class called `totalArea`. This should give us the combined areas of all the rooms in that house. 
1. Add a property on your `Building` class called `getAverageRoomSize`. This should return the average area of all the rooms in the house.
1. Add a method on your `Building` class called `estimateCost`. It should accept a parameter of a price per square foot and return a total estimate based on the total area of the house. 
