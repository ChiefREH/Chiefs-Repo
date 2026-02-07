# Cannon Ball Wall Run
Create a GROUP PROJECT to simulate a volley (down the wall and back) using all PLC/HMI combos:
    • Properly configured MSG instructions OR 
    • Properly configured PRODUCED/CONSUMED tags. 
    • Properly configured Controller scope tags versus Local scope tags. 
    • All necessary logic, graphics and configurations. 

DESIGN NOTES:
    • The visuals for the HMIs in between Ship 1 and Ship 2 must differ greatly. 
        ◦ No blank screens, duplicate screens, or blank backgrounds. I am grading the design aesthetics, so be creative! 
    • The scenes for Ship 1 and Ship 2 must not be mirrors. Be creative! 
        ◦ I will allow for a space battle theme, because space pirates are cool. 

PARAMETERS:
    • Player 1 starts at Ship 1, and targets Ship 2. 
        ◦ Each ship must have a visible fire button for the Player. 
    • The cannon ball must pass through all the HMI screens between Ship 1 and Ship 2. 
        ◦ No less than six PLC/HMI combos can be used. The more the better! <<< We have ? people, therefore we will have ? PLC/HMI combos in play 
        ◦ For the sake of time, I will allow for a minor "teleport" effect of the cannon ball as it moves through each HMI screen (including the Ship HMIs) 
            ▪ The motion of the effect must be adjustable for optimum viewing 
                • Adjustments to the timing OR movement increment must be made via the HMI using a numerical input (or slider) on a user-defined Configuration Screen 
                • Reason: to make adjustments while the routine is running online 
    • When Ship 1 or Ship 2 is hit, it must be on fire until all "hits" are received and the ship "explodes" 
    • If no Player input is made at either Station, the entire simulation must reset after 60 seconds ("Ready Mode") 
    • Each Ship must have a visual "hit" counter wired externally 
        ◦ After 3 "hits" the targeted ship explodes for 10 seconds and then the entire simulation resets 
        ◦ Must include a Red-Yellow-Green "hit" indicator light at each Ship/Player station output module 
        ◦ 1 hit = Green; 2 hits = Yellow; 3 hits = Red 
        ◦ Serves as visual feedback for single player mode 
            ▪ Also helpful in troubleshooting from the other end of the lab 
    • Must include 1 Red light indicator to each HMI station when the cannon ball is on that screen 
        ◦ Serves as visual feedback for single player mode 
            ▪ Also helpful in troubleshooting from the other end of the lab 

OPERATIONS:
    • What happens if we fire a second volley before the first volley hits the target? 

GRADING:
    • I will grade EVERYONE based on the worst design within the project. 
    • This means you ALL need to work together to create something visually stunning. 
        ◦ I want George Lucas & Steven Spielberg to weep at its magnificence! 

Remember: if the project doesn't work, you don't get paid.