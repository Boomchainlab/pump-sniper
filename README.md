# 🚀 pump-sniper

**High-performance sniper bot for Pump.fun tokens on Solana**  
Built by [Boomchainlab](https://github.com/Boomchainlab) to empower real-time, automated trading strategies for micro-cap tokens launched via [Pump.fun](https://pump.fun).

---

## 🎯 Overview

`pump-sniper` is a real-time, automated trading system that listens to token launches and volume spikes on Pump.fun, filters them based on customizable strategies, and executes trades instantly using Jupiter Swap and Pump.fun APIs. Designed for high-frequency execution, PnL tracking, and Telegram alerts, this sniper bot gives you a competitive edge in the Solana meme coin ecosystem.

---

## 🧩 Core Features

| Feature                | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| 🔁 Live Trade Listener | Real-time WebSocket feed for Pump.fun token activity                        |
| 🧠 Strategy Engine     | Configurable JSON-based trading strategies (wallets, age, volume, trends)  |
| ⚡ Auto Buy/Sell       | Instant token acquisition + optional auto-sell at profit or % threshold     |
| 🔐 Secure Wallets      | Keypair-based local signing (Ledger/Phantom support planned)                |
| 📊 PnL Logging         | Trade history with timestamp, entry/exit, gas fees, and net returns         |
| 📣 Telegram Alerts     | Bot notifications for executed trades, ROI, and signals                     |
| 🧪 Backtesting Engine  | Replay historical trades and simulate outcomes before deploying live        |
| 🐳 Docker Ready        | Fully containerized for production or headless cloud deployment             |

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Boomchainlab/pump-sniper.git
cd pump-sniper

2. Create a Virtual Environment
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

3. Configure Environment Variables
cp .env.example .env

🚀 Usage

Run the sniper bot
python3 src/main.py
Or use the provided script:
./scripts/run_sniper.sh

Run the backtester
python3 src/backtester.py --strategy config/strategy.json --data backtest/data.json

🧪 Tests
pytest tests/

📣 Telegram Integration

To enable Telegram alerts:
	1.	Create a bot via BotFather
	2.	Add the token and your chat ID to .env
	3.	Enable alerts in config/strategy.json

⸻

🐳 Docker Deployment

Build and run the container:
docker-compose up --build

📈 Roadmap
	•	Multi-wallet support for parallel sniping
	•	Ledger hardware wallet integration
	•	Strategy marketplace UI
	•	Sniper-as-a-Service (SaaS model via Auth0 + dashboard)
	•	Token auto-hold/rebuy strategies
	•	Base chain + Ethereum support

⸻

🤝 Contributing
	1.	Fork the repo
	2.	Create a new feature branch (git checkout -b feat/strategy-rebalancer)
	3.	Commit your changes
	4.	Open a pull request to main

⸻

📫 Support

For technical issues or deployment support, contact:

📧 support@boomchainlab.com
🐦 @BoomchainLabs

⸻

⚠️ Disclaimer

This tool is for educational and research purposes only. Use at your own risk. Boomchainlab is not liable for financial loss, API changes, or unauthorized use.

⸻

Boomchainlab™ – Dominating the DeFi frontier, one block at a time.
