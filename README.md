# Java Learning


## Best Practices
- Use **has-a** (Composition) and **is-a** (Inheritance of another) relationships carefully to as **has-a** offers more flexibility.
- Use OOPS principles such as 
  - Abstraction (Data Hiding): Abstract Classes, Abstract Methods
  - Inheritance: Single Level, Multi Level, Heirarchical, and Hybrid
  - Encapsulation: Protecting the code and data (state) of a single class from outside of the class using private, protected and setters/getter methods.
  - Compile-time Polymorphism: Method overloading, resolved at Compile time
  - Runtime Polymorphism: Method Overriding, determined only runtime
  - Aggregation Assocation: Weak association to allow objects to exist independently
  - Composition Assocation: Strong assocation (Part of Whole: Part cannot exist without a whole).  When a School object (Whole) is destroyed the associated Rooms (part) will automatically be destoryed.
- Use primitives over Wrapper classes to avoid the performance issues while Autoboxing/Unboxing and in NullPointerExceptions.
- Initialize the Collection objects with empty size rather than Null to avoid the NullPointerException. Does not cause any performance issues.
- Initialize the variables with default values to avoid NullPointerException
- Use Null check techniques (instanceof, Objects.rqeueireNonNull(obj), Optional.ofNullable(obj) and Optional.isPresent(), @NonNull, @Nullable annotations, CollectionUtils.isEmpty())
- Try with Resources: Practice to close the Resources automatically, even in exceptions scenarios, when are no longer used/referenced.
- Must log every Exception with Error, Bubble the Exceptions to caller by **throws** at method signature, or _rethrow_ it from the _Catch_ block.
- Use Collections with Generics (diamon instead of raw/traditional collections
- Use **final** keyword when a variable, Method, Method parameters, or Class requires immutability. Also implement Clone where it is needed to add the immutability.
- Use _@Override_ _@SuppressWarnings_ carefully and when needed
- Override the default **equals()** and **hashCode()** methods in the custom Class to avoid the unexpected behavior when used to compare the instances in hash based Collections.
- Use **StringBuilder** for String concatenation/modification cases to prevent memory allocations by JVM and performance degredation.
- Use **Constants** in a Final class or **Enum**s for readability and Type safety.
- Design a every project to use custome Log Appender to mask the sensitive data from the log output, configure in _application.properties_ or _application.yml_ files
- Employ to use _Code Coverage_ (**SonarLint**) tools and fix the recommendations from the early development of project






