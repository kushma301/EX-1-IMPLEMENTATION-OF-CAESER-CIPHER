## Name: S.Kushma
## Reg no: 212224040168

## Exp:1 IMPLEMENTATION OF CAESER CIPHER 

## AIM: 
To encrypt and decrypt the given message by using Caeser Cipher encryption algorithm. 
  
 ## ALGORITHM: 
1. Calculate the length of the plaintext. 
2. For each character in the plaintext:  
 a. Add the key to the character to get the cipher character.  
 b. If the result exceeds 'Z' for uppercase or 'z' for lowercase, subtract 26 to wrap within the  alphabet.  
3. Display the encrypted text.  
4. For decryption, subtract the key from each character of the ciphertext.  
 a. If the result is less than 'A' for uppercase or 'a' for lowercase, add 26 to wrap within the  alphabet.  
5. Display the decrypted text.  

## PROGRAM: 
```
#include <stdio.h>
#include <string.h>
void caesarCipher(char *name, int shift) 
{
    for (int i = 0; name[i]; i++) 
    {
        if (name[i] >= 'A' && name[i] <= 'Z')
        name[i] = ((name[i]- 'A' + value) % 26) + 'A';
        
    }
 }
int main() 
{
    char name[] = "KUSHMA";
    caesarCipher(name, 3);
    printf("Encrypted Message: %s\n", name);
    caesarCipher(name,-3);
    printf("Decrypted Message: %s\n", name);
    return 0;    
}
```
## OUTPUT: 
<img width="1689" height="1087" alt="Screenshot 2025-09-01 144858" src="https://github.com/user-attachments/assets/5c14ecc6-4e4a-4bb0-96ae-8652b80d1ede" />

## RESULT: 
The program implementing the Caesar cipher for encryption and decryption has been successfully  executed, and the results have been verified.
