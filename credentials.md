# 📜 PredictXY Soroban Deployment Credentials & Contract Details

> **Network**: Stellar Testnet (`https://soroban-testnet.stellar.org`)  
> **Deployment Date**: August 31, 2026  
> **Status**: ✅ All 3 Soroban Contracts Successfully Deployed & Initialized

---

## 👤 Account & Key Details

| Parameter | Address / Value | Notes |
| :--- | :--- | :--- |
| **Requested Account ID** | `GBQMA5C3GCWF3ZSPUS5YANPTPCKVMJME25KPVIBU2Z3PMYQHUEMXM7QK` | Target deployment account |
| **Deployer Account ID** | `GDBXC2M7LM2IDVJGANPYKGV4WZZLVICH7MSWZBT6XHMUVAMOD2AR2FCG` | Active testnet deployer identity |
| **Deployer Secret Key** | `SC65NTKZ2N2Z6BEO3UA7MVFQMUPXDXGNLKH75GEM5QNMOFMJQHY6HM2G` | Keep secure |
| **Deployer Balance** | `10,000 XLM` (Friendbot funded) | Testnet XLM |

---

## 🔗 Smart Contract Deployments

### 1. Price Oracle Contract (`price_oracle.wasm`)
- **Contract ID**: `CDXDPKE2CKZGGHNYPXQU3LAIIBXSLVWONQBP3Y4A4KOAV3ZUILL33ZRG`
- **WASM Hash**: `9ee72faa6dceb95f39ee151e635084fe45729cc1d27e663c6eb4663f06b5981e`
- **Deployment Transaction Hash**: `607b5f3c73547a6f7b817fb0b69f0267b8792c3dc010ae89fa6e875b147e4674`
- **Initialization Transaction Hash**: `4af44d57c31097642aa448fa288dce7392337e986a4103812bd329af24d10713`
- **Stellar Expert URL**: [View Deployment Tx](https://stellar.expert/explorer/testnet/tx/607b5f3c73547a6f7b817fb0b69f0267b8792c3dc010ae89fa6e875b147e4674)
- **Stellar Lab Explorer**: [Inspect Oracle Contract](https://lab.stellar.org/r/testnet/contract/CDXDPKE2CKZGGHNYPXQU3LAIIBXSLVWONQBP3Y4A4KOAV3ZUILL33ZRG)

### 2. Prediction Staking Contract (`prediction_staking.wasm`)
- **Contract ID**: `CDFNCCUHTU3Q2RA4DZQTHONISD32CNTVJ6KKYJFAIENOER7V7DYVQGQA`
- **WASM Hash**: `fc52d62975840b50e2f9cc4501e2ce0b6e86f120734938cf612a6770ee966a2e`
- **Deployment Transaction Hash**: `f864b20d7381dfb8ea7661c5c001177aa59787dd93ae87a118fc89adebe22a4b`
- **Initialization Transaction Hash**: `daeadf65d83f1511892b505b6977437dfb2d45688da76c8f56e8746f1d9c15fa`
- **Stellar Expert URL**: [View Deployment Tx](https://stellar.expert/explorer/testnet/tx/f864b20d7381dfb8ea7661c5c001177aa59787dd93ae87a118fc89adebe22a4b)
- **Stellar Lab Explorer**: [Inspect Staking Contract](https://lab.stellar.org/r/testnet/contract/CDFNCCUHTU3Q2RA4DZQTHONISD32CNTVJ6KKYJFAIENOER7V7DYVQGQA)

### 3. Rewards Distribution Contract (`rewards_distribution.wasm`)
- **Contract ID**: `CBT6BPI6DE2VBIP26XTYGTVLDHYNFB67PPZVHRIJKFHBF33ZYN4PB6CD`
- **WASM Hash**: `211b6c30831e49eca3f82afb1075784d88f28437698cf58c6e5c7c65f007f69e`
- **Deployment Transaction Hash**: `52255ae5e816f3608a973acada74c77d55733878679ea8fa3f2334090d9b2dae`
- **Initialization Transaction Hash**: `79161f913521f5a4a8e769f88e1d3d2627e9b7c0a53114dacb4dc81b59dffa3a`
- **Stellar Expert URL**: [View Deployment Tx](https://stellar.expert/explorer/testnet/tx/52255ae5e816f3608a973acada74c77d55733878679ea8fa3f2334090d9b2dae)
- **Stellar Lab Explorer**: [Inspect Rewards Contract](https://lab.stellar.org/r/testnet/contract/CBT6BPI6DE2VBIP26XTYGTVLDHYNFB67PPZVHRIJKFHBF33ZYN4PB6CD)

---

## 🛠️ Environment Configuration (.env)

```env
VITE_PREDICTION_API_URL=https://api.xpoll-predictor.vercel.app
VITE_NETWORK=testnet
VITE_RPC_URL=https://soroban-testnet.stellar.org
VITE_ORACLE_ADDRESS=CDXDPKE2CKZGGHNYPXQU3LAIIBXSLVWONQBP3Y4A4KOAV3ZUILL33ZRG
VITE_PREDICTION_ADDRESS=CDFNCCUHTU3Q2RA4DZQTHONISD32CNTVJ6KKYJFAIENOER7V7DYVQGQA
VITE_REWARDS_ADDRESS=CBT6BPI6DE2VBIP26XTYGTVLDHYNFB67PPZVHRIJKFHBF33ZYN4PB6CD
```
