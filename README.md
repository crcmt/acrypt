*acrypt*
========

*acrypt* stands for 'Asymetric enCRYPTion'.

*acrypt* is a tool to encrypt a password
using an asymmetric key encryption scheme.

It aims to solve the following scenario:  
  1. Admin Bob created an account for User Alice.
  2. Bob wants to send the account's password to Alice by email.

Steps:
  * Alice generates keys pair with *acrypt*.

        ./acrypt gen

  * Alice sends the pub key to Bob by email.
  * Bob encrypts the account's password with the pub key with *acrypt*.

        ./acrypt enc

  * Bob sends the encrypted passwd to Alice by email.
  * Alice decrypts the encrypted passwd with *acrypt*.

        ./acrypt dec

  * Alice now knows the password and can connect to her account.
  * Done !

installation
------------

    git clone https://github.com/crcmt/acrypt

Usage
-----

    cd acrypt
    ./acrypt
