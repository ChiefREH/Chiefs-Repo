# CANNON BALL WALL RUN
- Create a GROUP PROJECT to simulate a volley (down the wall and back) using all PLC/HMI combos:
    - Properly configured MSG instructions or PRODUCED/CONSUMED tags
    - Properly configured Controller scope tags versus Local scope tags
    - All necessary logic, graphics and configurations

### Video Demonstration

[![Watch on YouTube](https://img.youtube.com/vi/dJFL-XpIf0o/0.jpg)](https://youtu.be/dJFL-XpIf0o)

## DESIGN NOTES:
- The visuals for the HMIs in between Ship 1 and Ship 2 must differ greatly. 
    - _No blank screens, duplicate screens, or blank backgrounds._
- The scenes for Ship 1 and Ship 2 must not be mirrors. Be creative! 
    -  _I will allow for a space battle theme, because space pirates are cool._

## PARAMETERS:
- Player 1 starts at Ship 1, and targets Ship 2. 
    - Each ship must have a visible fire button for the Player. 
- The projectile must pass through all the HMI screens between Ship 1 and Ship 2. 
    - _The more the better!_
- For the sake of time, I will allow for a minor "teleport" effect of the projectile as it moves through each HMI screen (including the Ship HMIs) 
    - The motion of the effect must be adjustable for optimum viewing 
    - Adjustments to the projectile timing/movement must be made via the HMI
        - Can be a user-defined Screen or Pop-up Screen
        - _Reason: To make adjustments while the routine is running online_
- When Ship 1 or Ship 2 is hit, it must be on fire for 10 seconds, then explode for 10 seconds 
- After exploding, the Ship must reset, ready to return fire!
- Must include 1 visual light wired to each PLC/HMI station when the projectile is active on that screen 
    - _Serves as visual feedback for single player mode_
    - _Also helpful in troubleshooting from the other end of the lab_

## OPERATIONS:
- _What happens if we fire a second volley before the first volley hits the target?_

## GRADING:
- _I will grade EVERYONE based on the WORST design within the project._
- _This means you need to work together to create something visually stunning._
    - _I want George Lucas & Steven Spielberg to weep at its magnificence!_

### Remember:
- _If the project doesn't work, you don't get paid._