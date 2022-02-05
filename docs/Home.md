## Humans-VS-Goblins | 🥷🏿 ⚔️ 👺

### About
> Can you defeat the land of the goblins? 

*Project for Pyramid Academy(GenSpark)*

**Assignment:** Build a class-based RPG in the commandline.

### Documents
to use docsify:
```bash
# add global install of docisify
yarn global add docsify-cli 

# initialize docs folder with docsify files
docsify init ./docs
```
```bash
# command to display readme's in browser
docsify serve ./docs

# results
Serving /Users/jasmineanderson/Genspark/Projects/Humans-VS-Goblins/docs now.
Listening at http://localhost:3000
```

<!-- ### Features -->

### Install (MacOS)
0. Install Programs
   * Java 
   * Gradle
   * Groovy
   * Jenkins


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

### Project Information
[Technology](docs/Technology.md)

## Project Planning

### Project Specifications
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
    6. Keep track of player score
    7. create a scoreboard for top players
9. Unit Testing

### Programming List
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

#### [Detailed List](docs/Details.md)

#### [References](docs/References.md)

#### License: [MIT](https://choosealicense.com/licenses/mit/)
