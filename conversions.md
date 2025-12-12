# Binary Conversion Guides

[< Back to Basics](basics.md) | [Next: Real World Apps >](applications.md)

This section provides step-by-step instructions for converting numbers between human-readable formats and machine formats.

## 1. Binary to Decimal
To convert a binary number to decimal, you add up the "place values" of the ones.

**The Powers of 2 Cheat Sheet:**
* $2^0 = 1$
* $2^1 = 2$
* $2^2 = 4$
* $2^3 = 8$
* $2^4 = 16$
* $2^5 = 32$
* $2^6 = 64$
* $2^7 = 128$

### Example: Convert `1011` to Decimal
1. Write the powers of two above the digits, starting from the right:
    ```text
    8   4   2   1   (Place Values)
    1   0   1   1   (Binary Number)
    ```
2. Ignore the positions with `0`.
3. Add the values where there is a `1`:
    * $8 + 2 + 1 = 11$
4. **Result:** 1011 in binary is **11** in decimal.

## 2. Decimal to Binary
To convert decimal to binary, we use the **subtraction method**. We try to subtract the largest power of 2 possible from our number until we reach 0.

### Example: Convert `25` to Binary
1. Find the largest power of 2 less than or equal to 25. That is **16**.
    * Place a `1` in the 16 column.
    * Remainder: $25 - 16 = 9$.
2. Check the next power down (8). Can 8 fit into 9? **Yes**.
    * Place a `1` in the 8 column.
    * Remainder: $9 - 8 = 1$.
3. Check the next power down (4). Can 4 fit into 1? **No**.
    * Place a `0` in the 4 column.
4. Check the next power down (2). Can 2 fit into 1? **No**.
    * Place a `0` in the 2 column.
5. Check the next power down (1). Can 1 fit into 1? **Yes**.
    * Place a `1` in the 1 column.
    * Remainder: $1 - 1 = 0$ (Done).

**Result:** `11001`

---
[Go to Real World Applications >](applications.md)