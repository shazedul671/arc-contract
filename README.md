 How to add it:

Run this command in the terminal:

```bash
nano README.md
```

Then copy and paste the entire content below into nano:

```markdown
 ARC Testnet Smart Contract

A simple Counter smart contract deployed on Arc Testnet using the Foundry framework.

 🌐 Project Information

- Blockchain: Arc Testnet (Circle’s Stablecoin L1)
- Framework: Foundry
- Language: Solidity
- Contract Name: Counter
- Contract Address: `0x90CC........`

 📋 Features

- Smart contract deployment on Arc Testnet
- `increment()` function to increase counter
- `number()` function to view current count
- Fully functional on Arc Testnet

 🚀 Quick Start

 Prerequisites
- Foundry (`forge`, `cast`)
- Arc Testnet Wallet with USDC for gas

 Deploy Command
```bash
forge create src/Counter.sol:Counter \
  --rpc-url https://rpc.testnet.arc.network \
  --private-key $PRIVATE_KEY \
  --broadcast
```

Interact with Contract

Increment the counter:
```bash
cast send $COUNTER_ADDRESS "increment()" --rpc-url https://rpc.testnet.arc.network --private-key $PRIVATE_KEY
```

Check current number:
```bash
cast call $COUNTER_ADDRESS "number()(uint256)" --rpc-url https://rpc.testnet.arc.network
```

 📁 Project Structure

```
arc-contract/
├── src/
│   └── Counter.sol          # Main Smart Contract
├── script/
├── test/
├── .env.example
├── foundry.toml
└── README.md
```

 🔗 Useful Links

- Block Explorer: [testnet.arcscan.app](https://testnet.arcscan.app)
- Faucet: [faucet.circle.com](https://faucet.circle.com)
- Arc Network: [arc.network](https://arc.network)

 📝 License
MIT License

---

Made with ❤️ using Foundry
```

---

 Save the file:
- Press `Ctrl + O` → Press `Enter` (to save)
- Press `Ctrl + X` (to exit)

---

 Verify the file:
```bash
cat README.md
```

