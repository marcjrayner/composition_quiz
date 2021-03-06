# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?
It means an object can take many forms.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.
It means we can, for example, have an ArrayList of a particular class of objects, and we could add
various different class objects to the array. We can treat them all as being the same class.

From the wizard / fly example:

public IFly getRide(){
      return this.ride;
  }

The ride in this case could be one of three totally different classes. But since
all of the classes implement IFly, they can all be passed into a function which
accepts IFly as its required type.


3. What can we use to implement polymorphism in Java?

- We can use interfaces - we can have many different classes which, if they all implement
a given interface, can be treated as instances of that interface, even though the objects
may have totally different functionality from one another.
- We can also use Abstract classes - if multiple different classes are all children of
the same parent, we can treat them as instances of the parent (which can never actually
be instantiated itself)


4. How many 'forms' can an object take when using polymorphism?
As many as you want in your program. There's no limit

5. Give an example of when you could use polymorphism.
Morty Smith is a Morty. In a different universe Morty is Evil Morty, and there is also a Cronenburg Morty. Thus we can look at Morty in many ways:
    * Morty from the original dimension
    * Evil Morty
    * Cronenburg Morty
    * Fascist Morty
    * Morty Smith (C-132)

Each Morty is a Morty from a multiverse of near infinite different Morty's, each has different characteristics
as every possibile outcome has played out in the multiverse. Each different Morty class can be treated as though it were of type Morty (the parent or interface used to provide the common functionality across all child Morty's)


# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?
Composition means having instances small classes each doing their own particular specific job, then having
instances of larger more complex classes being composed of or built up of these smaller objects

7. When would you use composition? Provide a simple example in Java.
A car might be composed of an Engine, Wheels, Chassis and other components, each component would
be of its particular class with specific methods, the larger car object fits the pieces together, directing
them to do all their jobs together, which allows the car to drive.

8. What is/are the advantage(s) of using composition?
We can avoid the potential tangled mess of using too much inheritance of too many
behaviours. We can simply say an object -has a- other object which does that behaviour.
That way, we can share more specific relevant behaviours we need.

9. When an object is destroyed, what happens to all the objects it is composed of?
Java perfoms automatic garbage collection - any unreferenced objects are erased from memory.
