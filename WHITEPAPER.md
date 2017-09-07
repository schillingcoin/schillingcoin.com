# SchillingCoin White Paper

Smart economy on the blockchain

## SchillingCoin design goals: Smart Economy

SchillingCoin makes use of blockchain technology as well as digital identity to digitise assets and be able to use self-managed smart contracts. By combining these technologies, SchillingCoin is trying to archive a decentralised smart-economy


### Digital Assets

Digital assets are programmable assets that exist in the form of electronic data and are being stored on the blockchain. Therefor they can be decentralised, trustful, traceable, highly transparent and free of intermediaries. Users of the SchillingCoin blockchain are able to register, trade or circulate multiple types of assets. Proving the link between digital and physical assets is possible through digital identity. Through a validated digital identity assets are protected therefor by law.


SchillingCoin has 2 forms of digital assets available: 

1) Global Assets: Those can be recorded in the system space and can be identified by all smart contracts and clients
2) Contract Assets: These are recorded in the private storage area of the smart contract and require a compatible client to recognise them. Contract assets have to adhere to certain standards in order to achieve compatibility with different clients.


### Digital Identity

Digital identity refers to the identity information of individuals, organizations, and other entities that exist in electronic form. The more mature digital identity system is based on the PKI (Public Key Infrastructure) X.509 standard. With SchillingCoin, we will implement a set of X.509 compatible digital identity standards. This set of digital identity standards, in addition to compatible X.509 level certificate issuance model, will also support Web Of Trust point-to-point certificate issuance model. Our verification of identity when issuing or using digital identities includes the use of facial features, fingerprint, voice, SMS and other multi-factor authentication methods. At the same time, we will also use the blockchain to replace the Online Certificate Status Protocol (OCSP) to manage and record the X.509 Certificate Revocation List (CRL).



### Smart Contract

Smart contracts were first proposed in 1994 by the cryptographer Nick Szabo, just five years after the creation of the World Wide Web. Szabo defined a smart contract as the following: When a pre-programmed condition is triggered, the smart contract will execute the corresponding contract terms. By taking advantage of the blockchain technology, we get a decentralized, tamper-resistant and highly reliable system in which smart contracts can be implemented. SchillingCoin has an indepentend smart contract system built in: the SchillingCoin Contract.

SchillingCoin's smart contract system is the biggest feature in our developer ecosystem. Developers do not need to learn new programming languages or syntaxes. They can rely on already existing languages and program the smart contracts in either C#, Java or other mainstream languages, and they can also use their favorite IDE's for developing, debugging and compiling the smart contracts. 


The SchillingCoin VM is a Universal and Lightweight Virtual Machine embedded into the blockchain which gives the developer high certainity, concurrency and scalability. The SchillingCoin smart contract system allows quick development of smart contracts for developers around the world. The SchillingCoin contract will get a separated, specially crafted whitepaper describing the implementation details.




## SchillingCoin Management Model

### Economic Model

The Schillingcoin has two native tokens:

1) SchillingCoin (abbreviation ATS, for AusTrian Schilling)
2) Groschen (abbreviation GRS)


"SchillingCoin", with a maximum total of 100.000.000 tokens, respresents the right to manage the network, for example the right to vote a bookkeeper, network parameter changes and so on. The SchillingCoin itself is indivisible.

"Groschen", with also a maximum total of 100.000.000 tokens, represents the fuel token required in the SchillingCoin network for resource control. The SchillingCoin network charges its users for the storage of tokens, smart contracts or the operation of those, creating therefor economic inventives for bookkeepers and preventing the abuse of resources. Groschen (GRS) minimum unit is at 0.00000001 

In the so-called "Genesis-Block" (first ever block) of the SchillingCoin network, 100.000.000 (one hundered million) SchillingCoins (ATS) are generated. At this point in time, GRS would not be generated yet. 
100.000.000 (one hundered million) GRS which correspond to the 100.000.000 (one hundered million) are going to be generated automatically through the use of a decay-algorithm in about 22 years time after genesis.
If SchillingCoin (ATS) is being transferred to another address, the corresponding GAS will also be credited to the new address.


The SchillingCoin network will have a threshold by vote, to exempt GRS from a certain amount of transactions and smart contract operations to enhance the networks stability and the use experience.
When there are large amounts of spam transactions, SchillingCoinID can be used to prioritize transactions or smart contracts with qualified identities. If there is no qualifying digital identity available, the transaction can get a higher priority by paying a higher fuel fee: Groschen (GRS)





### Distribution 

