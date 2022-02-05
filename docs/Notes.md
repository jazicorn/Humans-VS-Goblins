## Notes
> Notepad for planning my code

### Character Creation
Character race? character job?

character stats:
- hp
- mp
- attack
- attack defense
- magic
- magic defense
- experience points
- character name
- character title(job)

- roles add points to base stats of character
Interface roles:
- warrior
- wizard
- assassin
- cleric

Class: Villager extends NPC

Class: Bandit extends NPC

Class: All

- Interface: Character
- Class: Player
- Class: NPC
- Cl

module: class-system


#### Order-Of-Operations
1. Create Player & NPC Objects
    - Class File: Character
        - Common Attributes
            - HP
            - Attack
            - Defense
    - Class: Goblin extends Character
        - Extra: Drops
    - Class: Human extends Character
        - Extra: Equipment
        - Extra: Items
    - Interface: Player
    - Interface: NPC
2. Create Land Objects
    - ClassFile: Land
        - Common Attributes
            - Size
            - Goblin NPC's
            - Extra: Random Treasure
            - Extra: Landmarks
                - landmarks take up space that npc's & players can't land on
    - Class: Dungeon
    - Class: Beach
    - Class: Ocean
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
