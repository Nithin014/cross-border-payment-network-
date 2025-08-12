# Cross-Border Payment Network — Demo
This demo implements a simple cross-border payment flow:
- Frontend: React + Vite (connects to MetaMask, displays form & tx list)
- Backend: Express (stores tx metadata for demo)
- Contracts: Hardhat deployment of a StableToken and CrossBorder contract

Run instructions:
1. Install Node 18+ and npm.
2. In `contracts`: `npm install` then `npx hardhat node`
3. Deploy to local: `npx hardhat run scripts/deploy.js --network localhost`
4. In `backend`: `npm install` then `node src/index.js`
5. In `frontend`: `npm install` then `npm run dev`
6. Open the frontend, connect MetaMask to Localhost:8545, import an account from Hardhat, mint tokens using the StableToken contract, approve CrossBorder contract and deposit.
