# Blockchain-in-Python

This repository contains a basic implementation of a blockchain in Python. This implementation is intended for educational purposes only and is not suitable for production use.

The code includes a Block class, which represents a single block in the blockchain, and a Blockchain class, which is used to manage the chain of blocks. The Block class includes a method for calculating the SHA-256 hash of the block, which is used to ensure the integrity of the block. The Blockchain class includes methods for creating the genesis block, getting the latest block, and adding new blocks to the chain.

### User Manual: ###

 1. Make sure you have Python installed on your machine. You can download it from the official website if you don't have it already.
 2. Clone the repository containing the blockchain script to your local machine using the command git clone https://github.com/<username>/<repository-name>
 3. Open a terminal or command prompt and navigate to the directory where you cloned the repository.
 4. Run the script using the command python blockchain.py or python3 blockchain.py depending on your system.
 5. The script will output the current chain of blocks, which should only contain the genesis block at this point.
 6. You can now add new blocks to the blockchain by creating new Block objects and passing them to the add_block method of the Blockchain object. For example:

```
bc = Blockchain()
bc.add_block(Block(1, "01/02/2020", { "amount": 4 }))
bc.add_block(Block(2, "01/03/2020", { "amount": 8 }))

```
 7. To check the latest chain after adding blocks you can print the chain like this:

```
print(bc.chain)
```

*Please note that this is a very basic implementation and is missing many important features such as consensus, security and scalability. It is not recommended to use this for any production use cases.*
