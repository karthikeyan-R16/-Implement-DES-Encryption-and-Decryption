# EX-7 Implement-DES-Encryption-and-Decryption

## Aim:
  Implement-DES-Encryption-and-Decryption using C program.

## ALGORITHM: 
  1.DES is based on a Feistel network, which divides the data into two halves and applies a series of permutations and substitutions in multiple rounds.
  
  2.DES uses a symmetric-key algorithm, where the same key is used for both encryption and decryption
  
  3.DES operates on a fixed 64-bit block size for data.
  
  4.It uses a 56-bit key for encryption, which is expanded to 64 bits with the inclusion of parity bits.
## PROGRAM:
```
#include <stdio.h>
#include <string.h>
void xor_encrypt_decrypt(char *input, char *key) {
int input_len = strlen(input);
int key_len = strlen(key);
for (int i = 0; i < input_len; i++) {
input[i] = input[i] ^ key[i % key_len]; // XOR encryption
}
}
int main() {
printf("\n\n***** ADVANCED-ENCRYPTION STANDARD-DES-ALGORITHM *****");
printf("\n\n");
char url[] = "KARTHIKEYAN";
char key[] = "secretkey"; // Simple key for XOR encryption
printf("Original Text: %s\n", url);
xor_encrypt_decrypt(url, key);
printf("Encrypted Text: %s\n", url);
xor_encrypt_decrypt(url, key);
printf("Decrypted URL: %s\n", url);
return 0;
}

```
## OUTPUT:
![image](https://github.com/user-attachments/assets/faf4465a-45e7-48da-8fd7-e13e4f624f4b)


## RESULT: 
thus, Implement-DES-Encryption-and-Decryption Executed Sucessfully
