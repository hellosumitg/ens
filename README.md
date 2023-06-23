# The Ethereum Name Service

![](https://i.imgur.com/eOvGgU7.png)


## Background
When web initially started the only way you could explore information on the web was by entering in its IP address. After that the concept of DNS was introduced which helped us to link a domain name to an IP address.

So whenever you type `google.com`, DNS takes care of translating it to the respective IP which is what the computer finally understands.

## What is ENS?

- ENS stands for `The Ethereum Name Service` and it behaves very similar to how DNS behaves in the web2 space. 
- As we all know that Ethereum has long addresses which are hard to remember or type
- ENS solves this issue by translating these wallet addresses, hashes etc into readable domains which are then saved on Ethereum blockchain
- The best part about ENS is unlike DNS servers which are centralized, ENS works with the help of a smart contract which is censorship resistant.
- So now when you are sending your wallet address to someone which looks like `0x1234huiahi....` you can actually send them `tom.eth` and the ENS would figure out that `tom.eth` is actually equal to your wallet address (`0x1234huiahi....`)


## Requirements

Its time to build something where we can use ENS.

We will develop a website which can display the ENS for an address if it has one.

Lets go... 🚀


## Setup

- First lets get an ENS name for your address, start by opening up [https://app.ens.domains/](https://app.ens.domains/)
- Make sure when you open the website, your MetaMask is connected to the `Rinkeby testnet` and it has some `Rinkeby Ether`
- Search for an ENS domain name, any name you like, as long as it is available!
- Click on `Available`

    ![](https://i.imgur.com/1p0EBmv.png)

- Then click on `Request To Register`
![](https://i.imgur.com/zBG5JRo.png)

- When the progress bar enters the 3rd step, Click `Register`
![](https://i.imgur.com/a4nd6O4.png)

- Then after the progress bar finishes click on `Set As Primary ENS Name`

    ![](https://i.imgur.com/8cXXopd.png)

- From the dropdown then select the ENS name you just created

    ![](https://i.imgur.com/MgSrlyG.png)

- Click `Save`
  ![](https://i.imgur.com/8qOcAnp.png)

- Now you have an ENS registered to your address on Rinkeby

Awesome, You did it ❤️

## Website

- To develop the website we will use [React](https://reactjs.org/) and [Next Js](https://nextjs.org/). React is a javascript framework used to make websites and Next.js is a React framework that also allows writing backend APIs code along with the frontend, so you don't need two separate frontend and backend services.
- First, You will need to create a new `next` app. Your folder structure should look something like

  ```
  - ENS
  ```

- To create this `next-app`, in the terminal point to ENS folder and type

  ```bash
  npx create-next-app@latest ./
  ```

  and press `enter` for all the questions

- Now to run the app, execute these commands in the terminal

  ```
  cd my-app
  npm run dev
    or
  yarn dev
  ```

- Now go to `http://localhost:3000`, your app should be running 🤘

