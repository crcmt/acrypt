*acrypt*
========

*acrypt* stands for 'Asymetric enCRYPTion'.

*acrypt* is a tool to encrypt password
using asymmetric key encryption scheme.

It aims to solve the following scenario:  
  1. Bob created an account for User Alice.
  2. Bob wants to send the account's password to Alice by email.

Technically, *acrypt* is a wrapper around openssl.

### Basic usage

  1. Bob and Alice install *acrypt*

        git clone https://github.com/crcmt/acrypt

  2. Alice generates keys pair

        ./acrypt generate

  3. Alice sends her public key to Bob by email.
  4. Bob encrypts the account's password with Alice's public key.

        ./acrypt encrypt public.key plaintext.txt

  5. Bob sends the encrypted password to Alice by email.
  6. Alice decrypts the encrypted password with her private key.

        ./acrypt decrypt private.key encrypted.dat

  7. Alice removes her private key.

        rm private.key

  8. Alice now knows the password and can connect to her account.
