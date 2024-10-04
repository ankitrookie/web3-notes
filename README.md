# All encoding algo that is used for converting binary into readable format.
1. ASCII
2. Hexadecimal(HEX)
3. Base64
4. Base58

# Hashing algo that convert our data into string & characters.
1. SHA-256 - used by SOL
2. keccak-256 - used by eth
3. MD5 - insecure due to vulnerabilities

# Encryption algo that converts our data into ciphertext.
Two types of encryptions :
1. Symmentric - same key is used for encryption & decryption. <br />
   algo are : <br />
         1. AES <br />
         2. DES
3. Asymmetric Encryption - uses key pairs for encryption and decryption. <br />
   algo are : <br />
        1. RSA (Rivest–Shamir–Adleman) <br />
        2. ECC (Elliptic Curve Cryptography) - Used by ETH and BTC <br />
           -Common elliptic curve algo are : <br />
               1. secp256k1: Used in Bitcoin (BTC) and Ethereum (ETH). <br />
               2. ed25519: Used in Solana (SOL). 
        3. EdDSA (Edwards-curve Digital Signature Algorithm) - Used by SOL

# some node js libraries for creating EdDSA - Edwards-curve Digital Signature Algorithm  - ED25519
1. @noble/edd5519
2. @solanaweb3.js

# Some libraries for creating ECDSA (Elliptic Curve Digital Signature Algorithm) - secp256k1
1. @noble/secp256k1
2. ethers - for ethereum wallets / cryptographic function

# HD
Hierarchical Deterministic Wallet” — generates addresses by taking the phrase and combining it with a piece of information called a derivation path. Together, they create any number of accounts, using Complex Math™ aka cryptography.

# RPC (Remote procedure call) communication protocol
We can also call procedure a (function) coz we are calling remote function through this protocol.

# Batch Request (this is universal topic not only in web3)

A batch request is a  mechianism in which multiple HTTP requests are combined into a single rquest. But we have to make sure that APi supports batch processing.

## private keys are used of transaction and signing messages.

## Links
https://sreeks.notion.site/Web3-Week3-cce0a7aee0a54348abd3d7b8ded1aef4

# Accounts on solana.
Accounts on solana are the data structure(scheam, just for my own undrstanding) for storing datas. We refer this data as Accounts. And it can also store verious type of data not only program/smart contract datas.
And it also stores fixed state, where we can eventually manipulate through smart contracts/programs. And program are special type of data storage structure in solan that contains executable codes.

## Cold start problems / this problem are miner problem initially when you create you own blockchain, there will be no miners. So this is refer as cold start problem.

## Command to interact with solana cli.
#### To check in which network env I am currently in.
```bash
solana config get
```
#### To change network env
```bash
solana config set --url https://api.devnet.solana.com
solana config set --url https://api.testnet.solana.com
solana config set --url https://your-rpc-node.com:8899
```
