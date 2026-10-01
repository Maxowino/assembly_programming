# Addition

# add1.asm

The program adds: 120 + 10 = 130 

# Flags

* **CF = 0 (Cleared)** : There is no carry because 130 can fit inside an 8-bit unsigned value.

* **OF = 1 (Set)** : Both numbers are positive, but 130 is bigger than the maximum positive signed 8-bit value, which is 127. This causes signed overflow.

* **SF = 1 (Set)** : The result is 130, which is `10000010` in binary. The most significant bit is 1, so SF is set.

* **ZF = 0 (Cleared)** : The result is 130, not zero.

* **PF = 1 (Set)** : The result has an even number of 1 bits, so the parity flag is set.

* **AF = 1 (Set)** : There is a carry from the lower 4 bits during the addition.

# add2.asm
The program adds: 32000 + 500 = 32500 

# Flags

* **CF = 0 (Cleared)** : 32500 fits inside the 16-bit unsigned range, so there is no carry outside the 16 bits.

* **OF = 0 (Cleared)** : 32500 is still within the maximum positive signed 16-bit value of 32767, so there is no signed overflow.

* **SF = 0 (Cleared)** : The result is positive, so the most significant bit is 0.

* **ZF = 0 (Cleared)** : The result is not zero.

* **PF = 0 (Cleared)** : The lowest byte of the result has an odd number of 1s.

* **AF = 0 (Cleared)** : There is no carry from the lower 4 bits.
