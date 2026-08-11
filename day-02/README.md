# Day 2 of Solana

## What I Learned

I learned how to generate a Solana wallet programmatically and then check its balance using the devnet RPC.  
I discovered that while I could create a wallet with just a few lines of code, persistence was key — otherwise, each run would generate a brand-new wallet.  
I also learned how to connect to the Solana devnet and query balances directly from my script.

## What I Did

- I created a new script called `wallet-balance.mjs`.
- I imported `createSolanaRpc` and `devnet` from `@solana/kit`.
- I connected to the devnet RPC and used my wallet’s public key to check its balance.
- I ran the script and confirmed that my wallet had the SOL I previously airdropped from the faucet.
- I experimented by running the script multiple times and noticed that without saving the keypair, I kept generating new wallets with zero balance.
- I understood that persistence (saving the wallet to a file) would be necessary to maintain continuity, which will be covered in the next challenge.

## Reflection

I realized that programmatic wallet creation is powerful but ephemeral if not persisted.  
This exercise helped me appreciate the importance of secure storage for private keys and the convenience of querying balances directly from code.  
It also reinforced the idea that devnet SOL is purely for testing, so I could experiment freely without risk.
