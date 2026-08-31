# 🎯 PredictXY - Decentralized Crypto Prediction Platform

Real-time cryptocurrency price prediction platform with gamification, leaderboards, and token rewards built on Stellar Soroban.

## 🚀 Live Production Status
- **Live URL**: [https://predictxy.vercel.app](https://predictxy.vercel.app)
- **GitHub Repository**: [https://github.com/Dark-95o/predictxy](https://github.com/Dark-95o/predictxy)
- **GitHub Actions**: ✅ Passing
- **Stellar Network**: Testnet

### ⛓️ Live Soroban Contract IDs
- **Oracle Contract**: `CDXDPKE2CKZGGHNYPXQU3LAIIBXSLVWONQBP3Y4A4KOAV3ZUILL33ZRG`
- **Prediction Staking Contract**: `CDFNCCUHTU3Q2RA4DZQTHONISD32CNTVJ6KKYJFAIENOER7V7DYVQGQA`
- **Rewards Distribution Contract**: `CBT6BPI6DE2VBIP26XTYGTVLDHYNFB67PPZVHRIJKFHBF33ZYN4PB6CD`
- **Deployment Details**: Full transaction hashes and hashes logged in [`credentials.md`](file:///c:/Users/subhr/OneDrive/Documents/GitHub/Subh/credentials.md)

---

## ✨ Features & Architecture

### 🎮 Prediction Arena
- **Live Market Prices**: Real-time crypto asset tracking (BTC, ETH, SOL, ADA).
- **Interactive Price Charts**: Historical price trends rendered via Recharts.
- **Dynamic Timeframes**: 1h, 4h, 12h, and 24h prediction cycles.
- **UP / DOWN Staking**: Gamified staking mechanics powered by XPOLL tokens on Stellar.

### 🏆 Leaderboard & Gamification
- **Global User Rankings**: Filter by Daily, Weekly, and All-Time performance.
- **Performance Analytics**: Profit/loss metrics, win-rate calculation, and total volume.

### 📊 Dashboard & Wallet Integration
- **Multi-Wallet Support**: Seamless connection with Freighter, Albedo, and Rabet wallets.
- **Asset Management**: Real-time balance detection for native XLM and XPOLL tokens.
- **Referral Rewards**: Invite friends and earn commission on platform predictions.

---

## 🔗 Smart Contracts (Soroban / Rust)

1. **Price Oracle Contract** (`smart-contract/contracts/oracle`)
   - Securely records and validates crypto prices on-chain.
   - **Contract ID**: `CDXDPKE2CKZGGHNYPXQU3LAIIBXSLVWONQBP3Y4A4KOAV3ZUILL33ZRG`

2. **Prediction Staking Contract** (`smart-contract/contracts/prediction`)
   - Manages user prediction pools, stake locking, and settlement logic.
   - **Contract ID**: `CDFNCCUHTU3Q2RA4DZQTHONISD32CNTVJ6KKYJFAIENOER7V7DYVQGQA`

3. **Rewards Distribution Contract** (`smart-contract/contracts/rewards`)
   - Calculates payout distributions and maintains user on-chain performance statistics.
   - **Contract ID**: `CBT6BPI6DE2VBIP26XTYGTVLDHYNFB67PPZVHRIJKFHBF33ZYN4PB6CD`

---

## 🛠️ Technical Stack

- **Frontend**: React 19 + Vite
- **Styling**: Modern Vanilla CSS (Glassmorphism, Dark Theme, Animations)
- **Blockchain**: Stellar Soroban (Rust smart contracts)
- **SDKs**: `@stellar/stellar-sdk`, `@stellar/freighter-api`, `@albedo-link/intent`
- **Data Integration**: CoinGecko API & Soroban RPC

---

## 🚀 Getting Started

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Configure Environment**:
   Copy `.env.example` to `.env`:
   ```env
   VITE_PREDICTION_API_URL=https://api.xpoll-predictor.vercel.app
   VITE_NETWORK=testnet
   VITE_RPC_URL=https://soroban-testnet.stellar.org
   VITE_ORACLE_ADDRESS=CDXDPKE2CKZGGHNYPXQU3LAIIBXSLVWONQBP3Y4A4KOAV3ZUILL33ZRG
   VITE_PREDICTION_ADDRESS=CDFNCCUHTU3Q2RA4DZQTHONISD32CNTVJ6KKYJFAIENOER7V7DYVQGQA
   VITE_REWARDS_ADDRESS=CBT6BPI6DE2VBIP26XTYGTVLDHYNFB67PPZVHRIJKFHBF33ZYN4PB6CD
   ```

3. **Run Local Development Server**:
   ```bash
   npm run dev
   ```

4. **Build Production Bundle**:
   ```bash
   npm run build
   ```

---

## 📊 CI/CD Pipeline

Automated continuous integration and deployment configured via GitHub Actions in `.github/workflows/deploy.yml` with automated builds and deployment to Vercel.
