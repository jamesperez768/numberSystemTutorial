# Real-World Applications: Hex & Text

[< Back to Conversions](conversions.md) | [Return Home](README.md)

Now that you understand the math, we can look at how these systems are used in the real world.

## 1. The Hexadecimal Shortcut
Computer scientists rarely convert large binary numbers using math. Instead, they use **Hexadecimal** as a shortcut.

Because 1 Hex digit represents exactly 4 Binary digits (a nibble), you can split binary numbers into groups of 4 to convert them instantly.

### Binary to Hex (The Grouping Method)
**Task:** Convert `11011010` to Hex.

1. **Split** the binary into groups of 4 (start from the right):
   `1101`  |  `1010`
2. **Convert** each group to decimal:
   * `1101` = 8 + 4 + 1 = **13**
   * `1010` = 8 + 2 = **10**
3. **Map** to Hex digits:
   * 13 = **D**
   * 10 = **A**
4. **Result:** `DA` (Base-16)

## 2. Storing Text (ASCII)
Computers can only store numbers. To store text, they use a standard mapping system called **ASCII** (American Standard Code for Information Interchange).

Every letter on your keyboard has a specific number attached to it.

| Character | Decimal Value | Binary Value |
| :--- | :--- | :--- |
| **A** | 65 | 01000001 |
| **B** | 66 | 01000010 |
| **C** | 67 | 01000011 |
| ... | ... | ... |
| **a** | 97 | 01100001 |
| **b** | 98 | 01100010 |

### Why is 'a' different from 'A'?
Note that capital 'A' (65) and lowercase 'a' (97) are totally different numbers. This is why passwords are "case-sensitive." To a computer, `01000001` is not the same as `01100001`.

---
[Return to Home](README.md)