# RANDOM NUMBER GENERATOR (RNG) IN STRUCTURED TEXT (ST)

Don't forget to create the TAGS!

## LINEAR CONGRUENTIAL GENERATOR

```text
// Generate is a BOOL tag
// temp is a DINT tag
// seed is a DINT tag
// randomNumber is an INT tag
//FALSE is a BOOL tag
 
// NEW RANDOM NUMBER GENERATOR
// Assume "Generate" is a BOOL tag that controls when to generate a new random number
IF Generate THEN
    // Linear Congruential Generator (LCG) parameters
    temp := (1664525 * seed + 1013904223);
    temp := temp MOD 2147483647; // 2^31 = 2147483647
    seed := temp;                // Update the seed value
    randomNumber := temp MOD 10; // Scale the result to range 0-9
    // Reset Generate flag to prevent continuous generation
    Generate := FALSE;
END_IF;
```

***

## DUAL NUMBER GENERATOR
> _Submitted by D. Cartwright, Fall '24_

```text
// Edited Random Structured Text
// Generate is a BOOL tag
// temp is a DINT tag
// seed is a DINT tag
// randomNumber1 & 2 is an INT tag

// NEW RANDOM NUMBER GENERATOR
//2x outputs, and absolute values so no negatives, can easily add more outputs


//Program will autostart when jumped
Generate := 1;

IF Generate THEN
// Linear Congruential Generator (LCG) parameters
temp := (1664525 * seed + 1013904223);
temp := temp MOD 2147483647; // 2^31 - 1 = 2147483647
seed := temp; // Update the seed value

// Generate first random number (1-686)
randomNumber1 := ABS((temp MOD 686) + 1);

// Generate second random number (1-418)
// We'll use a different modulus operation to ensure independence
temp := (1664525 * temp + 1013904223);
temp := temp MOD 2147483647;
randomNumber2 := ABS((temp MOD 418) + 1);

// Reset Generate flag to prevent continuous generation
Generate := 0;
END_IF;
```
## RANDOM INSULT GENERATOR

>_Submitted by P. Liberty, Spring '26_

```
// Free-running seed
Seed := Seed + 1;

IF Seed > 10000 THEN
    Seed := 1;
END_IF;

// Rising edge detect
IF Trigger AND NOT Trigger_Last THEN

    // Random roll 1-10
    Seed := (Seed * 37) + 11;

    IF Seed > 10000 THEN
        Seed := Seed MOD 10000;
    END_IF;

    IF Seed = 0 THEN
        Seed := 1;
    END_IF;

    Roll := (Seed MOD 10);

    // Pick insult
    CASE Roll OF
        1: ChiefInsult := 'Chief, that idea needed more maintenance than the machine.';
        2: ChiefInsult := 'Chief, I have seen sharper thinking from a dead battery.';
        3: ChiefInsult := 'Chief, that was a premium-grade bad call.';
        4: ChiefInsult := 'Chief, you are operating at full confidence and half accuracy.';
        5: ChiefInsult := 'Chief, that plan belongs in the scrap bin.';
        6: ChiefInsult := 'Chief, I respect the effort, not the result.';
        7: ChiefInsult := 'Chief, that was bold, unnecessary, and incorrect.';
        8: ChiefInsult := 'Chief, even the PLC looked disappointed.';
        9: ChiefInsult := 'Chief, that move had all the grace of a dropped wrench.';
        10: ChiefInsult := 'Chief, you are making mistakes with impressive consistency.';
    ELSE
        ChiefInsult := 'Chief, something went wrong.';
    END_CASE;

END_IF;

// Save trigger state
Trigger_Last := Trigger;
```

>_PS: The Chief is never wrong. LOL!_
