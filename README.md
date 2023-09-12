*acrypt*
========

*acrypt* stands for 'Asymetric enCRYPTion'.

*acrypt* is a tool to encrypt a password
using an asymmetric key encryption scheme.

It aims to solve the following scenario:  
  1. Admin Bob created an account for User Alice.
  2. Bob wants to send the account's password to Alice by email.

Basic Usage:

  * Bob and Alice install *acrypt*

        git clone https://github.com/crcmt/acrypt

  * Alice generates keys pair

        ./acrypt gen

  * Alice sends pubkey to Bob by email.
  * Bob encrypts the account's password with Alice's pubkey

        ./acrypt enc

  * Bob sends the encrypted passwd to Alice by email.
  * Alice decrypts the encrypted passwd

        ./acrypt dec

  * Alice now knows the password and can connect to her account.
  * Done !
