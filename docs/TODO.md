## TODO

#### TODO 2/3/21
- 1. Order of Operations
- In Progress Items
- Some Assignments??? 

#### Questions for instructor
- Does the map suppose to have a set size?
- Does the game suppose to have a goal other than fighting goblins?

#### Order-Of-Operations
1. Create Player & NPC Objects
   - Interface
     - Common Attributes
       - HP
       - Attack
       - Defense
   - Class File: Goblins
     - Extra: Drops
   - Class File: Humans
     - Extra: Equipment
     - Extra: Items
2. Create Land Objects
   - Interface
     - Common Attributes
       - Size
       - Goblin NPC's
       - Extra: Random Treasure
       - Extra: Landmarks
         - landmarks take up space that npc's & players can't land on
   - Class File: Dungeon
   - Class File: Beach
   - Class File: Ocean
3. Avatars (UTF characters)
    - Player
    - Goblin
    - treasure chest
    - cave entrance
    - cave exit
4. Land Map
    - Cave Entrance
    - move avatar n/s/e/w
    - Cave Exit
5. Encounter
  - Turn Based Combat
    - Point System
    - Combat uses math.random
  - Extra: Pursuit
    - Goblin pursues player

#### Extras:
1. Player Accounts
   - Player Name
   - Player Chooses Avatar
2. Inventory System
   - Redis Bloom
     - in databases: quickly checking if an entry exists in a table before accessing it on disk, and so on.
   - Redis JSON
     - Store Data
3. Leader Board
   - Player Rankings

##

### TODO

- Jenkins: Create Microservices Pipeline [Microservices](References.md#Microservices)
  - Research if maybe using GitHub webhooks better for Jenkins use?

- app Module: Change name to server Module
  - Rename DockerHub registered image
  - update Jenkins

- Design: Inventory System
- Design: Item Catalog
  - Player Armor
    - Helmet
    - Breastplate
    - Pants
    - Boots
    - Sword
    - Shield
  - Potions
  - Buffs
  - De-Buffs

- Class Goblins: Drop Rate
- Class Goblins: Follow Player

- Gameplay: Event Stream
  - Player/NPC Random Map Conflict
  
### In Progress

- GitHub: Add Hangman to academy repo
- GitHub: Add Humans-VS-Goblins to academy repo

### Done

...