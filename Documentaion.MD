### Block class ###

#### Properties #### 

 - `index`: Integer value representing the position of the block in the chain.
 - `timestamp`: Date and time the block was created.
 - `data`: Data stored in the block. Can be any type of object.
 - `previous_hash`: Hash of the previous block in the chain.
 - `hash`: Hash of the current block.

### Methods ###

 - `calc_hash()`: Calculates the SHA-256 hash of the block using the index, timestamp, data and previous_hash properties.

#### Blockchain class ####

### Properties ###

 - `chain`: List of Block objects representing the current state of the blockchain.

### Methods ###

 - `create_genesis_block()`: Creates and returns the first block in the blockchain, also known as the genesis block.
 - `get_latest_block()`: Returns the last block in the chain property.
 - `add_block(new_block)`: Adds a new block to the blockchain. The previous_hash property of the new block is set to the hash of the current latest block, and the hash of the new block is recalculated using the calc_hash method.

*Please note that this is a very basic implementation and is missing many important features such as consensus, security and scalability. It is not recommended to use this for any production use cases.*
