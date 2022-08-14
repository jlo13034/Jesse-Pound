---
layout: post
title:  "A brief Guide to Bitcoin for Beginners"
description: "An overview of what Bitcoin is as a currency and how Blockchain technology allows it to operate"
date: 2021-02-04
banner_preview: bitcoin.jpeg
banner_image: blockchain.webp
category: Tech
tags: [blockchain, technology, bitcoin]
---

Unless you’ve been living under a rock for the past decade, you’ve no doubt heard of Bitcoin — the largest and most popular digital currency on the market. But if you’re like me, you’ve never really had a solid understanding of how exactly it works or what all the hype is about. Lucky for you, I did all the nitty gritty research and have written this article for complete beginners to better understand Bitcoin!

<!--more-->

In this article, I’ll explain:

-Basics of Bitcoin
-What Blockchain is and how it allows Bitcoin to operate
-How Blocks get added to the chain
-How the Blockchain is validated
-Bitcoin mining vs. investing in 2021

Feel free to scroll to the bottom for a TL;DR summary, and if you like the article please give it some claps!

### BASICS OF BITCOIN

Bitcoin works through using Blockchain. I will explain what Blockchain is and how it operates in more detail very soon, but in simple terms it is a decentralized and anonymous database of all transactions completed through a network, listed in chronological order of the time they were executed. Users are connected to this network via nodes, which are any computer or device that has a copy of the blockchain. This allows all users to see new transactions constantly being added to the blockchain (or decentralized database) in real time, preventing fraudulent transactions and leaving an extensive log of all transactions ever made through the network. It also automates transactions, removing the need for any middle man like banks and other financial institutions, and it allows for smart contracts to be created.

{% include image_full.html imageurl="/assets/images/bitcoincurrency.png" title="Bitcoin Comparison" caption="Comparison of Bitcoin to other currencies" %}

The image above compares Bitcoin to two other popular forms of currency; gold and paper money. It’s easy to see the advantages of Bitcoin, or any cryptocurrency for that matter, over these more outdated forms of currency. So many resources and aspects of our lives are now digitzed that its surprising our currency hasn’t followed suit. But as Bitcoin and other cryptocurrencies continue to grow in popularity and as the younger generations become financially independent, the world will likely make that transition and cryptocurrencies could soon become the new normal.

In addition to it’s most popular application to cryptocurrencies, Blockchain can also be used to <a href="https://www.sdxcentral.com/articles/news/ibm-bets-big-on-blockchain-to-fight-climate-change/2021/01/">track product lifecycles</a>, <a href="https://www.thetatoken.org/">democratize internet access</a>, <a href="https://horizonstate.com/">prevent voter fraud</a>, and <a href="https://www.insurancejournal.com/news/national/2020/02/21/559057.htm">detect counterfeit drugs</a> to name just a few examples, and there are countless more innovative applications of blockchain being developed. It has the potential to revolutionalize technology, but there are some huge barriers it must first overcome. As stated in the <a href="https://hbr.org/2017/01/the-truth-about-blockchain">Harvard Business Review:</a>

> “True blockchain-led transformation of business and government, we believe, is still many years away. That’s because it is not a ‘disruptive’ technology, which can attack a traditional business model with a lower-cost solution and overtake incumbent firms quickly. Blockchain is a foundational technology: It has the potential to create new foundations for our economic and social systems. But while the impact will be enormous, it will take decades for blockchain to seep into our economic and social infrastructure. The process of adoption will be gradual and steady, not sudden, as waves of technological and institutional change gain momentum.”

This may be part of the reason blockchain is not getting as much attention as Artificial Intelligence for example, which is more obviously and more rapidly revolutionzing technology. However, I think that in the long run, blockchain will be even more impactful and is definitely worth talking about now, while it is in its early stages of development.

### HOW BITCOIN WORKS THROUGH BLOCKCHAIN

Every user on a blockchain platform has their own unique private key (or some may have multiple private keys), which is essentially just a decoded string of characters. A private key might look something like this for example:

<em>E9873D79C6D87DC0FB6A5778633389F4453213303DA61F20BD67FC233AA33262</em>

When a transaction is made with blockchain, all the data about the transaction (such as the payer and payee, the amount, etc.) is combined with the users private key to produce what is referred to as a digital signature. How exactly is this produced? Some pretty interesting math. I won’t get into the specifics of it in this article, but would highly recommend reading <a href="https://learnmeabitcoin.com/beginners/digital_signatures_signing_verifying">this</a> resource if you’re curious about it. For a user to make a bitcoin transaction, their transaction data, digital signature, and public key is first added to what’s called a transaction pool as a block. Like the private key, the public key is also a string of characters, but it is unique to the transaction itself and does not identify the user. You can think of the private key as a key to a mailbox: only the owner has that key so only they can open the mailbox and access what’s inside. The public key is like the mailbox slot: others can add things to it and view the slot itself, but they cannot see what is inside or access what is inside.

