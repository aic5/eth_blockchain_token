# Creating a Token Using Smart Contracts

## Intro
This repository has everything you need to create a publicly traded token on the Ethereum blockchain. No coding experience necessary. 

Here are a few terms used in the roadmap:
  * **Ether** is the name of the cryptocurrency used in the Ethereum blockchain.
  * **Faucet** a website that distributes cryptocurrency (usually fake crypto) for development.
  * **Smart contract** is the script that is executed by the blockchain network.
  * **Solidity** is the coding language used to write smart contracts on the Ethereum blockchain.
  * **Node** is one computer in a network.

## How to create the token?

1. **Install MetaMask extension in your browser**

    1.1. Go to https://metamask.io/ to get the extension. This will create a Ethereum wallet and allow your computer to connect to Ethereum networks.
    
    1.2. Create a local wallet in MetaMask. `Do not keep your metamask words on your hard drive!`
    
    1.3. Change the blockchain MetaMask is using to the Ropstein network. This way we will not have to pay for transactions with real Ether. 
<br>   

2. **Get fake Ether for testing and development**

    2.1. You can get fake Ether in different ways. The simplest is to by going to an Ether faucet (http://faucet.ropsten.be:3001/). You can also contact other developers or setup your own miners to get fake Ether. 

    2.2. Get 2 Ropstein Ether from a faucet or other source. You will probably need less than 1.

<br>

3. **Copy the smart contract that will create the token** 

    3.1. Download or copy the smart contract from this repository: https://github.com/aic5/blockchain_token/blob/master/token_demo.sol. This code creates a simple utility token for trading. 
    
<br>

4. **Compile the smart contract using a online tool**

    4.1. Go to https://remix.ethereum.org/

    4.2. Paste the smart contract code in the editor section of the website.
  
    4.3. Click the *"Settings"* panel and choose the compiler version (*"0.4.16+commit.d7661dd9"*).
  
    4.4. Click the *"Compile"* panel and check if there are any errors. Green means you are ready to go.
  
    4.5. Click the *"Run"* panel. Enter the number of tokens, name of the token and code in the box below "TokenERC20", such as: 10000,"My Token","MTK".  
<br>

5. **Send the smart contract to the Ethereum blockchain**

    5.1. In the *"Run"* panel, look at the Environment combobox and select *"Injected Web"*.
    
    5.2. Click the *"Create"* button to send the smart contract to the blockchain. 
    
    5.3. A popup window from MetaMask will appear confirming that you want to send the token to the blockchain. This is when you pay for the contract creation. Click the *"Submit"* button.
<br>

6. **Checking the token in the Ethereum network and MetaMask**

    6.1. In MetaMask, click on the transaction that created the token (check the *"Sent"* panel). This will open the Ethereum block explorer with the information on the transaction.
    
    6.2. Wait a few minutes for the transaction to process... That's it. You have just created a token in the Ethereum network!

    6.2. To add your new token to your MetaMask wallet, click on the contract link. Copy the contract address (it will be a long Hexadecimal number, such as 0xA72....). That is the place in the blockchain where your smart contract exists.

    6.4. Go to MetaMask. Click in *"Tokens"*, *"Add Token"*. Enter the address for your contract. Click *"Add"*. Your token should appear on your wallet. Your token should now be tracked by your MetaMask wallet.

<br>

7. **Sending and receiving my new token**

    7.1. MetaMask is great, but it does not have an interface that allows for sending tokens directly. You can transfer tokens by using other sites, such as https://www.myetherwallet.com/.
    
    7.2. Go to https://www.myetherwallet.com/
    
    7.3. Allow MyEtherWallet to connect to your MetaMask wallet (select *"MetaMask / Mist"*). Click in *"Send Ether & Tokens"*.
    
    7.4. In the bottom right corner, click in *"Add Custom Token"*. Enter your smart contract address, symbol and decimals (18). Click *"Launch"*.
    
    7.5. Send your tokens using the *"Send Ether & Tokens"* panel. Rememeber to click the type of token you want to send by clicking in *"Amount to Send"*.
    

---

## FAQ
1. *Do I have to install or download a compiler to create a token? I do not trust these blockchain folks with their strange ways...* 

      **No, you do not need to download a compiler to create a token**. Even coding is optional (although it does help). If you have the ability to copy and paste and a functioning browser you are good to go. Think of this as baking a cake for the first time.

2. *Do I need cryptocurrency to make my token work? How expensive this is?*

      **You do not need cryptocurrency to create a token**. We can use the test Ethereum network (known as Ropstein network) that uses fake Ether. However, you do need real Ether if you would like to do the same in the main Etherereum network. The same process will work in both the test and real blockchains. 

3. *Can I trade my token using my iPhone or Android wallet?*

      **Yes, you can trade the token using an app on your phone.** That is part of the fun. I suggest using the open source Trust wallet (https://itunes.apple.com/us/app/trust-ethereum-wallet/id1288339409)

3. *How long will this take?*

      About 15 minutes. Maybe less if you know what you are doing.

4. *Is my token worth something? If so, how much?*
   
      After you finish creating your token it will be worth exactly Zero dollars. That being said, value is never intrinsic to the thing, it is a perceived feature that in most cases evolves over time. So, who knows?   





