# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
```
STEP 1:
Start the program and import the required libraries.
STEP 2:
Seed the random number generator using the current time(i.e) rand(time(0));
STEP 3:
Get the number of randon number to generate.
STEP 4:
Pass the value for number of iterations and print the numbers.
STEP 5:
End the program.
```
# PROGRAM:
```
NAME: LOGA MITHRA R
REGISTER NUMBER: 212223100027

#include <stdio.h>

#define A 1664525
#define C 1013904223
#define M 4294967296 // 2^32

unsigned int lcg(unsigned int seed) {
    return (A * seed + C) % M;
}

int main() {
    unsigned int seed;
    int n;

    printf("Enter the seed value: ");
    scanf("%u", &seed);
    printf("Enter how many random numbers to generate: ");
    scanf("%d", &n);
    printf("Random numbers:\n");

    for (int i = 0; i < n; i++) {
        seed = lcg(seed);
        printf("%u\n", seed);
    }

    return 0;
}
```

# OUTPUT:

![image](https://github.com/user-attachments/assets/b1f2409f-8d4f-430f-a1e4-65f549a777e9)

# RESULT:
The program has been run successfully
