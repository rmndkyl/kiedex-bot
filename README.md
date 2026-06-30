# KieDex Auto Bot

Automated bot for **KieDex** Trade-to-Earn platform — daily faucet, social tasks, and trade execution.

## Features

- 🚰 Daily USDT Faucet Claim (100 USDT)
- ⛽ Daily OIL Bonus Claim (40 OIL)
- 📋 15 Social Tasks Auto-Complete (Repost, Follow, Join)
- 📈 Auto Trade Execution (BTC/USDT futures, 1x-50x leverage)
- 👥 Multi-Account Support
- 🌐 Proxy Support (Monosans Free / Private / None)
- 🔄 Token Auto-Refresh (Supabase JWT)
- ⏰ Daily Auto-Run Mode (`--daily`)

## How It Works

KieDex uses Supabase backend with Google OAuth authentication. The bot:
1. Refreshes expired tokens automatically
2. Claims daily USDT faucet (100 USDT testnet)
3. Claims daily OIL bonus (40 OIL trading fuel)
4. Completes all 15 social tasks (Twitter repost, CMC follow, Discord/Telegram join, etc.)
5. Executes a BTC/USDT long trade with calculated TP/SL
6. Repeats daily

## Requirements

- Node.js v16+
- Google account signed into [KieDex](https://kiedex.app)

## Setup

```bash
git clone https://github.com/layerairdrop/kiedex-bot.git
cd kiedex-bot
npm install
node auth.js      # Add your account tokens
node index.js     # Run the bot
```

## Getting Tokens

1. Open https://kiedex.app → Sign In with Google
2. DevTools (F12) → Application → Local Storage → kiedex.app
3. Copy `access_token` and `refresh_token` from Supabase auth
4. Run `node auth.js` and paste tokens

## Proxy Modes

| Mode | Description |
|------|-------------|
| Monosans | Free proxies (auto-fetched) |
| Private | Your own proxies in proxy.txt |
| None | Direct connection |

## Pricing

| Plan | Price |
|------|-------|
| Single License | $5 / Rp 80.000 |
| Bundle (3 scripts) | Rp 155.000 (20% off) |
| Pro Bundle (all scripts) | Rp 370.000 (30% off) |

## Purchase

Contact [@rmndkyl](https://t.me/rmndkyl) on Telegram.

**Payment Methods:**
- **E-Wallet (ID):** DANA / GoPay / ShopeePay
- **Bank Transfer (ID):** BCA / Seabank
- **Crypto (USDT/SOL):** Contact for wallet address
- EVM + Solana wallets (ask for address)

## Other Scripts

| Bot | Project | Price |
|-----|---------|-------|
| canopy-bot | Canopy Network | $5 / Rp 80K |
| simplechain-bot | SimpleChain | $4 / Rp 65K |
| watt2trade-bot | Watt2Trade | $4 / Rp 65K |
| uponly-bot | UpOnly | $6 / Rp 95K |
| afyniti-bot | Afyniti | $4 / Rp 65K |
| orbition-bot | Orbition Network | $4 / Rp 65K |
| unicity-bot | Unicity Network | $6 / Rp 95K |
| **kiedex-bot** | **KieDex** | **$5 / Rp 80K** |

**Bundle Pricing:**
- Starter (3 pick): Rp 155.000 (20% off)
- Pro (all 8): Rp 370.000 (30% off)
- VIP (monthly access): Rp 200.000/bulan

## Contact

- Telegram: [@rmndkyl](https://t.me/rmndkyl)
- Channel: [@layerairdrop](https://t.me/layerairdrop)
- Group: [@layerairdropdiskusi](https://t.me/layerairdropdiskusi)
- GitHub: [github.com/rmndkyl](https://github.com/rmndkyl)

## Disclaimer

This bot is for educational purposes. Use at your own risk. The author is not responsible for any losses.
