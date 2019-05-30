Vehicle Registration and Sales using Ethereum


# Description:


This is a simple application that helps in keeping vehicle history. Vehicle details are entered during the time of purchase of the vehicle. Presently it will keep track of the owner and the sales record, it can be easily expanded to keep service records and legal history also.


The main contracts involved are Car.sol and newCar.sol. Car.sol is the main contract and newCar.sol inherits the properties of Car.sol. Each car added is given a unique registration number, there is buyer and seller. Mappings and events are used as data structures and also events are triggered for particular actions.


This Dapp is a beta model which helps in removing manual third party involvement in buying and selling cars and has room for further future proofing.  


#############################
Installation Instructions
#############################


Please ensure that your computer has the following prerequisites installed before proceeding:


-node npm
-truffle
-ganache-cli
-geth --datadir "data" --rpc --rpcport "8545" --rpccorsdomain "*" --rpcapi "db,eth,net,web3,personal" --ipcpath "~/.ethereum/geth.ipc" --dev --unlock "0"
-metamask-extension (preferably in google chrome) [with at least 1 ether in a couple of the accounts in Ropsten/Rinkeby/localhost]


1) Clone the repo into a local folder.
2) From the terminal navigate to 'frontend'.
3) Execute 'npm install' to install all the necessary dependencies.


[For local execution]
1) In another terminal run 'ganache-cli'.
2) From the terminal navigate back to the root folder.
3) Execute 'truffle compile' and then 'truffle migrate'[make note of the transaction address shown on screen].
4) From the terminal navigate to 'frontend' and execute 'npm start'.[This will fire up the dApp on your browser]


[For testnet execution]
1) Deploy contracts on to the test net of your choice
2) Ensure your metamask account has at least 1 ether on the said network.
3) From the terminal navigate to 'frontend' and execute 'npm start'.[This will fire up the dApp on your browser]
