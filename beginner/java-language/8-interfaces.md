# Interfaces

- contracts without implementation
- if your class implements the interface, then you have to implement the methods
- your class can still have other functionality and implement other interfaces
- ex: if your class implements `java.lang.Comparable` has to implement `compareTo`
  - then `Arrays.sort(yourArrayOfComparableObjs)` can sort your array
  - in `compareTo`, return negative if `this` is before, 0 if same order, and positive if after
    - sometimes you can just do a subtraction and return the result
- classes can only extend another class, but can implement
- if a class implements an interface, then you can do `Interface inst = new ClassName()`
  - meaning, you can use polymorphism with the interface
- interfaces can:
  - specify method names
  - specify constants (treated as public, final, static)
  - extend from another inteface
    - classes implementing your interface will have to implement the child interfaces
- GOAL: make it easy to add classes that implement the interface and take advantage of polymorphism
- GOAL:
  - take a problem and model it in term of its pieces
  - model the contract to fulfill those pieces as an interface
  - build implementations of the interface to focus on units of work
  - good because incremental work eaech time
- KEY: Gets rid of if statements
