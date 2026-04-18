# PROJECT: DUNGEON CRAWL

- **WHAT:** Simulate a dungeon crawl gaming experience using PLC and HMI lab equipment.
- **WHY:** To simulate a large scale, data management scenario common in modern manufacturing environments.



## GAME RULES

**Random Number Generators (RNG)**
- 1d20 for your Initiative and normal Actions. 
- 1d6 for your Damage rolls. 
    - Enemies have a fixed damage value. No RNG needed. 
    - You may automate your Damage roll RNG on a successful hit, so you don't have to click an additional damage button. 
    - You may **not** automate the player Attack rolls. If you did that, then YOU aren't really the game; the PLC is just playing with itself! 
- 2d20 take the highest result for Advantage. 
- 2d20 take the lowest result for Disadvantage. 
 
**Action Economy**
- Everyone gets ONE Action on their Turn 
- Roll 1d20 + relevant Stat + Bonus (if any) vs DC 
    - If your total is equal to or greater than the DC, you SUCCEED with the Action. 
    - If your total is less than the DC, you FAIL at the Action. 



## CHARACTER CREATION

Create an interface for Player Class selection based on the following three choices:

- Fighter 
- Rogue 
- Mage 

Use navigation and popup screens as needed



## CHARACTER STATS

Based on Player input, allocate the following data to each Class:

1. Character Name (needs a **$String** to enter your character name?) 
2. Class type selected
3. Physical stat (for attacks) 
4. Mental stat (for lock-picking/trap disarming) 
5. Mystical stat (for Spell casting) 
6. Hit Points (HP) 



### STAT REFERENCE TABLE

| **CHARACTER'S NAME**  | **CLASS** | **PHYSICAL** | **MENTAL** | **MYSTICAL** | **HP** |
| --------------------- | --------- | :----------: | :--------: | :----------: | :----: |
| _Requires user input_ | Fighter   |      3       |     1      |      0       |   6    |
| _Requires user input_ | Rogue     |      2       |     3      |      2       |   4    |
| _Requires user input_ | Mage      |      1       |     2      |      3       |   2    |


### CHARACTER SELECTION SCREEN EXAMPLE 1

![Dungeon Crawl](Assignments-Adv-PLC-Images/Dungeon-Crawl2.jpg)


### CHARACTER SELECTION SCREEN EXAMPLE 2

![Dungeon Crawl](Assignments-Adv-PLC-Images/Dungeon-Crawl4.jpg)


## CHARACTER INVENTORY

Based on Player input, allocate the following data to each Class:


**The Fighter**
- Sword stat (+2 bonus to attack, 1d6 dmg)

**The Rogue**
- Dagger stat (no attack bonus, 1d6 dmg) 
- Lock-Pick stat (Advantage on traps, locks and doors) 

**The Mage**
- Spell (fireball, no bonus to attack, 2d6 dmg) 



## MAP & MOVEMENT

- Navigate an interactive map (boundaries & collision mechanics)
- Character must be able to travel each square of the map.
    - **No teleportation!**

### DUNGEON TILE EXAMPLE

![Dungeon Tiles](Assignments-Adv-PLC-Images/Dungeon-Tiles.jpg)



## ENEMY LOGIC

Randomly Generated Creature (1-6) for Combat:
- Name/Type 
- Hit Points (HP) 
- Attack Damage (fixed value, no attack RNG) 

   
| **ROLL** | **ENEMY TYPE** | **HP** | **DMG** |
| :------: | :------------- | :----: | :-----: |
|    1     | AI ROBOT       |   10   |    2    |
|    2     | MUTANT BEAR    |   8    |    2    |
|    3     | MUTANT DOG     |   4    |    1    |
|    4     | MUTANT SNAKE   |   4    |    1    |
|    5     | MUTANT SPIDER  |   6    |    2    |
|    6     | MUTANT ZOMBIE  |   3    |    1    |



## COMBAT ENCOUNTER

When you land on a tile with an ENEMY creature:
 
**ROLL FOR INITIATIVE:**
- Roll 1d20 vs DC 12 (no stats, mods or bonuses)
    - Equal to or greater than the DC, the Character goes first. 
    - Less than the DC, the Enemy goes first! 
 
**Each side gets ONE Action:**
- Enemies will always ATTACK v. DC 15 (automated)
- Characters always have the option to leave on their turn.* 
- A normal Action in combat is 6 seconds in length. 
- This is good when automating the Enemy's turn, so the Player has time to see the Actions take place. 
 
**How are you going to defeat the enemy?**
- The FIGHTER will attack the enemy: Roll 1d20 + Physical stat + Bonus vs DC 15 
- The ROGUE will attack the enemy: Roll 1d20 + Mental stat vs DC 15 
- The MAGE will attack the enemy: Roll 1d20 + Mystical stat vs DC 15 

## ROLLED OUTCOMES

**ON A NORMAL ATTACK SUCCESS:**
- Roll for damage. Deduct damage from Enemy total HP.
- Continue with the encounter until one side is victorious. 

**ON A CRITICAL ATTACK SUCCESS (You roll a Natural 20):**
- Deal double damage. Deduct damage from Enemy total HP.
- Continue with the encounter until one side is victorious. 

**ON A CRITICAL ATTACK FAILURE (You roll a Natural 1):**
- You have dropped your weapon, dagger or burned out your spell.
- You have no options remaining except to flee the area and maybe return another day.* 

**ON A NORMAL DEFEND FAILURE:**
- Suffer damage from the Enemy. Deduct damage from your HP.
- Continue with the encounter until one side is victorious. 

**ON A CRITICAL DEFEND FAILURE (Enemy rolls a Natural 20):**
- Suffer double damage from the Enemy. Deduct damage from your HP.
- Continue with the encounter until one side is victorious. 

**ON A CRITICAL DEFEND SUCCESS (Enemy rolls a Natural 1):**
- The Enemy flees and you are safe to proceed.
 
## *DEV NOTE: 
You cannot proceed until an encounter is successfully completed. Have an option to exit the encounters, moving back the way you came. When you exit without a success, the encounter must be reset to start from the beginning, regardless of your initial progress. For a combat encounter, you must randomly generate a new creature.



## EXAMPLE HMI

![Dungeon Crawl](Assignments-Adv-PLC-Images/Dungeon-Crawl1.jpg)


![Dungeon Crawl](Assignments-Adv-PLC-Images/Dungeon-Crawl3.jpg)


![Dungeon Crawl](Assignments-Adv-PLC-Images/Dungeon-Crawl5.jpg)



## GAME EXAMPLES FOR INSPIRATION


Rogue-lite is a variation of the Rogue video game from the 1980's

https://en.wikipedia.org/wiki/Rogue_(video_game)
 
Rogue-like games:

https://en.wikipedia.org/wiki/Roguelike
 
EXAMPLES of computerized (grid-based, pseudo-3D) RPG Dungeon Crawler games from the 70s-90:

https://youtu.be/g8FJi2jwsmg?si=XFLPlW3TXH4ZjZJb

https://youtu.be/GQgHSX2tof4?si=WCkMzTZZxa68seTR


## FINAL PROJECT NOTES
A PDF copy of all .ACD files (with YOUR name) will be provided to the instructor for review. Failure to produce a copy **before the deadline** will result in an automatic 0 for the entire assignment. No exceptions.
 
And remember, Chief will **almost always** play the game as a MAGE…



_"IN GYGAX WE TRUST"_
