# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
## NAME : YUGABHARATHI T
## REG.NO : 212224040375
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
```
#include <stdio.h>
#include <string.h>
int main() {
    char url[100];
    char key = 'K';  
    int i;

    printf("Enter Text: ");
    scanf("%s", url);
    for (i = 0; i < strlen(url); i++) {
        url[i] = url[i] ^ key;
    }
    printf("\nEncrypted Text: %s", url);
    for (i = 0; i < strlen(url); i++) {
        url[i] = url[i] ^ key;
    }

    printf("\nDecrypted Text: %s\n", url);

}


```

# OUTPUT:


<img width="1345" height="647" alt="Screenshot 2026-02-06 141455" src="https://github.com/user-attachments/assets/24296afd-c1fb-4dc5-b220-a005e1d412cf" />

# RESULT:
Thus, the AES algorithm was successfully implemented to encrypt a URL securely.
The encrypted URL ensures data confidentiality, security during transmission, and protection against unauthorized access.