SchillingCoins 100.000.000 (one hundered million) tokens is divided into two portions:

1) 50.000.000 (fifty million) tokens are being locked up for the duration of 1 year after the ICO by a smart contract
2) 50.000.000 (fifty million) tokens are being distributed for the following use:

*) 10% (10.000.000 / ten million) tokens will be used for paying developers and the council of SchillingCoin
*) 10% (10.000.000 / ten million) tokens will be used for motivating developers in the SchillingCoin community
*) 10% (10.000.000 / ten million) tokens will be used for cross-investing in the development of other block-chain projects that would benefit SchillingCoin, such as cross-chain communication partners.
*) 10% (10.000.000 / ten million) tokens will be retained as a contigency 
*) 10% (10.000.000 / ten million) tokens will be distributed on the ICO 


Groschen (GRS) distribution:

A Groschen is generated with every new block. The initial amount of GRS on creation of the genesis block is zero. By increasing the rate of the blocks generation, the total set limit of 100.000.000 (one hundered million) GRS will be achieved in about 22 years. The interval for every new block is aproximatively 15-20 seconds, therefor about 2 million blocks should be generated per year. 

Since there are going to be around 2.000.000 (two million) blocks generated and the initial generation is 8 GRS per block, the annual reduction will be 1 GRS per block and year to coincide with the passing of every 2.000.000 blocks. The reduction of GRS per block will continue to just 1 GRS per block and will be held at that rate for 22 years. After the generation of the 44th millionth block the total amount of generated GRS will have reached 100 million. From this point there will be no more generation of GRS from new blocks.

By taking in consideration the current release curve, 16% of all GRS should be created in the firt year. 52% in the first four years and 80% of the total GRS should be created in the first 12 years. 

Holders of SchillingCoin (ATS) can claim their gas at any time at their holding address.


### Governance mechanism


Chain governance: SchillingCoin holders can manage the network through voting, using the Groschen (GRS) that is being generated from their SchillingCoins (ATS). SchillingCoin tokens themselves can be transferred. 

Off-chain governance: The SchillingCoin council consists of the founders of the SchillingCoin project, under which the management comittee is responsible for strategic decision-making. 


## SchillingCoin technologic implementations

### Consensus mechanism: dBFT


dBFT, abbrevation for "Delegated Byzantine Fault Tolerance" is a consensus mechanism that is fault-tolerant, which enables large-scale participation consensus throgh proxy voting. Hlders of Schillingcoin tokens can vote for a supported bookkeeper. The elected bookkeepers can reach a consensus through the BTF algorithm and can generate new blocks. Votings in the network are executed in real time, rather than in accordance with a fixed term.

dBFT provides  fault tolerance of f = ⌊ (n-1) / 3 ⌋ for a consensus system consisting of n consensus nodes. This type of fault tolerance includes both security and availability. It is therefor resistant to general and Byzantine failures and is suitable for any type of network environment. dBFT has good finality, meaning that once a confirmation is final, the block can not be altered or bifurcated anymore, thus the transaction can't be rovoked or rolled back anymore.


In the SchillingCoin dBFT consensus mechanism a block takes about 15 to 20 seconds to be generated, which leads to a transaction throughput up to about 1.000TPS (transactions per second). Among the already established public chains this is an excellent performance. This is not the maximum of TPS possible, because through proper optimization it can reach up to 10.000TPS, allowing it to support also large-scale commercial applications. 

SchillingCoin also combines dBFT with digital identity technlogy, meaning that bookkeepers can be a individual, or an institution. Thus, it is possible to alter, revoke, inerhit, retrieve or even freeze assets due to judicial decisions on them. This helps to facilitate the registration of regulatory compliant financial assets in the SchillingCoin network. We are planning on supporting such operations in the network if necessary.



### Smart contract system: SchillingCoin Contract

The smart contract szstem consists of three primary parts:


**SchillingCoinVM - Universal Block Chain Virtual Machine:**


The SchillingCoin VM is a Universal and Lightweight Virtual Machine with an architecture that is very close to the JVM and .NET Runtime, similar to a virtual CPU that reads and executes instructions in the contract in sequence, performs process control based on the functionality of the instruction operations, logic operations and so on. It has a good start-up speed and versatility, is very suitable for small programs such as smart contracts, can also be ported to non-blockchain of the scene, or integrated with the IDE to provide an optimal development experience. SchillingCoinVM's functionality can be extended, like introducing a JIT (real-time compiler) mechanism, thereby enhancing the efficiency of the implementation.

