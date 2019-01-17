# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?
The ability of an object of a specific class to:
  - Behave as an object of any classes higher up it's inheritance tree, including abstract Classes
  - Or behave as an object of any interface type which is implemented in the class
This allows objects from different classes to be grouped together (e.g. in an ArrayList or HashMap). Functions can the be used on the collective objects.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

Olympic Village Security Example

- Mammal super Class (abstract) + implements ISecurity(int idNumber)
  - Human Class (abstract)
    - Athlete Class (abstract)
      - Hurdler Class
      - Rower Class
  - Dog Class (abstract)
    - GuideDog Class

- Item super Class (abstract) + implements ISecurity(int idNumber)
  - Delivery Class
  - Javelin Class

All objects inheriting from the Mammal super Class, can be grouped together as mammals e.g. new ArrayList<Mammal> which instances of Hurdler, Rower and GuideDog classes can be added and e.g. looped through.

All objects of either the Mammal or Item superclasses implement the ISecurity interface, so they can be grouped as ISecurity objects e.g. new ArrayList<ISecurity> which instances of Hurdler, Rower, GuideDog, Delivery and Javelin classes can all be added to e.g. return all their security numbers.


3. What can we use to implement polymorphism in Java?
Inheritance or Interfaces

4. How many 'forms' can an object take when using polymorphism?
The object can only take on one form at any one time, but it can recast into another form later, so the furthest down the inheritance tree form is more obscured than destroyed.

5. Give an example of when you could use polymorphism.
See olympic village above



# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?
Composition is when an object is made up (composed) of other objects.

7. When would you use composition? Provide a simple example in Java.
Composition should be used when we want to use object types interchangeably within other objects.
- e.g A Computer object wants to output different data types to different data handling devices such as printers, speakers and monitors. This can be achieved by creating a data handling interface which is implemented int the Computer and all other component classes.

8. What is/are the advantage(s) of using composition?
Composition allows objects from distinct and separate class inheritance hierarchies to use the same functions within another object.

9. What happens to the behaviours when the object composed of them is destroyed?
When the composite object is destroyed, the behaviours and all the composing objects are also destroyed.
