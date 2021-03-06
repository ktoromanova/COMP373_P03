# Project 3 for COMP  373: Implementing Patterns I 

## Bridge Pattern

Without the Bridge Pattern, our initial solution looked like that:

![alt text](https://github.com/ktoromanova/COMP373_P03/blob/master/img/wo_bridge.jpg)

The problem with this solution was that if we later wanted to change the Carrot class, then we may ended up changing the PlantCarrot and HarvestCarrot as well and then we may need to change the Potato class as well. 

We used the Bridge pattern to solve the above problem by decoupling the Vegetable and Farm interfaces as shown below:

![alt text](https://github.com/ktoromanova/COMP373_P03/blob/master/img/w_bridge.jpg)

Thus, we achieved decoupling the abstraction from its implementation so that the two can vary independently.

## Observer Pattern

For the implementation of Observer Pattern we created a Subject, Observer and Client(Main) class. The Subject have methods attach and detach observers to the client object, so that the observable is now an object which notifies observers about the changes in its state.

In conclusion, the we added the Observer pattern to define a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.
