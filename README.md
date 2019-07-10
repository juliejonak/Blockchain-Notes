# Blockchain-Notes

[Lecture I](#Lecture-I)


<br>
<br>

[Lecture II](#Lecture-II)

<br>
<br>

## Pre-Class Resources

[The Trust Machine: The History of Bitcoin](https://youtu.be/ZKwqNgG-Sv4) 

[2 Part Blockchain Demo & Explanation](https://anders.com/blockchain/)  
[Quick Read: Blockchain Explained Simply](https://gardenofcrypto.com/blog/blockchain-explained-simply)  

[Blockchain Project Repo](https://github.com/LambdaSchool/Blockchain)  



# Lecture I

![Centralization and Ledgers](./ledgers_centralization.jpg "Centralization and Ledgers")


<br>
<br>

## Bitcoin

Who is Satoshi Nakamoto?

Nobody knows!

While we don't know individually who or what Satoshi Nakamoto really is, it is the name used by the unknown person or persons who developed bitcoin, authored the bitcoin white paper, and created and deployed bitcoin's original reference implementation. As part of the implementation, they also devised the first blockchain database.  

<br>

Bitcoin is a cryptocurrency that allows us to prove that currency has not been double spent, created in 2008.  

Satoshi currently holds (supposedly) 1 million Bitcoin. As of July 10, 2019, the value of a single Bitcoin is roughly $12,300.  

We took the pieces apart of hashing and building hash tables to understand how they work. Hash tables were invented in the 1950's, so while it's an old computer science data structure, it's continually being used in new and unique ways that fundamentally shift how we use computing.  

Every time you use an object in modern languages, that is based on a hash table.  

Blockchain is another shift in computing that we don't yet understand the implications of.  

Blockchain is made up of nodes, which are a linked list of hash tables. Hashing is key to blockchain technology, as well as Proof of Work.

Bitcoin uses the HashCash Proof of Work system, invented in 1997 to prevent mail gateway abuse, spam, and domain squatting.  

<br>
<br>

## What is a Blockchain?

It's a chain of blocks, or a linked list. Each block contains a cryptographic hash of the previous block, a timestamp and transaction data.  

The _key_ part of blockchain is that it is immutable with reference to the preceding blocks.  

It contains an index, transactions (the data), timestamp, and hash of the previous block.  

<br>

![How Blockchain Works](./blockchain_cycle.jpg "How Blockchain Works")  

![Another How Blockchain Works](./blockchain_cycle_2.png "Another How Blockchain Works")  
<br>

When the first block is created, it contains data. The second block contains data and a hash of block one, hashed. Block three contains a hash of block two. And so on...   

If we try to change something in Block Two, the hash will be different from the stored Hash on Block Three, that references Block Two. In order to change one Block, you'd have to change all of the subsequent Blocks as well, because each modification would invalidate the stored Hash.  

In Bitcoin, value is created by requiring work -- made up problems that take a computer a long time to solve and immense amounts of electricity. This creates an "expense" for mining. The first person to solve this arbitrarily difficult problem is the one who mines the bitcoin.   

To offset the time required to solve these problems, people pool together to mine coins collectively.  

<br>
<br>

## Consensus

The Bitcoin Blockchain is public. Everyone has a copy of it and there's a network of nodes hosting a copy of it. The person with the longest chain has the "correct" chain -- the longest chain wins.  

<br>

![Why You Can't Cheat Bitcoin](./blockchain.png "Why You Can't Cheat Bitcoin")

<br>

To cheat the system in a brute force method, you'd have to not only change one block, but all the following blocks _before_ and new block is added to the chain. Due to the substantial computing power and electricity required for mining a single block, it's nearly impossible to attack so many at once.  


## Working with BlockChain  

Let's use our `blockchain.py` file from the [project repo](https://github.com/LambdaSchool/Blockchain) to start working with the concept of Blockchain.  














