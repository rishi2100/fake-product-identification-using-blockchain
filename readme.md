# 🚫 Fake Product Identification using Blockchain

## 📦 Packages Required:
- **Truffle** v5.6.7 (core: 5.6.7)
- **Ganache** v7.5.0
- **Solidity** v0.5.16 (solc-js)
- **Node.js** v15.8.0
- **Web3.js** v1.7.4
- **npm** 7.5.1

## 💻 Other Requirements:
1. Any browser (e.g. Chrome, Firefox, etc)
2. MetaMask browser extension

---

## 🛠️ Setup Process

1. **Clone the Project**
   ```bash
   git clone https://github.com/Sumanth9797/Fake_product_detection_using_blockchain
   ```

2. **Navigate to Project Directory & Install Dependencies**
   ```bash
   cd Fake_product_detection_using_blockchain
   npm install
   ```

3. **Compile Smart Contracts**
   ```bash
   truffle compile
   ```

4. **Setup Ganache (Local Blockchain)**
   - Open Ganache
   - Create a new workspace
   - Add the `truffle-config.js` from this project
   - Set **port** to `7545` in Ganache **Server Settings**

5. **Setup MetaMask in Chrome**
   - Add a new **Custom Test Network**:
     - **Network Name**: Ganache Local
     - **RPC URL**: `http://127.0.0.1:7545`
     - **Chain ID**: `1337`
     - **Currency Symbol**: ETH (optional)
     - **Network ID**: `5777`
   - Import an account using the **private key** from any Ganache account

6. **Run Migrations to Deploy Contracts**
   - To deploy contracts cleanly every time:
     ```bash
     truffle migrate --reset
     ```
     This ensures that all contracts are redeployed even if they were deployed earlier.

7. **Start the Dev Server**
   ```bash
   npm run dev
   ```
   This will start the server and open the homepage (`index.html`) in your default browser.

8. **Connect MetaMask**
   - Log in to MetaMask
   - Connect your imported Ganache account to `localhost:3000` (your app)

9. **🎯 Interact with the DApp**
   - You can now use the app to add and verify fake products using Blockchain!

