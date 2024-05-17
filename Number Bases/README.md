# Understanding Numeral Bases

## Introduction

In mathematics and computer science, a numeral system (or system of numeration) is a writing system for expressing numbers. It is a mathematical notation for representing numbers of a given set using digits or other symbols in a consistent manner. 
The base (or radix) of a numeral system is the number of unique digits, including zero, that a positional numeral system uses to represent numbers.

## Common Bases

### Base 10 (Decimal)
- **Digits:** 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
- **Usage:** This is the standard numeral system used in everyday life.
- **Example:** The number "254" in base 10 means:
  \[
  2X10^2 + 5 X 10^1 + 4X10^0 = 200 + 50 + 4 = 254
  \]

### Base 2 (Binary)
- **Digits:** 0, 1
- **Usage:** Widely used in computing and digital electronics because digital devices use binary logic.
- **Example:** The number "1011" in base 2 means:
  \[
  1X2^3 + 0X2^2 + 1X2^1 + 1X2^0 = 8 + 0 + 2 + 1 = 11 \text{ (in decimal)}
  \]

### Base 8 (Octal)
- **Digits:** 0, 1, 2, 3, 4, 5, 6, 7
- **Usage:** Sometimes used in computing, especially in older systems and for compact representation of binary numbers.
- **Example:** The number "745" in base 8 means:
  \[
  7X8^2 + 4 X8^1 + 5X8^0 = 448 + 32 + 5 = 485 \text{ (in decimal)}
  \]

### Base 16 (Hexadecimal)
- **Digits:** 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F (A-F represent 10-15)
- **Usage:** Commonly used in computing and digital electronics for a more human-readable representation of binary-coded values.
- **Example:** The number "1A3" in base 16 means:
  \[
  1X16^2 + 10X16^1 + 3X16^0 = 256 + 160 + 3 = 419 \text{ (in decimal)}
  \]

## Converting Between Bases

### To Decimal (Base 10)
To convert a number from another base to decimal, **multiply** each digit **by its base raised to the power of its position** (starting from 0 on the right) and sum the results.

- **Example:** Convert "1011" (base 2) to decimal:
  \[
  1X2^3 + 0X2^2 + 1X2^1 + 1X2^0 = 8 + 0 + 2 + 1 = 11
  \]

### From Decimal to Another Base
To convert from decimal to another base, repeatedly **divide** the decimal number by the new base, keeping track of the remainders. 
The remainders form the digits of the new base number, starting from the rightmost digit.

- **Example:** Convert 419 (decimal) to base 16:
 
1. Divide 419 by 16:
   - Result: 26
   - Remainder: 3 (rightmost digit)

2. Divide the result 26 by 16:
   - Result: 1
   - Remainder: 10 (A in hexadecimal)

3. Divide the result 1 by 16:
   - Result: 0
   - Remainder: 1 (most significant digit)

So, 419 in decimal is represented as:

419 (decimal) = 1A3 (hexadecimal)



## Why Use Different Bases?

- **Binary (Base 2):** Efficient for computers, as they operate using binary logic (0 and 1).
- **Octal (Base 8) and Hexadecimal (Base 16):** More compact representation of binary numbers, making it easier for humans to read and understand. Frequently used in programming and digital electronics.
- **Decimal (Base 10):** Intuitive and commonly used in everyday life for general purposes.

