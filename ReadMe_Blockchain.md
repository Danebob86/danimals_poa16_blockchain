# Week 18 - Proof of Authority Development Chain

![blockchain](https://static.bangkokpost.com/media/content/20210430/c1_2108411_210430122446.jpg)

## Background
I have just landed a new job at ZBank, a small, innovative bank that is interested in exploring what blockchain technology can do for them and their customers. My first project at the company is to set up a private testnet that our team of developers can use to explore potentials for blockchain at ZBank.

ZBank has decided on setting up a testnet because:
* There is no real money involved, which will give your team of developers the freedom to experiment.
* Testnets allows for offline development.


# Running poa16 Blockchain

endpoint = http://127.0.0.1:8545

chainid = 16

pswd = 1216

Run the following code in seperate Git Bash terminals to initiate blockchain.  
## Node1
./geth --datadir node1 --unlock "a0f5f5df49C0bb9596d4Bb5610A733FB5c7A410B" --mine --rpc --allow-insecure-unlock3

## Node2
./geth --datadir node2 --unlock "a0f5f5df49C0bb9596d4Bb5610A733FB5c7A410B" --mine --port 30304 --bootnodes "enode://6bab79d8f6581e21f7f1a47d8443baf11430cf106603557256fb845e37567aa332726b10c542b69aa7bce3aaf02e30d065876d2f50da6025ef325c819bdf1c8b@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock


# Making a Test Transaction
1. Connect to customm Node RPC via my crypto. You will need to use endpoint and chainid listed above. 
* See custom_7_setup_custom_node_MyCrytpo screen shot as example.
2. Select public address you would like to send test transaction to and pick amount. 
* See 8_send_ETH_test_transaction screen shot as example. 
3. Confirm transaction is sucessfull via recent transactions on MyCrypto. 
* See 8_send_ETH_test_transaction screen shot as example. 
4. Check Git Bash terimnal that is running node/blockchain to double check blockchain recored sucessfull transaction. 
* See 10_blockchain_showing_transaction_success screen shot as example. 

# Reference Documents
Please refrence the following documents/folders in the GitHub repo for further instructions and clarification. 
* poa_structure_blockchain
* poa16
* screen_shots
