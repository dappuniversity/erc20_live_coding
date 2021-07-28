## Deploy Simple ERC20 Token on Remix

### Deploy Token on Remix 

1. Compile and deploy contracts on JVM to check all is working well 

- Copy Token.sol Solidity Code into a file in Remix rename Token.sol
- Select Solidity Compiler Page
  - On Compiler Options dropdown select 0.8.6 version
  - Click "Compile Token.sol" button
- Select Deploy and Run Transactions Page
  - Environment dropdown select JavaScript VM
  - Accounts dropdwon -> pick any of the accounts in dropdown
- Deploy Button
  - Enter the parameters for deployment for (name, symbol, decimals,totalSupply) 
  - Example paramters "TokenName", "TKT", 18, 7000
  - Click deploy button
- Deployed Contracts
  - Scroll down to deployed contracts section and click on deployed contract
  - View buttons for all the functions you can carry out on contract e.g approve, transfer etc

1. Deploy Token to Kovan Testnet

- Select Deploy and Run Transactions Page
  - Environment dropdown select Injected Web3 (to allow use of Metamask)
  - Accounts dropdwon will have first currently selected Metamask account
- Get some testnet ETH, Kovan ETH into the deploying account 
  - Copy the address from accounts 
  - Go to [https://linkfaucet.protofire.io/kovan](https://linkfaucet.protofire.io/kovan) paste account and request some Kovan ETH
- Deploy Button
  - Enter the parameters for deployment for (name, symbol, decimals,totalSupply) 
  - Example paramters "TokenName", "TKT", 18, 7000000000000000000000
  - Click deploy button and confirm transaction on MetaMask
- Deployed Contracts
  - Scroll down to deployed contracts section and click on deployed contract
  - View buttons for all the functions you can carry out on contract e.g approve, transfer etc (Deployer will have all the initial tokens)
  - Copy the Deployed Token address on Deployed Contracts e.g 0x5b01c8aE3185774068AF96978e1461c2A31e8A9e

### List ERC20 Token on Uniswap 

- Go to [Uniswap](https://app.uniswap.org/)
  - Click on Pool Tab
  - Click on More Tab and Select Create Pool
- Add Liquidity 
  - Under Select Pair leave ETH selected 
  - Click on Select Token dropdown 
  - Paste your deployed Token address into Search 
  - Your deployed Token will show => Click Import 
  - On same add Liquidity Page, select a fee e.g 0.3% fee ideal for stable pairs
- Initialize Pool 
  - On same Liquidity Page => Set the starting price for Token e.g 0.001
  - Set the price range 0.001 to 0.002
- Deposit Amounts 
  - Ensure you have sufficient balances for the amounts you will choose to deposit 
  - Select amount of ETH to deposit e.g 0.001 ETH corresponding equal amount of your Token will be displayed
  - Click Approve Button and confirm transaction on Metamask
  - Once transaction finished you can click on Preview to view the added Token vs ETH liquidity pool 
  - Click Add to finalize the adding of assets and liquidity pool creation
- New Pool will display once success on your positions on page 





