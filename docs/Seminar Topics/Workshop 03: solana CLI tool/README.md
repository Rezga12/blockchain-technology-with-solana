Workshop 02.5: solana CLI tools

solana cli the workshop will be dedicated to working with solana cli tool. it's the main entrypoint 
for developers new to solana.

we will only cover rudimentary things with this CLI tool:
* generating keypairs
* connecting to different clusters using `solana config` command
* airdropping SOL using `solana airdrop` command (explaining why it doesn't work :D)
* getting addresses and balances for accounts
  * explaining how public-private keypair is stored as 64 byte array
* transfering sol using `solana transfer` command
* fetching transaction statuses with `confirm` command
* fetching account data with `solana account` command
* using different keypairs for different instructions, using `-k` option
* 