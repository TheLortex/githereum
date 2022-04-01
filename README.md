# githereum

Githereum is a blockchain based on the distributed control system Git with a novel consensus algorithm based on Github pull requests.
As such, it features:
 - a currency, named the Gitcoin, that people can use to exchange goods and services.
 - a transaction system: simply fork the project, edit the blockchain state and submit a pull request to perform a transaction.
 - _smart contracts_ are implemented as legal documents in the `/smart` folder

Thanks to its disruptive consensus algorithm, the chain is self-upgradeable and open for contributions, so don't hesitate to take ownership 
and propose changes and new contracts !

## Money

Each Github user starts with 10 Gitcoins, and can ask for them by opening an _issue_ containing a proof of existence.
The monetary value of the Gitcoin is a constant integer and that integer is zero. As such, Gitcoins can be considered as _internet points_.

The ledger content is stored in this file: `/purse`

## Transaction

To perform a transaction:
 - 🍴 fork the repository
 - ✏️ edit the blockchain state as needed
 - 📈 submit a _pull request_

The review process is completely decentralized as anybody can comment on the _pull request_. 
The _pull request_ can either be accepted or denied by a _dictator_. A _dictator_ is an user appearing in the `/dictators` files. 

A transaction is considered valid if:
 - the math checks out
 - the creator of the transaction has proven its existence
 - the contracts are respected

## Smart contracts

Just add legal documents in the `/smart` folder.

## Q&A

- **Is this secure ?** This blockchain is very secure because Github is HTTPS-compliant, also I will enable branch protection on the main branch so trust the white paper (this readme).
- **Is this decentralized ?** This is a git repository so yes indeed git is decentralized, Github is just the interface (send patches by email if you don't want to use Github).
- **Doesn't look very efficient to me.** Okay, rude. This is low tech and substainable.

