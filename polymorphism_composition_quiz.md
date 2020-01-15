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
a given interface, can be treated as instances of that interface, even though the objects
may have totally different functionality from one another.
- We can also use Abstract classes - if multiple different classes are all children of
the same parent, we can treat them as instances of the parent (which can never actually
be instantiated itself)

4. How many 'forms' can an object take when using polymorphism?

5. Give an example of when you could use polymorphism.

# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

7. When would you use composition? Provide a simple example in Java.

8. What is/are the advantage(s) of using composition?

9. When an object is destroyed, what happens to all the objects it is composed of?
