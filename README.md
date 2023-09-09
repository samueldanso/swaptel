# Swaptel 
Swaptel

Our new product demo, swaptel, is a game-changer for anyone who needs to transfer money quickly and easily. With Swaptel, you can make transfers on the go, and receive instant notifications. Swaptel is designed to meet the needs of everyday people, with a user-friendly interface that makes it easy to use.

What Problem are we working to solve ?
 
In Africa, there are more people offline than those connected to the internet. As a result, financial services within the continent cost more to end users. Local and Cross-border transfers are either limited, expensive, slow or all three. Despite advertised cost savings and speed advantages, decentralized applications have barely made an impact on the daily activity of people, or disrupted legacy products at the entry-level of service delivery. Product offerings so far have resembled a dystopian informational campaign presenting technical specifications to the wrong audience; cryptography, self-custody, alphanumeric wallet data, and tutorial videos and reels for using crypto wallets.

##What solution have we developed to address said problem ?

Swaptel is a web3 Dapp that simplifies financial transactions within African communities. It builds on familiar user behavior of token transfers to anyone using a phone number. It resolves the challenge of complexity in user experience associated with cryptocurrencies, particularly for users unfamiliar with the technology, having no prior knowledge of wallets, digital currencies or self custody paraphernalia.
With Swaptel, users effortlessly send, track, and receive money using  phone numbers as unique IDs.  



##How does the application of blockchain technology help solve the problem ?

Blockchain technology enables the cost-effective transfer of digital assets between wallets. Transaction immutability serves as a fraud-proof record of transactions that can be leveraged for secondary uses, such as insurance costing, credit profiling, etc. 
Unlike alternative payment methods, Swaptel is fast, efficient, cost-effective and reliable. You can trust that your money will be transferred securely and quickly.
With Swaptel, you can enjoy the convenience of completing rapid and cost-effective  digital payments without the need for tutorials to complete a task. We’ve got easy one-click transfers, push notifications, all using your familiar phone numbers as ID. Enjoy ease with swaptel.

#Key Features:
- 1. Cost-effective transfers : enter a phone number as ID and confirm the amount to initiate a transfer.

- 2. Security : Funds are secured, and provide immutable record-keeping of all transactions. Wallet owners are the only authorized signers of transactions, authenticated at login.



#How It Works

- 1. Users log in to the Swaptel platform using their phone numbers.

- 2. A wallet is automatically created for each user profile.

- 3. Users input the recipient's phone number and specify the payment amount.

4. Users initiate the money transfer by sending it to the recipient's phone number.
 
5. Users share the Swap link with recipients through SMS or messaging apps.
  
 
#Why it Matters:
 
Swaptel simplifies the process of requesting and receiving payments, making it accessible to all users.
  
 Easy wallet creation eliminates barriers for newcomers to cryptocurrency. Whether users are new to cryptocurrency or don't possess a wallet, Swaptel offers an accessible solution. Swaptel provides a user-friendly experience, making it an ideal choice for onboarding new users to a suite of decentralized products.

 
 When you have money in Swap, it is truly yours — just like digital cash. That means no limits, no "business hours," no delays.
 
Swaptel aims to revolutionize financial transactions in Africa by offering an inclusive, cost-effective web3 solution that can onboard millions of everyday African users to web3/crypto, regardless of their technical knowledge.

 
#How it’s Made:
 
It Uses Safe{Core} AA SDK for creating the smart contract accounts on Base Görli testnet. For Login we are using a safe Auth Kit which is built on top of Web3 Auth.
 
Every link is a smart contract account, This is possible by generating the new wallet account EOAs using trust wallet’s wallet core. Once the new account is created the private key is encoded with base58 format and sent in the URL. Hence URL will act as a private key for the EOA account.
 
From the EOA account we are predicting the Safe Smart Contract Account address whenever the user tries to load the link. P.S., due to which the slow load time as well.
Smart contract address will have the reward balance. And whenever the user tries to claim it we are using a Safe Relay Kit which is built on top of the Gelato.
  
 
#Tech Stack:
 
Frontend: Next.js with app directory structure.
 
Backend: Next.js API routes.
 
Authentication: Nextauth for  wallet authentication.
 
Wallet Creation: Web3auth for wallet creation.
 
