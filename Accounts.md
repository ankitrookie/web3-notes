## How rent works in SOL
"Rent proportional" means the amount you need to pay (in SOL) for storing data on the blockchain increases based on how much data you have. More data requires more payment to maintain your account.

## Owners in Accounts.
My account that I crated is owned by another program called System Program. what is system program check System-Token-program.md file.
And even System Program has owner, which we called Native Loder | BPF loder. So every account you have in sol has an owner.

And each account is identified by its unique address which is 32 bytes in the format of an ed25519(elliptic curve algo) as publick key.

I must I minium balance in the account either i have data or not coz we have this fields like owner, executable, etc. 
run below command on solana cli how much min sol, you must have  if you have to have and account :
```bash
rent 0 
```
