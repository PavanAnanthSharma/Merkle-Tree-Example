# Merkle-Tree-Example
This has the basic solidity code, where you can verify and test Merkle proof with Merkle Tree and root hash, yes and i understand it sounds confusing but after you get an indea trust me its super eazy.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Understanding what Merkle Tree or Hash Tree: 

In cryptography and computer science, a hash tree or Merkle tree is a tree in which every leaf node is labelled with the cryptographic hash of a data block, and every non-leaf node is labelled with the cryptographic hash of the labels of its child nodes. Hash trees allow efficient and secure verification of the contents of large data structures. Hash trees are a generalization of hash lists and hash chains.
Demonstrating that a leaf node is a part of a given binary hash tree requires computing a number of hashes proportional to the logarithm of the number of leaf nodes of the tree; this contrasts with hash lists, where the number is proportional to the number of leaf nodes itself. Merkle trees are therefore an efficient example of a cryptographic commitment scheme, in which the root of the Merkle tree is seen as a commitment and leaf nodes may be revealed and proven to be part of the original commitment.
More can be found here: https://en.wikipedia.org/wiki/Merkle_tree

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

What is Merkle Hash or Root hash:

A Merkle root is the hash of all the hashes of all the transactions that are part of a block in a blockchain network. A  blockchain is comprised of various blocks that are linked with one another (hence the name blockchain). A hash tree, or the Merkle tree, encodes the blockchain data in an efficient and secure manner. It enables the quick verification of blockchain data, as well as quick movement of large amounts of data from one computer node to the other on the peer-to-peer blockchain network.
Every transaction occurring on the blockchain network has a hash associated with it. However, these hashes are not stored in a sequential order on the block, rather in the form of a tree-like structure such that each hash is linked to its parent following a parent-child tree-like relation.
Since there are numerous transactions stored on a particular block, all the transaction hashes in the block are also hashed, which results in a Merkle root.
For example, consider a seven-transaction block. At the lowest level (called the leaf-level), there will be four transaction hashes. At the level one above the leaf-level, there will be two transaction hashes, each of which will connect to two hashes that are below them at the leaf level. At the top (level two), there will be the last transaction hash called the root, and it will connect to the two hashes below it (at level one).
Effectively, you get an upside-down binary tree, with each node of the tree connecting to only two nodes below it (hence the name "binary tree"). It has one root hash at the top, which connects to two hashes at level one, each of which again connects to the two hashes at level three (leaf-level), and the structure continues depending upon the number of transaction hashes.
More can be found here: https://www.investopedia.com/terms/m/merkle-root-cryptocurrency.asp


> What is Merkle Proof:


Merkle proofs are established by hashing a hash's corresponding hash together and climbing up the tree until you obtain the root hash which is or can be publicly known. Given that one way hashes are intended to be collision free and deterministic algorithms, no two plaintext hashes can/should be the same.

Merkle proofs are used to decide upon the following factors:
1. If the data belongs in the merkle tree
2. To concisely prove the validity of data being part of a dataset without storing the whole data set
3. To ensure the validity of a certain data set being inclusive in a larger data set without revealing either the complete data set or its subset.
More can be found here: https://computersciencewiki.org/index.php/Merkle_proof


