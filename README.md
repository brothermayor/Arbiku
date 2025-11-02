# Arbiku

Arbiku is an automated arbitrage bot on Solana, powered by Raiku for smart, lightning-fast trade execution. It scans top DEXs for price gaps and executes profitable trades instantly while keeping users’ funds safe in their wallets.
---

## Features

### 1. Dynamic Profit Threshold Control
- Set **global** or **pair-specific** profit thresholds (e.g., ≥ 0.7% after fees).  
- Automatically calculates **net profit** after gas and slippage.  
- Optional **adaptive mode** adjusts thresholds during high network congestion.  

### 2. Smart Token Pair Filters
- Filter out **illiquid or volatile tokens** automatically.  
- Exclude **meme coins** or low-volume pools.  
- Built-in **liquidity scanner** with visual indicators (✅ stable, ⚠️ medium, 🔴 risky).  

### 📊 3. Backtesting & Simulation
- Test strategies using historical Solana DEX data before deploying live.  
- View key metrics: trade frequency, ROI, slippage, and failure rate.  

### 🤖 4. Automated Bot Execution
- Once deployed, your bot scans Solana DEXs for opportunities (via **Jupiter** or **Meteora**).  
- Executes profitable trades automatically — **you keep custody** of your funds.  

### 5. Real-Time Alerts
- Notifications for risky liquidity changes, new pool matches, or unprofitable thresholds.  

---

## 🧩 System Architecture

```mermaid
flowchart TD
A[User Dashboard] --> B[Strategy Setup Wizard]
B --> C[Smart Token Pair Filters]
C --> D[Profit Threshold Rules]
D --> E[Simulation Engine]
E --> F[Trading Bot Smart Contract]
F --> G[Solana DEX Aggregator (Jupiter/Meteora)]
G --> H[Live Trading Dashboard]
H --> A