Styling: TailwindCSS and Shadchan UI for a clean and user-friendly interface.

 
#Challenges: 
 
How it can be improved:  text-based features for offline use cases to deepen the reach into remote users and target communities. 
 

#Future Outcomes: 
 
Our product feature roadmap is divided into online initiatives that build on the functionality of the product online, as well as offline initiatives that offer text-based functionality. Online initiatives include notification links for repeating frequent transfers, internal messaging and group creation for split expenses and targeted savings, and impact fundraising.
 After the basic use case of transfers to gain traction, educational content can progressively introduce an advanced suite of features in a toggle switch to pro version that offers inter-currency swaps, bulk transaction scheduling for merchant services, as well as other products.

https://www.canva.com/design/DAFt8Kt-r9I/AWY0jeG0G1L8qBOYG4Yg9g/edit?utm_content=DAFt8Kt-r9I&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
 


# Built on 🏗 Scaffold-ETH 2

🧪 An open-source, up-to-date toolkit for building decentralized applications (dapps) on the Ethereum blockchain. It's designed to make it easier for developers to create and deploy smart contracts and build user interfaces that interact with those contracts.

⚙️ Built using NextJS, RainbowKit, Hardhat, Wagmi, and Typescript.

- ✅ **Contract Hot Reload**: Your frontend auto-adapts to your smart contract as you edit it.
- 🔥 **Burner Wallet & Local Faucet**: Quickly test your application with a burner wallet and local faucet.
- 🔐 **Integration with Wallet Providers**: Connect to different wallet providers and interact with the Ethereum network.

## Contents

- [Requirements](#requirements)
- [Quickstart](#quickstart)
- [Deploying your Smart Contracts to a Live Network](#deploying-your-smart-contracts-to-a-live-network)
- [Deploying your NextJS App](#deploying-your-nextjs-app)
- [Interacting with your Smart Contracts: SE-2 Custom Hooks](#interacting-with-your-smart-contracts-se-2-custom-hooks)
- [Disabling Type & Linting Error Checks](#disabling-type-and-linting-error-checks)
  - [Disabling commit checks](#disabling-commit-checks)
  - [Deploying to Vercel without any checks](#deploying-to-vercel-without-any-checks)
  - [Disabling Github Workflow](#disabling-github-workflow)
- [Contributing to Scaffold-ETH 2](#contributing-to-scaffold-eth-2)

## Requirements

Before you begin, you need to install the following tools:

- [Node (v18 LTS)](https://nodejs.org/en/download/)
- Yarn ([v1](https://classic.yarnpkg.com/en/docs/install/) or [v2+](https://yarnpkg.com/getting-started/install))
- [Git](https://git-scm.com/downloads)

## Quickstart

To get started with Scaffold-ETH 2, follow the steps below:

1. Clone this repo & install dependencies

```
git clone https://github.com/scaffold-eth/scaffold-eth-2.git
cd scaffold-eth-2
yarn install
```

2. Run a local network in the first terminal:

```
yarn chain
```

This command starts a local Ethereum network using Hardhat. The network runs on your local machine and can be used for testing and development. You can customize the network configuration in `hardhat.config.ts`.

3. On a second terminal, deploy the test contract:

```
yarn deploy
```

This command deploys a test smart contract to the local network. The contract is located in `packages/hardhat/contracts` and can be modified to suit your needs. The `yarn deploy` command uses the deploy script located in `packages/hardhat/deploy` to deploy the contract to the network. You can also customize the deploy script.

4. On a third terminal, start your NextJS app:

```
yarn start
```

Visit your app on: `http://localhost:3000`. You can interact with your smart contract using the contract component or the example ui in the frontend. You can tweak the app config in `packages/nextjs/scaffold.config.ts`.

Run smart contract test with `yarn hardhat:test`

- Edit your smart contract `YourContract.sol` in `packages/hardhat/contracts`
- Edit your frontend in `packages/nextjs/pages`
- Edit your deployment scripts in `packages/hardhat/deploy`


## Contributing to Scaffold-ETH 2

We welcome contributions to Scaffold-ETH 2!

Please see [CONTRIBUTING.MD](https://github.com/scaffold-eth/scaffold-eth-2/blob/main/CONTRIBUTING.md) for more information and guidelines for contributing to Scaffold-ETH 2.
