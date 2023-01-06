# Encryption tools

Here is a preliminary list of encryption tools. Please note that this is Very Much Work In Progress. Any suggestions for improvement are welcome.

- Bitlocker
- Veracrypt
- Boxcryptor
- GnuPG2
  - From https://research.csc.fi/best-practices-for-client-side-encryption: "GnuPG version 2 is likely the most widely used good free of charge and open source suite of software for encrypted messaging. GnuPG 2.2 is compliant with the OpenPGP RFC4880 and can utilise asymmetric encryption with public keys for easier key exchange and transport. Selecting option"—rfc4880" for maximum portability would select symmetric encryption algorithm to be 3DES which is not considered good enough anymore.  
  On command line the algorithm defaults can be seen with option "--verbose". Starting with version 2.1 the default for symmetric encryption is AES128, for older versions it is CAST5. On command line AES256 encryption is selected with options "--symmetric --cipher-algo AES256" which should be the symmetric algorithm to be used."
- openssl
  - From https://research.csc.fi/best-practices-for-client-side-encryption: "openssl is more a toolkit for encryption related needs than a standalone application. It is anyway easy to use tool for symmetric encryption.  
  AES256 encryption is selected with options "enc -aes-256-cbc". If you use password to generate the actual encryption key, then use only version 1.1.1 or later and with options "-pbkdf2 -iter 100000". These same options must also be used when decrypting the data.  
  Example run with openssl 1.1.1 where file data.dat is encrypted to data.enc:  
  `openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -in data.dat -out data.enc`  
  enter aes-256-cbc encryption password:  
  Verifying - enter aes-256-cbc encryption password:  
  If you choose to generate the actual random binary key and initialisation vector yourself then you can also use older versions than 1.1.1 of openssl."
- Cryptomator (in combination with Cyberduck)
  - From https://research.csc.fi/best-practices-for-client-side-encryption: "Cyberduck includes an open source tool called cryptomator for client-side encryption. Cyberduck's strong point is its multiplatform GUI interface, drawback is so far short history as cryptography tool, compared to GnuPG or openssl.  
  To make managing encryption easy for the end user, the Cryptomator treats a remote directory as if it were a single encrypted structure (a vault), but it actually encrypts each file for its own. In addition to the content of files, file and directory names are encrypted.


