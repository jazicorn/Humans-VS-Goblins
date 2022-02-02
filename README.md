## Humans-VS-Goblins

### About
Project assignment for Pyramid Academy(GenSpark).

- System: MacOS

#### Project run
0. Install Java Tools
````bash
brew install openjdk
brew install gradle
brew install groovy
````
1. Clone Repository
```bash
https://github.com/jazicorn/Humans-VS-Goblins.git
```
2. Build Project
```bash
./gradlew build
```
3. Run Project
```bash
./gradlew run
```
Project Tools Information [macOS]
|   Tool   |  Version  |     Purpose     | Documentation |
| :------: | :-------: | :-------------: | :-----------: |
| IntelliJ | Community | Code Editor     | [Install](https://www.jetbrains.com/idea/download/#section=mac) |
| Java     | 17        | Language        | [Docs](https://docs.oracle.com/en/java/javase/17/) |
| Homebrew | 1.16.1    | Package Manager | [Install](https://brew.sh/) |
| Gradle   | 7.3.3     | Build Platform  | [Docs](https://groovy-lang.org/documentation.html) |
| Groovy   | 4.0.0     | Build Script DSL| [Docs](https://docs.gradle.org/current/userguide/userguide.html) |

Project Dependencies
|  Tool  | Version |  Purpose  | Documentation |
| :----: | :-----: | :-------: | :-----------: |
| JUnit  |    5    | Testing   | [Docs](https://junit.org/junit5/docs/current/user-guide/) |

## Project Planning

#### Project Set-up
- [X] Create GitHub Repository
- [X] Choose Maven or Gradle
- [X] Create .gitignore
- [X] Project Specifications
- [X] Built Docker Image for app

##### Project Specifications
1. Everything must be objects: land/goblins/humans
2. You must override the toString method to represent each of the object
3. Create a grid for the game world
4. Use UTF characters for the players and goblins and the land
5. Game is turn based move: n/s/e/w
6. Once a human and goblin collide combat is initiated
7. Combat uses math.random
8. Extras:
    1. human has inventory system
    2. goblins have drops
    3. stats can be modified by equipment
    4. map gen random treasure chest after each round of combat
    5. goblins pursue player
9. Unit Testing

##### Project Steps
- [ ] Create Objects
- [ ] Object: Land
- [ ] Object: Goblin
- [ ] Object: Human
- [ ] Create Grid
- [ ] Create UTF Characters
- [ ] UTF: Players
- [ ] UTF: Goblins
- [ ] UTF Land
- [ ] Create Turn Based Moves: n/s/e/w
- [ ] Create Initiate Combat

#### License: [MIT](https://choosealicense.com/licenses/mit/)