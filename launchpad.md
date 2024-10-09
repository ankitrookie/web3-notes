## How does Solana launch pad work, with the library in React. Understanding it.

Creating launch pad in browser/application is different then creating token from 
cli/local mechine. Coz we want other people to mint the token, it is fully 
dynamic, anyone can come and create thir token from the application.

when I was creating token. creating with js for my self. I had the access to my own 
private key. But when we make application dynamic such that everyone can come and create
their own token. I need to do something to create token coz I don't have access to their
pricate key. phantom, backpack won't share their private key. But they can sign a transaction
tho, that is what we are descussing next :

We need to read through createMint function/api that @solana/spl-token library provides.
Below is under the hood code of createMint function :
```js
export async function createMint(
    connection: Connection,
    payer: Signer,
    mintAuthority: PublicKey,
    freezeAuthority: PublicKey | null,
    decimals: number,
    keypair = Keypair.generate(),
    confirmOptions?: ConfirmOptions,
    programId = TOKEN_PROGRAM_ID
): Promise<PublicKey> {
    // below function is rent for the data that i want to store in account.
    const lamports = await getMinimumBalanceForRentExemptMint(connection);

    const transaction = new Transaction().add(
        SystemProgram.createAccount({
            fromPubkey: payer.publicKey,
            newAccountPubkey: keypair.publicKey,
            space: MINT_SIZE,
            lamports,
            programId, // who own this account
        }),
        createInitializeMint2Instruction(keypair.publicKey, decimals, mintAuthority, freezeAuthority, programId)
    );

    await sendAndConfirmTransaction(connection, transaction, [payer, keypair], confirmOptions);

    return keypair.publicKey;
}
```
