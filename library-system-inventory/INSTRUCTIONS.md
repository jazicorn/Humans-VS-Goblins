## Instructions

### Building
```gradle
build.gradle

// create custom version or jar file
version = '0.1.0'

// customize jar file
jar {
    manifest {
        attributes('Implementation-Title': project.name,
                   'Implementation-Version': project.version)
    }
}
```
```gradle
// creates jar in build folder
./gradlew build

// add custom version to jar file
./gradlew jar
```

### Refs
- [TutorialPoint: Building Java Libraries](https://medium.com/@tutorialspointexamples/building-java-libraries-6038d715af39)