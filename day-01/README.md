# Day 1 of Solana

## What I Learned

I learned that on Solana, my identity is represented by a **keypair** (public and private keys).  
The public key acts as my wallet address, while the private key proves ownership and must be kept secret.  
I realized this is similar to SSH keys in Web2, but here it’s used to interact with a decentralized blockchain.

## What I Did

- I created a new project folder with `mkdir 100-days-of-solana && cd 100-days-of-solana`.
- I installed the dependency: `npm install @solana/kit`.
- I wrote a script (`create-wallet.mjs`) that generated a new wallet using `generateKeyPairSigner()`.
- Each time I ran the script, I got a fresh wallet address.
- I funded my wallet using the [Solana Faucet](https://faucet.solana.com) on **Devnet**.
- I verified the balance by connecting to the devnet RPC and checking my wallet.

## Reflection

I discovered that the wallet only exists in memory unless I save it, which means I lost the private key each time I reran the script.  
This taught me the importance of persistence and secure storage, which I’ll explore in the next challenge.  
I also saw how decentralized identity works without relying on a central server.
