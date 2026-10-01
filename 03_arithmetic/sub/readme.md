# Subtraction

## sub1.asm
The program subtracts: 50 - 80 = -30

# Flags
* **CF = 1 (Set)** : 50 is smaller than 80, so a borrow is needed to perform the subtraction.

* **OF = 0 (Cleared)** :The result is -30, which can be represented in an 8-bit signed value, so there is no signed overflow.

* **SF = 1 (Set)** : The result is negative, so the most significant bit is 1.

* **ZF = 0 (Cleared)** : The result is -30, not zero.

* **PF = 1 (Set)** : The result has an even number of 1 bits, so the parity flag is set.

* **AF = 0 (Cleared)** : There is no borrow from the lower 4 bits.

# sub2.asm
The program subtracts: 1000 - 2000 = -1000

### Flags

* **CF = 1 (Set)** : 1000 is smaller than 2000, so a borrow is needed.
* **OF = 0 (Cleared)** : -1000 is within the signed 16-bit range, so there is no signed overflow.
* **SF = 1 (Set)** :  The result is negative, so the most significant bit is 1.
* **ZF = 0 (Cleared)** : The result is not zero.
* **PF = 1 (Set)** : The lowest byte of the result contains an even number of 1 bits.
* **AF = 0 (Cleared)** : There is no borrow from the lower 4 bits.

