#  Data Modeling & NoSQL

### Name 3 advantages to Test Driven Development 

1. Writing the tests first requires you to really consider what do you want from the code.
2. You receive fast feedback.
3. TDD creates a detailed specification.
4. TDD reduces time spent on rework.
5. You spend less time in the debugger.
6. You are able to identify the errors and problems quickly.
7. TDD tells you whether your last change (or refactoring) broke previously working code.
8. TDD allows the design to evolve and adapt to your changing understanding of the problem.
9. TDD forces the radical simplification of the code. You will only write code in response to the requirements of the tests.
10. You're forced to write small classes focused on one thing.

### In what case would you need to use beforeEach() or afterEach() in a test suite?

```javascript
 beforeEach(browser) {
    // > this will get run before every test case <
  }
```

```javascript
afterEach(browser) {
    // > this will get run after every test case <
  }
```

### What is one downside of Test Driven Development?

- It necessitates a lot of time and effort up front, which can make development feel slow to begin with.
- Focusing on the simplest design now and not thinking ahead can mean major refactoring requirements.
- It’s difficult to write good tests that cover the essentials and avoid the superfluous.
- It takes time and effort to maintain the test suite – it must be reconfigured for maximum value.
- If the design is changing rapidly, you’ll need to keep changing your tests. You could end up wasting a lot of time writing tests for features that are quickly dropped.

### What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.

### Name a use case for a static method

Usually, static methods are used to implement functions that belong to the class, but not to any particular object of it.

### Write an example of a Higher Order function and describe the use case it solves

Higher-order functions are functions that take other functions as arguments or return functions as their results.

For example, the map function on arrays is a higher order function. The map function takes a function as an argument.

```javascript
[1, 2, 3, 4].map(function(n){
    return n * 2
}) // [ 2, 4, 6, 8 ]
```

## Document the following Vocabulary Terms:

- **functional programming:**  is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects.

- **pure function:** is a function where the return value is only determined by its input values, without observable side effects. 

- **higher-order function:**  Higher-order functions are functions that take other functions as arguments or return functions as their results.

- **immutable state:** immutable object (unchangeable object) is an object whose state cannot be modified after it is created.

- **object:** n object is a collection of properties, and a property is an association between a name (or key) and a value. A property's value can be a function, in which case the property is known as a method.

- **object-oriented programming (OOP):** he basic idea of OOP is that we use objects to model real world things that we want to represent inside our programs, and/or provide a simple way to access functionality that would otherwise be hard or impossible to make use of.

- **class:** Classes are a template for creating objects. They encapsulate data with code to work on that data.

- **prototype:** Prototypes are the mechanism by which JavaScript objects inherit features from one another.

- **super:** The super keyword is used to access and call functions on an object's parent. The super.

- **constructor:** Inheritance is an important concept in object oriented programming. In the classical inheritance, methods from base class get copied into derived class.

- **instance:** An “instance” means a reference to an “object” created by “new” or the equivalent.

- **Context:** - Refers to the object within a function being executed.

- **this:** Within a constructor, refers to the object that will be created when the constructor is run. 

- **Test Driven Development (TDD):** Programming practice which involves developing tests for every small functionality of an 
application. It instructs developers to write new code only if an automated test has failed. This avoids duplication of code.

- **Jest:** Javascript testing framework with a focus on simplicity.

- **Continuous Integration (CI):**  A coding philosophy and set of practices that drive development teams to implement small changes as a mechanism to integrate and validate changes. 

- **Unit Test:**  Software testing method where individual units of source doe are tested to determine whether they are fit for use. 