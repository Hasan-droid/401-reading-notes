## Data Modeling
### Review, Research, and Discussion

- Name 3 advantages to Test Driven Development
    - Better program design and higher code quality.
    - TDD reduces the time required for project development.
    - Code flexibility and easier maintenance.
- In what case would you need to use beforeEach() or afterEach() in a test suite?
    - when we need to automatically run before and after each tests, which 1. removes the explicit calls from the tests themselves, and 2. invites inexperienced users to share state between tests.
- What is one downside of Test Driven Development
    - Additional Complexity.
- What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
    - Objects inherit properties from other objects. In prototypal inheritance, instead of defining the structure through a class, you simply create an object. This object then gets reused by new objects . Instances are typically instantiated via factory functions or Object.
- Why REST?
    - REST is much easier than other approaches such as SOAP which keeps developers from having to reinvent the wheel as far as HTTP request operations go. SOAP also requires separate server and client programs. 
    - Since REST is based on standard HTTP operations, it uses verbs with specific meanings such as "get" or "delete" which avoids ambiguity. Resources are assigned individual URIs, adding flexibility.
    - With REST, information that is produced and consumed is separated from the technologies that facilitate production and consumption. As a result, REST performs well, is highly scalable, simple, and easy to modify and extend.


### Vocabulares List
- Continuous Integration (CI): stands for Continuous Integration, which is the practice of merging all developers’ working copies to a shared mainline several times a day.

- REST: is software architectural style that was created to guide the design and development of the architecture for the World Wide Web.

- functional programming: is a way of thinking about software construction by creating pure functions.

- object-oriented programming (OOP): is a computer programming model that organizes software design around data, or objects, rather than functions and logic.

- class: is a blueprint for creating objects.

- super: is the parent class of the derived one.

- Test Driven Development (TDD): a software development approach where we write the tests before the code.

- Jest: is a JavaScript testing framework maintained by Facebook for tests and such.

- Data Model: is an abstract model that organizes data description, data semantics, and consistency constraints of data. The data model emphasizes on what data is needed and how it should be organized instead of what operations will be performed on data.