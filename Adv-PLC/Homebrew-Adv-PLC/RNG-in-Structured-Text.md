# RANDOM NUMBER GENERATOR (RNG) IN STRUNCTURED TEXT (ST)

Don't forget to create the TAGS!

***

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

## D. Cartwright's Random Number Generator Code (ST)
> _Submitted by Devin Cartwright, Fall 2024_

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