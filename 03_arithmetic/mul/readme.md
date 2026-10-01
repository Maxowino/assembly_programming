# Multiplication
# mul1.asm
 25 × 10 = 250

# Flags
* **CF =(0) Cleared** — The result fits within 8 bits.
* **OF =(0)Cleared** — The result fits within the original 8-bit size.
* **SF = (0)Cleared** — The result is positive.
* **ZF =(0) Cleared** — The result is not zero.
* **PF = (0)Cleared** — The result has an odd number of 1 bits.
* **AF =(0) Cleared** — There is no carry from the lower 4 bits.

# mul2.asm
3000 × 200 = 600000

# Flags
* **CF =(1) Set** — The result is too large to fit in 16 bits.
* **OF =(1) Set** — The result is larger than the 16-bit range.
* **SF =(0) Set** — The result has its most significant bit set.
* **ZF =(0) Cleared** — The result is not zero.
* **PF =(0) Cleared** — The result has an odd number of 1 bits.
* **AF =(0) Set** — A carry occurs from the lower 4 bits.
