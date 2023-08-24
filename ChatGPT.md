What is a class in JavaScript?

In JavaScript, a class is a blueprint for creating objects that share similar properties and behaviors. It defines the structure and behavior of the objects that will be instantiated from it. Classes provide a way to define object templates with reusable methods and properties.

JavaScript introduced a more formal class syntax in ECMAScript 6 (ES6) to make object-oriented programming more intuitive and organized. The class syntax provides a clearer and more familiar way to define classes and instantiate objects compared to the traditional prototype-based approach.

Here's a basic example of how you can define a class in JavaScript:
class Animal {
  constructor(name, species) {
    this.name = name;
    this.species = species;
  }

  makeSound() {
    console.log("Some generic animal sound");
  }
}

// Creating instances of the class
const dog = new Animal("Buddy", "Dog");
const cat = new Animal("Whiskers", "Cat");

console.log(dog.name);  // Output: Buddy
console.log(cat.species); // Output: Cat

dog.makeSound(); // Output: Some generic animal sound

In this example, the Animal class has a constructor method that initializes properties name and species when an object is created from it. The makeSound method is defined within the class and can be called on instances of the class.

It's important to note that even though JavaScript now has class syntax, it is still based on prototypes behind the scenes. The class syntax is essentially syntactic sugar over the prototype-based system, making it easier and more readable to work with objects and their behaviors in an object-oriented manner.