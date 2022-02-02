## Humans-VS-Goblins  🥷🏿 ⚔️ 👺

### About
> Can you defeat the land of the goblins? 

Project assignment for Pyramid Academy(GenSpark).

Task: Build a class-based RPG in the commandline.

### Features

### Install (MacOS)
0. Install Java Tools
````bash
brew install openjdk
brew install gradle
brew install groovy
brew install jenkins
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

Project Tools Information
|   Tool   |  Version  |     Purpose     | Install | Documentation |
| :------: | :-------: | :-------------: | :-----: | :-----------: |
| IntelliJ | Community | Code Editor     | [Install](https://www.jetbrains.com/idea/download/#section=mac) | [Resources](https://www.jetbrains.com/idea/resources/) |
| Java     | 17        | Language        | [Downloads](https://www.oracle.com/java/technologies/downloads/) | [Docs](https://docs.oracle.com/en/java/javase/17/) |
| Homebrew | 1.16.1    | Package Manager | [Install](https://brew.sh/) | [Docs](https://docs.brew.sh/) |
| Gradle   | 7.3.3     | Build Platform  | [Install](https://gradle.org/install/) | [Docs](https://groovy-lang.org/documentation.html) |
| Groovy   | 4.0.0     | Build Script DSL| [Install](https://groovy-lang.org/install.html) | [Docs](https://docs.gradle.org/current/userguide/userguide.html) |
| Jenkins  | openjdk@11| CI/CD           | [Install](https://www.jenkins.io/doc/book/installing/) | [Docs](https://www.jenkins.io/doc/) |

Project Dependencies
|  Tool  | Version |  Purpose  | Documentation |
| :----: | :-----: | :-------: | :-----------: |
| JUnit  |    5    | Testing   | [Docs](https://junit.org/junit5/docs/current/user-guide/)|

### Testing
Jenkins Scripts (app)
> Default runs on http://localhost:8080 | http://127.0.0.1:8080/
```bash
brew services start jenkins
brew services stop jenkins
brew services restart jenkins
brew upgrade jenkins
```

## Project Planning

#### Project Specifications
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

#### Project Task
- [X] Create GitHub Repository
- [X] Choose Maven or Gradle
- [X] Create .gitignore
- [ ] Add Badges
   - [ ] Version
   - [ ] Coverage
   - [ ] Build
   - [ ] License
- [X] Project Specifications
- [ ] Add Dependencies to README dependency chart
- [ ] Docker
  - Documentation
    - [ ] Add Instructions to README
  - Installation
    - [ ] Install Docker Hub locally and create online account
  - Docker-Compose
    - [X] Create docker-compose.yaml
    - [X] Add "app" module to docker-compose.yaml
  - Dockerfiles
    - [X] "app" module
      - [X] Create Dockerfile
      - [X] Build Docker Image
      - [X] Push Docker Image to DockerHub
      - [X] Add com.palantir plugin dependencies to build.gradle
- CI/CD
  - [X] Add Jenkins
- [ ] Add Redis as Cache Memory Store
- [ ] Add Elastic Stack for logging

#### Programming Task
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


#### References
- [CodingConcepts](https://codingnconcepts.com/spring-boot/deployment-of-microservices-using-docker-and-jenkins/)

#### License: [MIT](https://choosealicense.com/licenses/mit/)