**InteropService - Interoperable Services:**

The InterOPService is benig used to load the blockchain, digital assets, digital identity and other services. Those are built like virtual machines, enabling smart contracts to access these services at run time to achieve some advanced functionality. By using this kind of low-coupling desin, **SchillingcoinVM can be ported to other blockchains or non-blockchain systems, therefore increasing the utility of the smart contracts.**

**DevPack - Compiler and IDE plugin:**

DevPack includes a high-level language compiler and the required IDE-plugin. Since SchillingCoinVM's architecture is similar to JVM and .NET Runtime, the supplied compilers in the DevPack can compile Java byte code and .NET MSIL into SchillingCoinVM's instruction set. C# or Java developers therefor do not need to learn a new language and will be able to easily and quickly understand and create smart contracts in Visual Studio, Eclipse or other familiar IDE environments. **The learning curve is being reduced massively for developing smart contracts, allowing us to easily build a big community arround the SchillingCoin's Smart Contracts.


The SchillingCoin Contract can create a call tree through static analysis before running a smart contract. **By using a deterministic call tree, the SchillingCoin node can fragment a smart contract dynamically to achieve theoretical unlimited expansion**, thus overcoming the well-known "jamming-effect" caused by static fragmentation used in other public blockchain systems.



### Cross-chain interoperability agreement: SchillingCoinX

SchillingCoinX is a built-in protocol that is able to implement cross-chain interoperability. This protocol is devided into two parts: 

1) Cross-chain assets exchange protocol
2) Cross-chain distributed transaction protocol


**Cross-chain assets exchange protocol:**

SchillingCoinX is extended on existing double-stranded atomic assets exchange protocls to allow multiple participants to exchange different assets across multiple kinds of chains, to ensure that all steps in the transaction process succeed of fail together. To achieve this function, we need to create a contract account for each transaction participant. If other blockchains are not compatible with the SchillingCoin Contract, they can still be compatible with SchillingCoinX, as long as they provide simple smart contract functionalities.


**Cross-chain distributed transaction protocol:**

Cross-chain distributed transactions can be scattered across different blockchains and still ensure the consistency of the entire transaction. This is an extension of cross-chain assets exchange, extending the behavior of assets exchange into arbitrary behavior. In layman`s terms this means that SchillingCoinX makes it possible to have different parts of smart contracts on multiple chains, which in the end each of those can suceed or revert the transaction as a whole. Therefore this gives excellent possibilities for cross-chain collaborations between multiple blockchain projects.


### Distributed Storage Protocol: SchillingCoinFS (FS = File System)

The SchillingCoin File System is a distributed storage protocol which utilizes DHT (distributed hash table) technology. The protocol indexes the data by the hash of the files content, rather than by the filepath (URI). Large files are being devided into fixed-size data blocks which are then distributed and stored on different SchillingCoin nodes.

With this type of system for storage there is the big problem of finding a good balance between redundancy and reliability. SchillingCoinFS plans to solve this by offering token incentives and the establishment of backbone nodes. Users can choose their preferred reliablity level of the stored files. Files with a low level of reliablity can be stored and accessed for free or almost free. Files that need a high level of stability and reliability will be provided by backbone nodes.

The SchillingCoinFS protocl will server as one of the interoperability services under the SchillingCoin smart contract system, enabling smart contracts to store large files directly on the blockchain. In addition, SchillingCoinFS can be combined with digital identity so that digital certificates used by digital identities can be assignet, sent and revoked without a central server to manage them. For the future it is planned to store old block data in the SchillingCoinFS, so that full nodes can release old data for better scalability and at the same time, ensure the integrity of historical data. 


### Anti-quantum cryptography mechanism: SchillingCoinQS (QS = Quantum Safe)

The emergence of quantum computers pose a major threat to RSA and ECC-based cryptographic mechanisms. They can can solve a large number of the existing decomposition problems (which RSA relies on) and also the elliptic curve discrete logarithm which ECC rlies on in a very short amount of time. SchillingCoinQS uses a lettice-based cryptographic mechanism. 
Current quantum computers are not able to quickly solve the Shortest Vector Problem (SVP) and the Closest Vector Problem (CVP), therefore making those the most reliable alogrithms for resisting quantum computers. 

## Summary

SchillingCoin is a network that combines digital assets, digital identities and smart contracts. The Schillingcoin project will use dBFT, SchillingCoinX, SchillingcoinFS, SchillingCoinQS and many other technologies as the infrastructure for the intelligent economy of the future. 
