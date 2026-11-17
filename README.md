# KieDex Bot

**Versi:** 1.0.0 · **Harga:** Rp 120.000 (~$8) · **Kontak pembelian:** [@rmndkyl](https://t.me/rmndkyl)

Automated bot for KieDex Trade-to-Earn platform. Daily faucet, bonus, social tasks, and trade execution.

## Kebutuhan

| Item | Detail |
|---|---|
| Runtime | Node.js 18+ |
| Wallet | EVM / sesuai chain proyek (kamu sendiri) |
| Proxy | opsional (1 proxy per akun) |
| Captcha | tidak perlu |
| Akses | akun proyek yang kamu kelola sendiri |

## Pembayaran

E-Wallet: DANA / GoPay / ShopeePay · Bank: BCA / Seabank · Crypto: contact for wallet address.
Pembeli menghubungi [@rmndkyl](https://t.me/rmndkyl), kirim bukti transfer, lalu terima license key.

---

🌐 **Website:** https://kiedex.app

## Features

- Daily USDT Faucet Claim (100 USDT)
- Daily OIL Bonus Claim (40 OIL)
- 15 Social Tasks Auto-Complete (Repost, Follow, Join)
- Auto Trade Execution (BTC/USDT futures)
- Multi-Account Support
- Proxy Support (Monosans Free / Private / None)
- Token Auto-Refresh

## Requirements

- Node.js v16+
- Google account signed into KieDex

## Setup

1. Clone this repo
2. Install dependencies:
   ```bash
   npm install
   ```
3. Get your tokens (see below)
4. Run the bot:
   ```bash
   node index.js          # Interactive mode
   node index.js --daily  # Daily auto-run mode
   ```

## Getting Tokens

1. Open https://kiedex.app in Chrome
2. Sign In with Google
3. Open DevTools (F12) → Application → Local Storage → kiedex.app
4. Find the Supabase auth token (key starting with `sb-`)
5. Copy `access_token` and `refresh_token`
6. Run: `node auth.js` and paste the tokens

Alternative (Network tab):
1. Sign in to KieDex
2. DevTools → Network → filter "token"
3. Find request to supabase.co/auth/v1/token
4. Copy tokens from response

## Configuration

Edit `config.json`:
- `delay_min` / `delay_max`: Delay between accounts (ms)
- `retry_count`: Number of retries on failure
- `trade_leverage`: Trade leverage (default: 1x)
- `trade_tp_percent`: Take profit percentage (default: 5%)
- `trade_sl_percent`: Stop loss percentage (default: 2%)

## Proxy Modes

1. Monosans Free Proxy (auto-fetched)
3. No Proxy (direct connection)

## Files

```
kiedex-bot/
├── index.js          # Main entry point
├── auth.js           # Token setup helper
├── config.json       # Configuration
├── tokens.json       # Account tokens (auto-created)
├── src/
│   ├── api.js        # Supabase REST API wrapper
│   ├── auth.js       # Token management
│   └── tasks.js      # Task execution logic
├── utils/
│   ├── banner.js     # LYID banner
│   ├── logger.js     # Colored logger
│   ├── proxy.js      # Proxy manager
│   └── utils.js      # Helpers
└── package.json
```

## Notes

- KieDex uses Supabase backend (PostgreSQL + REST API)
- Auth is Google OAuth via Supabase (standard JWT, no wallet signature needed)
- Wallet connection is for display only, not required for bot operations
- Trade uses demo/testnet USDT + OIL as fee credits
- No captcha required

## Contact

- Telegram: @rmndkyl
- Channel: https://t.me/layerairdrop
- Group: https://t.me/layerairdropdiskusi

## License

Free and open source. Do not believe in the paid version.

## 💰 Harga

| Lisensi | Harga | Fitur |
|---------|-------|-------|
| **Single** | Rp 120.000 / ~$8 | 1 device, lifetime |
| **Bundle (3 bot)** | Rp 120.000 / ~$16 | Pilih 3 bot, hemat 20% |
| **Pro (semua bot)** | Rp 120.000 / ~$70 | Semua bot + update, hemat 30% |

**Cara beli:** Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) di Telegram → /buy

**Bayar pakai:**
- 🇮🇩 DANA / GoPay / ShopeePay / BCA / Seabank
- 🌐 Crypto (USDT/SOL/ETH)

## 🔧 Troubleshooting

| Masalah | Solusi |
|---------|--------|
| `Cannot find module` | Jalankan `npm install` di folder bot |
| `insufficient balance` | Pastikan wallet punya cukup token untuk gas |
| `429 Too Many Requests` | Tunggu 30-60 detik, bot auto-retry |
| Bot diam/tidak jalan | Cek `config.json` — pastikan API key valid |
| License invalid | Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) → /verify |

**Butuh bantuan?** Join [Discord](https://discord.gg/ZK2NVkfSNn) atau chat [@layerairdrop](https://t.me/layerairdrop)
