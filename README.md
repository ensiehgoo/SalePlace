# Sale Place 

Ethereum based e-commerce app for sale
A decentralized application running on Ethereum were a user can purchase/sell an item and track/update its status on the go.

[EtherScan Contract Deployed Address](https://rinkeby.etherscan.io/address/0x5526d108b8a002ec2a46d000bb31fd35d263cd5c)

## What's a Sale Place
Decentralized marketplace is a blockchain-based e-commerce app. There is two types of users buyer and seller

## Seller' role
1. Seller can sell an item
2. Seller can enlist items as many as possible
3. Sellers can update the item details that they created
4. Sellers can see the items list but can't buy item that they have creted
5. Sellers can refund the purchase amount of an item once they have recieved
6. Seller can set the status of a purchase item from purchase to shipped
7. Sellers have the purchase history of an item they have enlisted

## Buyer Actions
1. Buyers can buy an item that they don't create
2. Buyers can see the list of item they have purcahsed
2. Buyer can see the list of items available in the market
4. Buyer can set the item status as received only if shipped



## Running locally
1.MetaMask can be installed from the [Firefox add-ons store](https://addons.mozilla.org/en-US/firefox/addon/ether-metamask/).

2.If you want to use local blockchain, install ganache according to your operating system from [here](https://www.trufflesuite.com/ganache)

3. Install git and truffle 
    ```sh
    # install git
    sudo apt-get install -y git
    # install truffle
    sudo npm install -g truffle
    ```
4. Install node (v10.0+), npm
    ```sh
    # install curl
    sudo apt-get install curl
    # install node & npm
    curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
    sudo apt-get install -y nodejs
5. Install project dependencies
    ```sh
    git clone https://github.com/anandmv/Sale-Place
    cd Sale-Place/client
    npm install
    ```
6. After cloning this project delete all the json files from this path("350_Decentralized_MarketPlace/client/src/contracts/") of the project.
7. After downloading ganache ui, open this in your pc, click the new workspace button here.

![alt text](https://1.bp.blogspot.com/-hqMhtEh0AH0/XEIUQH7YT6I/AAAAAAAAb5g/7MkrdQigbaIq7-cXhFsscl8zxu1QfQqJgCK4BGAYYCw/s1600/Screenshot%2Bfrom%2B2019-01-18%2B23-28-07.png)

In the next page name your project with a suitable name. Then click the add project option and navigate to the file where the truffle-config.js of this project is stored and select this. Finally click save workspace button after completing the setup.

![alt text](https://www.trufflesuite.com/img/docs/ganache/v2-shared-seese/new-workspace.png)

Then you will see a gui like that

![alt text](https://eattheblocks.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-25-at-7.58.24-PM.png)

Then leave it open like that.

8. Run the Truffle development console.
    ```sh
    cd Sale-Place
    truffle develop
    # switch back to console one (truffle console)
    compile
    migrate
    test
    ```
9. Start the React front end from the local server
    ```sh
    # console three
    cd Sale-Place
    npm start
    ```
    Be sure to configure MetaMask using the the mnemonic phrase provided by your ganache:
    ```
    candy maple cake sugar pudding cream honey rich smooth crumble sweet treat 
    ```
    Add the custom RPC endpoint when choosing a network: 
    ```
    http://127.0.0.1:7545 
    ```
    and then refresh the app page.Please confirm the network url from the truffle GUI/CLI 
    Once the app recognizes your MetaMask account you are good to go!
    
You will need to setup a firebase project and configure it [here](https://github.com/anandmv/Sale-Place/blob/master/client/src/firebase-config.js) before you start you can follow the procedure given [here](https://dev.to/itnext/react-with-firebase-firestore-setup-4ch3).


