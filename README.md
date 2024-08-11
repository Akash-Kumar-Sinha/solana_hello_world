# Hello world program on solana blockchain

**Reference:** (<https://solana.com/developers/guides/getstarted/local-rust-hello-world#what-you-will-learn>
  )

1. **Start the Local Validator**

   First, run your local Solana validator:

    ```bash
    solana-test-validator
    ```

2. After writing the code, build the program using:

    ```bash
    cargo build-sbf
    ```

3. Then deploy the program you need to have you solana validator running and the balance should not to be `0 sol`
   **To Deploy:**

    ```bash
    solana program deploy ./target/deploy/hello_world.so
    ```

    - If you have `0 sol` (you can check it by running ```solana balance```)
    - If your balalnce is `0 sol` then you can request for sol by writing `solana airdrop 1`. It will add 1 sol to you account.

4. After deploying you get a program id like

    ```bash
    Program Id: CVLmT78vDxndE98sjCDUSs5ohojcsWFGWD59fNauMUD
    ```

5. Now you have successfully deployed your sol program over the devnet (Everything is happening on devnet not on mainnet)

6. Then you just need to run `npm install` in your client folder and replace Program id with yours and then run
    - You can also run this```npm install @solana/web3.js @solana-developers/helpers```

    ```bash
    cd Client
    node client.mjs
    ```
