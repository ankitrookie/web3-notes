# All encoding algo that is used for converting binary into readable format.
1. ASCII
2. Hexadecimal(HEX)
3. Base64
4. Base58

# Hashing algo that convert our data into string & characters.
1. SHA-256 - used by SOL
2. MD5 - insecure due to vulnerabilities

# Encryption algo that converts our data into ciphertext.
Two types of encryptions :
1. Symmentric - same key is used for encryption & decryption.
   algo are :
         1. AES
         2. DES
3. Asymmetric Encryption - uses key pairs for encryption and decryption.
   algo are :
        1. RSA (Rivest–Shamir–Adleman)
        2. ECC (Elliptic Curve Cryptography) - Used by ETH and BTC
           -Common elliptic curve :
               1. secp256k1: Used in Bitcoin (BTC) and Ethereum (ETH).
               2. ed25519: Used in Solana (SOL). 
        3. EdDSA (Edwards-curve Digital Signature Algorithm) - Used by SOL

# some node js libraries for creating EdDSA - Edwards-curve Digital Signature Algorithm  - ED25519
1. @noble/edd5519
2. @solanaweb3.js

# Some libraries for creating ECDSA (Elliptic Curve Digital Signature Algorithm) - secp256k1
1. @noble/secp256k1
2. ethers - for ethereum wallets / cryptographic function
