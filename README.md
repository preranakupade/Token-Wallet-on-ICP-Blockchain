# Token-Wallet-on-ICP-Blockchain

This project is a Rust-based token wallet implemented on the Internet Computer Protocol (ICP) blockchain. The wallet supports functionalities such as sending and receiving tokens, checking balances, and ensuring basic wallet security.


**Features**

Mint Tokens: Add tokens to a wallet for testing purposes.
Transfer Tokens: Send tokens from one wallet to another.
Check Balance: Display the balance of a specified wallet.


**Prerequisites**

1. DFINITY SDK:
   
Install the DFINITY SDK by following the official installation guide.

2. Rust Programming Language:
   
Install Rust from rust-lang.org.

3. Clone the Repository:
   
git clone <repository-url>
cd <repository-folder>



Setup Instructions

1. Initialize the Project:
   
Run the following commands:
dfx new icp_wallet_project
cd icp_wallet_project

2. Add Rust Code:
   
Copy the provided Rust code into the src folder of the project.
Update the dfx.json file to include the Rust canister configuration.

3. Build and Deploy the Canister:
dfx deploy


**Usage Instructions**

1. Mint Tokens:

Use the mint function to add tokens to a wallet:
dfx canister call icp_wallet mint '("<wallet_address>", <amount>)'

2. Transfer Tokens:

Transfer tokens from one wallet to another:
dfx canister call icp_wallet transfer '("<from_address>", "<to_address>", <amount>)'

3. Check Balance:

Check the balance of a specific wallet:
dfx canister call icp_wallet balance_of '("<wallet_address>")'


**Testing**

1. Run Unit Tests:

Run the Rust unit tests to validate the functionality:
cargo test

2. Manual Testing:

Use the ICP local testnet to manually invoke canister functions.


**Troubleshooting**

If the deployment fails, verify your Rust and DFINITY SDK installation.
Use the dfx help command for troubleshooting common issues.