{% include image_full.html imageurl="/assets/images/bitcoinanalogy.png" title="Bitcoin Analogy" caption="The private key is like a mailbox key, and the public key is like a mailbox slot" %}

The goal of the digital signature is to prove that the mailbox actually belongs to the owner without letting anyone else see what’s inside the mailbox. In other words, the digital signature proves that you are the owner of the public key which is tied to the transaction you are trying to make, without revealing the private key which is tied to your identity.

Once a block is added to the transaction pool, it has not yet been added to the blockchain. Before that can happen, the block must be validated. There are many different validation methods that are used in blockchain, but Bitcoin uses a particular method called “Proof-of-Work”.

### PROOF-OF-WORK

You have probably heard of the term “Bitcoin miner”. Bitcoin miners are essential to the Proof-of-Work verification method used for bitcoin transactions. In order for new blocks to be added to the blockchain, they must be “mined”. The action of mining a block requires work, and once enough work has been done for a block to be mined, it is considered validated and is added to the blockchain. In other words, this means that the transaction is approved from the transaction pool and it gets added to the chain of all transactions on the decentralized database (blockchain). If all this still seems a little unclear, don’t worry — I’m about to explain what the process of bitcoin mining actually is and how Proof-of-Work validates the blocks.

Once a users transaction data, digital signature, and public key are added to the transaction pool as a block, bitcoin miners will mine them in order to receive a reward, which as of right now is equivalent to 6.25 bitcoin. There is a finite amount of bitcoin — 21 million bitcoin to be exact — that can ever be mined, and as more nodes are added to the blockchain network and more people start mining, this finite amount of bitcoin gets mined at increasingly rapid rates. To control this, the value of the reward for mining bitcoin is halved every 4 years. When Bitcoin was first introduced, the reward was set to 50 bitcoin, but as of May 2020 it was only 6.25 bitcoin.

A crucial tool used in the bitcoin mining process is cryptographic hash functions. A cryptographic hash function is a mathematical algorithm that takes an input of any length and produces an output of fixed length, which is (big surprise) called a hash. In order for a block to be mined, the miner must create a hash from the data that the block contains which also links to the hash of the previous block that is already verified and in the blockchain. Doing this is like solving an extremely complex math problem, but the only way to solve it is through guess and check and there are around 4 billion possible answers! The process requires special software and huge amounts of computational power.

The difficulty of this math problem can be adjusted by setting a target that the hash must be lower than. The lower the target, the fewer possible hash combinations there are and the harder it is to generate the correct hash. This means the hashes will begin with long strings of zeros, like this for example:

<em>000000000000000004dd3426129639082239efd583b5273b1bd75e8d78ff2e8d</em>

To ensure that they generate a hash below the target, miners will input an integer called a nonce into the block data. Then it is up to the miner’s computer to solve the complicated math problem of finding the nonce that generates a hash that is under the target. The target is deliberately adjusted so that it always takes about 10 minutes for computers to solve this problem. Multiple miners work to mine blocks at the same time, and whoever is lucky enough to mine the block first gets rewarded with bitcoin. And when I say lucky, I really do mean lucky — successfully mining a block is like winning the lottery due to the guess and check nature of the math problem your computer is trying to solve. But once the block is mined, the miner receives bitcoin as a reward and the block is then added to the blockchain and the centralized database is updated, meaning the new block can now be seen on the blockchain at all nodes. All the miners then move on to attempt at mining other blocks from the transaction pool.

### HOW DOES PROOF-OF-WORK ENSURE SECURITY?

Since each block’s hash in the blockchain is mathematically connected to the last block’s hash, in order to tamper with a block in the blockchain one would need to re-mine all of the blocks that come after it. So the farther back a block is in the blockchain, the harder it is to tamper with. Additionally, if there are multiple different version of the blockchain (which often happens due to the sheer amount of bitcoin miners who are all mining at the same time), newly mined blocks will only get added to the longest chain and that is the chain that is publicly viewable in the blockchain. This makes it quite impossible for anyone to tamper with blocks in the blockchain because once they tamper with a block, they will have to re-mine it and then re-mine all of the new blocks that had been mined and added to the blockchain in the time it took for them to do that. So essentially it would require them to mine at an extremely fast rate to catch up to all the other miners in order for their version of the blockchain to be the longest one, but as previously mentioned this is both mathematically and computationally infeasible. It would require them to control over half of the computational power in the entire network — so over 51% of the huge blockchain network would need to be cooperating with each other as hackers! This is incredibly infeasible, and gets less and less possible the bigger the network is. And that is the beauty of blockchain — it essentially eliminates any possibility of attack, tampering of data, or fraud.

