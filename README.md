*acrypt*
========

*acrypt* stands for 'Asymetric enCRYPTion'.

*acrypt* is a tool to encrypt a password
using an asymmetric key encryption scheme.

It aims to solve the following scenario:
Admin A created an account for User U.
Now A wants to send the account's password to U by email.

Steps:
A asks U to generate priv/pub keys pair with *acrypt*.
A asks U to sent the pub key to him by email.
A encrypts the passwd with the pub key with *acrypt*.
A sends the encrypted passwd to U by email.
U decrypts the encrypted passwd with *acrypt*.
U now know the password and can connect to his account.
U removes his priv/pub keys pair (one-time keys pair).
Done !

Current implementation is based on openssl.

dependencies
------------

bash
openssl

installation
------------

    git clone https://github.com/crcmt/acrypt

Usage
-----

    cd acrypt
    ./acrypt
