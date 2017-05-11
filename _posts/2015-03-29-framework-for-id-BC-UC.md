---
layout: post
title:  "Framework for identifying a Blockchain Use case"
date:   2017-05-11 15:38:00
categories: normal
tags:
- blockchain
- use cases

#image: /assets/article_images/gopher.jpeg
comments: true
---
"*Blockchain is No Silver Bullet . It is a chain of blocks*" - Ganeshram Ramamurthy  

If an use case can be well implemented using a traditional RDMS or a trendier NoSQL
Databases - using  Blockchain to implement that will yield no greater results. 	

In order to identify an Use case for Blockchain it is important to understand the following (and forget Bitcoin for sometime )

* Blockchain is a technology for **Shared Database** - So it is important to understand what is the role of a Database in your user case

* Blockchain is a technology for **Shared Database with multiple writers** - Know who the writers are , do they modify the database directly ? Writers in most of the blockchain cases are nodes (machines)

* Blockchain is a technology for **Shared Database with multiple non-trusting writers** - identify if  this  is your use case

Even if your use case fits all the above said cases - there are solutions out there doing this without blockchain , where in the shared database is maintained by an intermediary who all the writers / readers involved trust (banks for ex).

So your use case is a candidate for Blockchain if what you need is  a technology for  
**Shared Database with multiple non-trusting writers with no central gatekeeper that is a final transaction log** enabling all the parties involved (writers/readers) to  independently verify the transaction and their authenticity .

Some compelling reasons to move away from a central gatekeeper are costs, faster transactions, automatic reconciliation, new regulation or a simple inability to find a suitable intermediary.

## Smart Transactions

Smart constraints can be applied to Blockchain based transactions . The constraints can range from say release 50 % now and rest at a later date, invalidate a transactions if certain rules are not met  and things like a collaborative transaction where a transaction can be validated only if it is signed by a group .

The options are  unlimited , but the point is these smart constraints  (or contracts) can be written into a blockchain transaction and no intermediary is needed to validate them.

So if your use case needs interactions between transactions , needs smart contracts on the transactions  themselves and can define a clear set of rules that can be defined to accept a transaction as valid  it is a candidate for Blockchain.


## Transaction and Block Validators

Blockchain is shared database of transactions that meet a certain criteria . Blocks in a block chain  could be a groups of transactions happening at a same time. And these transactions can have smart contracts on them. This brings us a natural question who validates the transactions and the block of transactions ?

 In a public blockchain any one ( or any node) can be a validator , this might not be applicable for an Enterprise - so we have private/hybrid blockchains , which really means the writers and validators are limited to a closed group. However they need not trust each other , but they can trust the blockchain because the chain can be independently validated .

So it is important to know for your use case who your validators are and why you trust them.

## When you should not use  Blockchain ?

* You are not ready to accept the application performance penalty that you get with Blockchain .   Writing to a public blockchain is slow and hard  by design .

* You cannot make your data viewable to public

* You cannot satisfactorily decide on the above discussed criteria

## Conclusion

It is important to view Blockchain  technology as a shared database of transactions that can be validated independently by  decentralized groups. This perspective really opens up the applications of this technology beyond just being a ledger to anything like shared calendars , wiki-style discussions forms , a patient portal , EMR/EHR, Asset ownership ,KYC  details, Id and authorization, IoT etc.


## references :

http://www.multichain.com/
