# Coffee Supply chain & data auditing
Version 2.0

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The 4 actors in the coffee supply chain are:

- Farmer: The Farmer can harvest coffee beans, process coffee beans, pack coffee palettes, add coffee palettes, ship coffee palettes, and track authenticity.
- Distributor: The Distributor can buy coffee palettes and track authenticity.
- Retailer: The Retailer can receive coffee palettes and track authenticity.
- Consumer: The consumer can buy coffee palettes and track authenticity.


The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)


### Contract Creation Addresses on the Rinkeby Network:
- Migrations: Tx hash: 0x5db96d7697f19c2a883269123a37ac6c8695d1a1e1d2c9f3a1ec215c72aec2da
Contract address: 0x67F8E03e71EE0e02eaeA91F3c33a1AAd6cfc24ee

Etherscan: https://rinkeby.etherscan.io/tx/0x5db96d7697f19c2a883269123a37ac6c8695d1a1e1d2c9f3a1ec215c72aec2da
https://rinkeby.etherscan.io/address/0x67f8e03e71ee0e02eaea91f3c33a1aad6cfc24ee

- FarmerRole: Tx hash: 0xbbf607c962ddd848d33aeee37576babc972627046988855d8af2475d32cc1830
Contract address: 0x75535fe0CCD740f29dFDC7879760a656cF191A5E
- DistributorRole: Tx hash: 0x2586edb75fff30db55ba557adbe9a84e206115f1b95714e8382e43d5616a560c
Contract address: 0x5006667AD4557285eEf17BEF7EA53B3b77B851D2
- RetailerRole: Tx hash: 0x9563d85b41fa916e8dd97debf73f66e0d7fd39c1ea1c280231b94f9913a60d69
Contract address: 0xabDEA977B468ef8235DEc2FCCEb5eD6332611Ce5
- ConsumerRole: Tx hash: 0xe4b7fea725a12b2ca4c56b828d603ef948b279c69b182147cbd20d01bf521366
Contract address: 0x092844755A8AFc4F20BA818d5792E514dA80bba9
- SupplyChain: Tx hash: 0xbeadbf1d68ecc8dda5d3a87831437c65f5e3bc20107355d2c1f366105b888ba9
Contract address: 0x67C57Ac36E7b1083851Ef618f00CD8285f6F6F36


## UML Diagrams

### Activity Diagram


![truffle test](project-6/UMLs/Coffee_Supply_Chain_Activity_Diagram.jpg)

### Sequence Diagram


![truffle test](project-6/UMLs/Coffee_Supply_Chain_Sequence_Diagram.jpg)

### State Diagram


![truffle test](project-6/UMLs/Coffee_Supply_Chain_State_Diagram.jpg)

### Data Model


![truffle test](project-6/UMLs/Coffee_Supply_Chain_Data_Model.jpg)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

Truffle v5.0.21 (core: 5.0.21)

Node v10.15.3

Solidity >=0.4.24

### Installing

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/sdossou/Project-6b-Coffee_Supply_Chain
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS
* Infuria
* Metamask
