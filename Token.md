## Tokens / Token Mint(Mint Account)
Token is a digital assets createed/deployed on a blockchain.

The folks at USDC, UDDT, Tether haven't created their own blockchain, and 
created their Token. They simpley create on the top of the existing blockchain like solana
eth.

#### The way we create Tokens on SOl and ETh are totelly different :
SOL :: In solana we dont't write our own smart contract to create toekns, we just derive from already writeen/deployed
smart contract by solana folks. We just create an account on top of the contract.

ETH: But the the case of ETH, if we have to create Token we have to create our own smart contract ourselfs and deploy it
in the blockchain.

For more instence : If in future i want to create my own token called AnkitCoin, so what will i do. Call a function on 
the solana smart contract. So that will create new account for me.

This exact thing creating account is called minting account(Mint Account).

More jargon :: In solana each token mint account has a fised size of 82 bytes. Coz every mint is same and storing same thing right so that why it is constant accross the mint.

The Decimals we see while creating Token in solan which is 9. It is same as lamports in solana the smallest unite of 
solana is lamport => 1000000000. So 1 Token => 9

## fungible and nonfungible token
Fungable tokens are those assets that are devisable(one that can broken down into smaller unites without losing their value)
Indian rupee :: notes such as 100 INR is fungible. you can change one with other coz they hold same value.

Nonfungible tokens are unique and non-devisable.
Art Works :: Traditional Indian art pieces, paintings by renowned artiest.

That is what non-fungible token are, unique digital assets that cannot be divided. Something that cannot be devided down further.

## Associated Token Account
associated  token is a account of User account created from Mint account. Where user has their own token of that mint.
For like real life ex: RBI is a Mint account and Assocaited token account is a Bank account that every coutumer has.
And when user have 0 SOL in account the account colse automatically.
And for every token like : doggy, Dogy, USDC, USDT, I have each bank account. 
Statment would be something like this : whos bank account you want to open, and in what currency do you want to open bank account on.(doggy coint, USDC etc)

If we create our own token and want to send it to someone, first we have to create account for them which happens 
automatically, then put it there. And to little clerify it creates account for that specific Token, for lets say i want to send my own token called ankitCoin
to some one and they dont have account(ankitCoin token account) whele we dont have to create it saperately, while if we send to wallet address it will create that token
account automatically.