### JUMPING ON THE BITCOIN TRAIN

Now that you have a better understanding of blockchain and how Bitcoin works, maybe you want to get involved. Since it first exploded in 2011, Bitcoin has generally performed very well. Someone who mined a single block back when the reward was 50 bitcoin and held on to it since 2010 would now own over $450, 000 worth of bitcoin. However, cryptocurrency in general is still a highly volatile asset (meaning it is subject to sudden significant fluctuations in value), and there are a few things you should consider before jumping on the Bitcoin train.

If you are looking to start mining bitcoin, you should seriously consider all factors involved and how serious you are about it. In today’s market it is impossible to profit from bitcoin mining as an independent at-home miner. The math problems that must be solved in order for bitcoin to be mined are 16 trillion times more difficult than they were when Bitcoin was first introduced. This is due to exponential developments in computing power that have been made in recent years, and the development of huge bitcoin mining centres created for the sole purpose of hosting extreme amounts of computational power to profit from bitcoin mining. To keep the time it takes to mine a block at a minimum of around 10 minutes, the math problems have had to become so complicated that even these huge mining centers take that amount of time to solve them. So if you want to mine your own bitcoin, you can’t just use your laptop. You will need to invest in more powerful hardware, which can range in cost from a few hundred to tens of thousands of dollars depending on how efficient it is. Even with more powerful hardware, in order to successfully mine any blocks you will likely need to join a mining pool, which are groups of individual miners who combine their computing capabilities and share the rewards. Since you share the rewards you won’t be able to make as much profit from mining each block, but in a group you will be able to mine more blocks and at least have a chance at making some profit off of it.

Another thing to consider is the reward for mining bitcoin. Since the amount gained from mining a block halves every four years and the power of computers continues to increase, the difficulty of the math problems are increasing at the same time the reward for solving them is decreasing, so it makes less and less sense to mine bitcoin at all. The graph below illustrates this issue:

{% include image_full.html imageurl="/assets/images/mininginsights.png" title="Mining Insights" caption="Mining insights graph" %}

The last factor I will mention which is a huge influencer in whether or not you can profit from mining bitcoin is the cost of electricity where you live. As previously mentioned, mining bitcoin requires huge amounts of computational power and as a result it uses a lot of electricity. It is a very real possibility that the electricity bill that will arise due to the mining process will be greater than whatever profit you make, so make sure you consider the cost of electricity where you live if you are serious about mining bitcoin. If you are trying to do a deeper analysis of whether you could profit from mining bitcoin, check out this online <a href="https://www.cryptocompare.com/mining/calculator/btc?HashingPower=15&HashingUnit=TH%2Fs&PowerConsumption=0&CostPerkWh=0&MiningPoolFee=1">profitability calculator.</a>

In my view, unless you are very serious about mining bitcoin and are prepared to invest substantial capital upfront, it isn’t worth it. It would be much easier to invest in Bitcoin by simply creating an account through a platform such as <a href="https://www.wealthsimple.com/en-ca/product/crypto/">Wealthsimple</a> and buying a few bitcoin to add to your own digital wallet. Just make sure that you understand the risks involved with this — don’t just sign up and invest a bunch of money into Bitcoin if you have no experience with managing an investment portfolio.

### TL;DR

-Bitcoin operates via a blockchain, which is essentially a decentralized database of all transactions made with bitcoin that is publicly validated and updated in real time
-When a transaction is made, all the necessary data needed to validate the transaction without identifying the parties involved is added as a “block” to a transaction pool
-For the transaction, or block, to be approved and added to the blockchain, it must be mined
-Bitcoin miners competitively mine blocks by solving complicated math problems which require immense amounts of computational power. The first miner to solve the problem gets a certain amount of bitcoin as a reward, and the transaction is approved and added to the blockchain
-This mining process is a validation method called “Proof-of-Work” and it makes it nearly impossible for transactions to be tampered with, thereby eliminating fraud
-The larger a network is (AKA the more nodes that are added to the network) the more secure it is
-Today it isn’t profitable to start mining bitcoin unless you are very serious about it and willing to invest a large amount of capital upfront. It is much easier to simply buy bitcoin, and right now (February 2021) is a great time to do so as Bitcoin is seeing very high returns

