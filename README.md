# Bitcoin B's conversion

To testrun this program locally with hardhat localhost,
1. open up the backend in VScode and in the terminal run:  ```console
yarn hardhat node
```
This will deploy all contracts to the "fake" hardhat localhost blockchain (chainId 31337)
Update your constants.js (in b-donate-front) with the new contract address.
In your constants.js file, update the variable contractAddress with the address of the deployed "FundMe" contract. You'll see it near the top of the hardhat output.

Connect your metamask to your local hardhat blockchain.
```PLEASE USE A METAMASK ACCOUNT THAT ISNT ASSOCIATED WITH ANY REAL MONEY.``` I usually use a few different browser profiles to separate my metamasks easily.

In the output of the above command, take one of the private key accounts and import it into your metamask.

Additionally, add your localhost with chainid 31337 to your metamask.


2. open the frontend and 
Click the “Go Live” button at the bottom-right-hand corner of VSCode to start a server on port 5500. This will also often prompt your browser to open a new window/tab that loads your index.html file.
If the browser doen't open then go to [a link]http://127.0.0.1:5500/

3. You can play around with the website functionality including funding, and withdrawing. The balance is logged into the console, so to see that, press cmd/ctrl + shift + i
and then press the balance button.

If you quit this and the on a later occasion you want to do this again you will need to first open your metamask,
go to settings, ---  advanced, --- and choose RESET WALLET
otherwise you will get this NONCE error in the console and the functions wont work anymore.
```MetaMask - RPC Error:
[ethjs-query] while formatting ouputs from RPC '{"value":{"code":-32603,"data":{"code":-32000,"message":"Nonce too high. Expected nonce to be 2 but got 4. Note that transactions can't be queued when automining."}}}'```

have fun!