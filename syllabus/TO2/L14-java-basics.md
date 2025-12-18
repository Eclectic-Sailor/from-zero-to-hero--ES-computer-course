# L14: Java Basics (EO3)
**Objectives:** Classes/objects, collections, exceptions; build/run with Maven or Gradle.

## Resources
- Read: Oracle Java Tutorials (Getting Started; Classes/Objects; Collections): https://docs.oracle.com/javase/tutorial/
- Setup: JDK 17+ download: https://adoptium.net/temurin/releases/
- Maven quickstart: https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html
- Gradle getting started: https://docs.gradle.org/current/samples/sample_building_java_applications.html

## Tasks
- Create a small CLI app:
  - Define a `User` class with fields and methods.
  - Use `ArrayList` and `HashMap` to store users and look them up.
  - Handle bad input with try/catch.
- Build and run with `mvn package` or `gradle run`.

## Example Code to Analyze
```java
try {
    int x = Integer.parseInt("abc");
} catch (NumberFormatException e) {
    System.out.println("Bad number");
}
```
What happens and why?

## Knowledge Check
- Difference between interface and class?
- How does Java handle memory vs C (GC vs manual)?
- Checked vs unchecked exceptions basics.

## Exit Criteria
- `java -jar` (or `gradle run`) works for your CLI.
- You can explain why collections need generics (type safety).
