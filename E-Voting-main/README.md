
## Installation

### Requirements

- [Node.js](https://nodejs.org/en/download/)
- [Ganache GUI](https://trufflesuite.com/ganache/) (Graphical User Interface)
- [Metamask](https://metamask.io/download) (Browser Extension)


### Configuring the project for development

1. **Clone this repository**:
   ```shell
   git clone https://github.com/AswinArsha/E-Voting.git
   cd E-Voting
   ```
2. **Install Truffle and Ganache CLI using Node Package Manager (npm)**:
   ```shell
   npm install -g truffle
   npm install -g ganache-cli
   ```

3. **Run Ganache GUI**:  
   - Launch Ganache GUI on your machine. 
   - If you haven't already, download and install Ganache GUI from [here](https://trufflesuite.com/ganache/).
   - Start Ganache GUI. 
   - If you're launching it for the first time, it may prompt you to create a new workspace. You can create a new workspace or choose an existing one.
   - Once Ganache GUI is running, it will start a local Ethereum blockchain with predefined accounts and private keys.

4. **Configure MetaMask**:
   - Open MetaMask in your browser.
   - Click on the network dropdown in the top left corner and select "Add Network".
   - A new MetaMask window will open. Select "Add a network manually".
   - Give the network a name.
   - Set the "New RPC URL" to `http://127.0.0.1:7545` (adjust the port if necessary).
   - Set the Chain ID to `1337`.
   - Set the currency symbol to `ETH`.
   - Click "Save".

5. **Import Accounts**:
   - In Ganache GUI, copy the private keys by clicking on the 'key' symbol. This will open a new "ACCOUNT INFORMATION" window.
   - In MetaMask, click on 'Add account'.
   - Select "Import account" and paste the private key.
   - Click "Import".

6. **Deploy Smart Contracts**:
   - Navigate to your project directory where you have your Truffle project set up.
   - Ensure that your `truffle-config.js` file is configured to connect to your local Ganache blockchain.
   - Run `truffle migrate` in your terminal to deploy your smart contracts to the local blockchain.

7. **Launch the development server (frontend)**:
   ```shell
   cd client
   npm install
   npm start
   ```
    > **Note:** If you encounter an error during `npm install`, you might need to install Microsoft Visual C++ Redistributable packages from [here](https://aka.ms/vs/17/release/vc_redist.x64.exe).


---

