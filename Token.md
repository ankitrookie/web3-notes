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
