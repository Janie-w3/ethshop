# Ethereum Shop

This tutorial is meant for those with a basic knowledge of Ethereum and smart contracts, who have some knowledge of HTML and JavaScript, but who are new to dapps.

# What we'll do

- Setting up the development environment.
- Creating a Truffle project using a Truffle Box.
- Writing the smart contract.
- Migrating the smart contract.
- Creating a user interface to interact with the smart contract.
- Interacting with the dapp in a browser.

### Default config for truffle.js

```
module.exports = {
    networks: {
        development: {
            host: "127.0.0.1",
            port: 8545,
            network_id: "*" // Match any network id
        }
    }
};
```
Window's user rename the **truffle.js** file to **truffle-config.js**

# How to setup

Install **NodeJS** (includes **NPM** 5.5.1) [https://nodejs.org/en/download/]

**Open terminal and run** 

1. Install Truffle globally ``npm install -g truffle``

2. Clone the project using ``git clone https://github.com/sany2k8/ethshop.git``

3. Install the dependencies from package.json file ``npm install`` 

4. Now, you have **2** choices whether you can use **Truffle develop** or run **TestRpc**

 A. **Using Truffle develop**

 Run the development console. `truffle develop`

 Compile the smart contracts. ``compile``
 
 Migrate the smart contacts. ``migrate``

 B. **Using TestRpc**

 Install ``testrpc``, using ``npm install -g ethereumjs-testrpc`` [https://github.com/ethereumjs/testrpc]

 Run the testrpc using ``testrpc``

 Migrate the smart contacts ``migrate``

5. Run the **liteserver** development server (outside the development console) for front-end hot reloading.

 Run the DAPP : ``npm run dev``

The DAPP will serve the front-end on [http://localhost:3000]