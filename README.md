# Python ZOOP Lab

In this lab, you will be building a simulation of a virtual zoo using object-oriented programming (OOP) principles in Python. The goal of this lab is to practice defining base and derived classes, using constructors, and method overriding.

## Getting Started

* fork and clone this repo, cd into the new folder
* use `zoo.py` to complete the assignment

## Instructions

### Base `Animal` Class

Create a base `Animal` class that has the following properties:

* name
* species
* age
* gender

Add the following methods:

* `describe` -- prints out all information about the animal
* `feed` -- prints out `"< animal name > is eating"`
* `make_sound` -- prints out `"< animal name > is making a sound"`
* `move` -- prints out `"< animal name > is moving"`

### Extending the Base `Animal` Class

Create the following child class that derive from the base `Animal` class, adding properties and
using method override when needed:

* `Mammal` -- has a `fur_color` property that is printed out it's description
	* drinks milk when feeding
	* walks when moving
	* growls when making a sound

Create a `Zoo` class with an `animals` property that is a list of all of the animals in the zoo. 

### Creating a `Zoo` Class

The `Zoo` class should have the following methods:

* `add_animal` -- adds an animal to the list 
* `display_animals` -- displays information for all animals
* `feed_animals` -- feeds all animals
* `listen_to_animals` -- listens to all the animals
* `watch_animals` -- watches the animals more around

### Bonus

Create additional child classes to populate your zoo!

* `Bird` -- has a `wingspan` property that is printed out it's description
	* drinks nectar when feeding
	* flies when moving
	* chirps when making a sound
* `Reptile` -- has a `scale_color` property that is printed out it's description
	* eats insects when feeding
	* slithers when moving
	* hisses when making a sound

### Example Code

Example code:

```python
zoo = Zoo()

lion = Mammal("Simba", "Lion", 5, "male", "golden")
snake = Reptile("Kaa", "Snake", 4, "female", "green")

lion.make_sound()
# > Simba is making a sound
# > Simba is growling

zoo.add_animal(lion)
zoo.add_animal(snake)
zoo.feed_animals()
# > Simba is eating
# > Simba is drinking milk
# > Kaa is eating
# > Kaa is eating insects
```

Write similar code chunks to test your zoo and the various
animals you create.

