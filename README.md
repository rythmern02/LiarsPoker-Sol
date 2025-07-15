# 🃏 Liars Poker: The On-Chain Bluffing Game

**Bluff. Bid. Win — or get exposed. A fully on-chain bluff-based strategy game on Solana.**  
Built using **Solana + Anchor + Next.js + TailwindCSS**. Powered by **truth... or lies.**

![Liars Poker Banner](https://raw.githubusercontent.com/rythmern02/Liarspoker-Sol/main/public/banner.jpg)

---

## 🌍 Live Demo

🔗 [liars-poker-sol.vercel.app](https://liars-poker-sol.vercel.app)

---

## 🎯 About the Game

**Liars Poker** is a multiplayer bluffing game where players stake SOL, receive hidden cards, and battle through psychological warfare — making increasing digit-count bids or calling out lies.

All interactions, rules, outcomes, and rewards are enforced **entirely on-chain** using **Anchor smart contracts** for maximum fairness.

---

## 🧩 Game Flow

1. 🔗 Connect your Solana wallet (Phantom, Backpack, etc.)
2. 🏁 Create or join a game lobby
3. 🎴 Receive secret cards (on-chain generated)
4. 🗣️ Start bidding how many of a digit exist in total
5. 📈 Raise the bid — or ❌ Call the bluff
6. ✅ Smart contract validates, winner claims the round

---

## ⚙️ Tech Stack

| Layer          | Tech                                             |
|----------------|--------------------------------------------------|
| Frontend       | `Next.js`, `React`, `TailwindCSS`, `TypeScript` |
| Wallet         | `@solana/wallet-adapter`                         |
| Blockchain     | Solana Devnet / Mainnet-ready                    |
| Smart Contract | `Anchor` framework (Rust)                        |
| State Mgmt     | Custom Hooks + `@solana/web3.js`                |

---

## ✨ Features at a Glance

| 🔹 Feature                 | 💬 Description                                          |
|--------------------------|--------------------------------------------------------|
| 🎴 Secret Cards           | Assigned on-chain, tamper-proof                        |
| 🧠 Bluffing Logic         | Turn-based bid/challenge mechanism                     |
| ⚖️ On-chain Fairness      | Fully validated using Anchor smart contracts           |
| 💰 Stake & Win            | SOL wagering (optional but rewarding)                  |
| ⚡ Real-time Updates      | Live game state sync via hooks                         |
| 📱 Responsive UI          | Mobile-first + beautiful animations                    |
| 🔐 Game Security          | Verified logic + turn locks + disconnect handling      |

---

## 🖼️ Screenshots

| Homepage | Game Lobby | In-Game |
|----------|-------------|---------|
| ![Home](https://raw.githubusercontent.com/rythmern02/LiarsPoker-Sol/main/public/home.png) | ![Lobby](https://raw.githubusercontent.com/rythmern02/LiarsPoker-Sol/main/public/lobby.png) | ![Game](https://raw.githubusercontent.com/rythmern02/LiarsPoker-Sol/main/public/game.png) |

---

## 🔗 Programs

Programs written in Rust, powered by **Anchor**:
- Deterministic state with PDAs
- Secure transitions between turns
- Random-ish card logic (for now!)
- Upgradeable & multiplayer-ready

🧠 Source: [`/programs/liars_poker/src/lib.rs`](./programs/liars_poker/src/lib.rs)

---

## 🗂️ Folder Structure

/app
/components → Modular UI (cards, players, HUD)
/pages → Next.js routes
/hooks → Game state, contract interactions
/utils → Anchor client + Solana helpers
/styles → Tailwind theme

/programs
/liars_poker → Anchor smart contract (Rust)

tests/ → Anchor Mocha test suite


---

### 🛠️ Local Setup

To get started with Liars Poker locally, follow these steps:

1. **📦 Install Dependencies**

   ```
   pnpm install
   ```

2. **🔧 Configure Solana**

   ```
   solana config set --url devnet
   anchor build
   anchor deploy
   ```

3. **🧪 Launch Frontend**

   ```
   pnpm dev
   ```

### 🧪 Game Add-ons Coming Soon

We're constantly working on new features and game modes:

* 🎲 Heads or Tails (quick-fire staking)

* 🎲 Dice Predictions

* 🃏 NFT-based Poker Showdowns

* 📈 Prediction Markets

* 🏆 On-chain Leaderboards & Token Rewards

### 🔐 Security & UX

Our focus is on a secure and user-friendly experience:

* 🧷 Button lockouts per turn

* 🔌 Wallet reconnect/resume state

* 🧪 On-chain validation before render

* 🔔 Animated toasts & error feedback

### 🤝 Contributing

We're open to contributions! Add game modes, improve UX, or help with audits.

```
git clone [https://github.com/YOUR_GITHUB_USERNAME/liars-poker-sol.git](https://github.com/YOUR_GITHUB_USERNAME/liars-poker-sol.git)
cd liars-poker-sol
```

📖 See `CONTRIBUTING.md` to get started.

### 👥 Credits

Built with ❤️ by @YourTwitterHandle
Inspired by game theory, Web3, and every bluff ever called.

### 📜 License

MIT License © 2025

### 🚀 Spread the Word

If you loved it —

* 🌟 Star the repo

* 🍴 Fork it

* 🔁 Share on Farcaster, Lens, or Twitter
