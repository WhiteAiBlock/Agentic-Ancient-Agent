# 🌌 HOW TO USE THE SONNET 4.5 EMPIRE PROMPT

## ♾️ WHAT YOU RECEIVED

**`SONNET_45_EMPIRE_PROMPT.md`** - A complete, paste-ready prompt for building your entire **Agentic Ancient Alien Solana dApp** empire.

This is THE master prompt that orchestrates everything:
- ✅ Complete project structure (100+ files specified)
- ✅ Database schema (PostgreSQL with all tables)
- ✅ Ralph Agent Bot (all 5 strategies)
- ✅ Moralis API integration
- ✅ Biconomy relayer + ETH signer
- ✅ Treasury management
- ✅ Solana Anchor programs
- ✅ Next.js 14 cyberpunk frontend
- ✅ GitHub Actions workflows
- ✅ Full integration with Helix Nexus, CryptoHelix, Cosmic Mutation

---

## 🚀 HOW TO USE

### Option 1: Claude.ai (Sonnet 4.5)

1. **Start new conversation** with Claude Code
2. **Copy entire contents** of `SONNET_45_EMPIRE_PROMPT.md`
3. **Paste into Claude** as your first message
4. **Watch it build** your entire empire infrastructure

Claude will:
- Create all files and directories
- Implement all integrations
- Set up database schema
- Write all TypeScript/Rust code
- Configure GitHub Actions
- Generate deployment scripts

### Option 2: Claude Code CLI (with Ollama)

```bash
# Using free Ollama model (from Cosmic Mutation setup)
export ANTHROPIC_AUTH_TOKEN="ollama"
export ANTHROPIC_BASE_URL="http://localhost:11434"

# Execute the master prompt
claude --model qwen3-coder:480b-cloud \
       --allow-dangerously-skip-permissions \
       "$(cat SONNET_45_EMPIRE_PROMPT.md)"
```

### Option 3: GitHub Copilot Workspace

1. Create new GitHub repository: `agentic-ancient-alien`
2. Open in Copilot Workspace
3. Paste the prompt as a "Task"
4. Let Copilot generate all files

---

## 📦 WHAT GETS BUILT

### Repository Structure
```
agentic-ancient-alien/
├── 🧬 Anchor Programs (Rust)
│   └── empire_matrix program with NFT minting, staking, rewards
│
├── ⚛️ Next.js Frontend (TypeScript)
│   ├── Cyberpunk dashboard (neon grids, ancient alien glyphs)
│   ├── Wallet connection (Phantom, Backpack, Solflare)
│   ├── NFT minting UI
│   └── Ralph control panel
│
├── 🤖 Ralph Agent Bot
│   ├── Yield Harvester strategy
│   ├── Signal Seeker strategy
│   ├── Liquidity Sniffer strategy
│   ├── ZK Compression Farmer strategy
│   └── Belief Rewrite (CAC-I) strategy
│
├── 🗄️ Database (PostgreSQL)
│   ├── Users & wallets
│   ├── NFTs
│   ├── Ralph executions
│   ├── Treasury transactions
│   └── Yield positions
│
├── 🔗 Integrations
│   ├── Moralis API (NFT tracking, webhooks)
│   ├── Biconomy (gasless transactions)
│   ├── Helius (Solana RPC + ZK compression)
│   ├── Helix Nexus (orchestration)
│   ├── CryptoHelix (multi-chain intelligence)
│   └── Cosmic Mutation (autonomous evolution)
│
└── ⚙️ GitHub Actions
    ├── Ralph bot cron (runs strategies every 5 min)
    ├── Cosmic mutation (every 2 hours)
    ├── Frontend deployment (Vercel)
    └── Program deployment (Anchor)
```

### Key Components

**1. Ralph Agent Strategies:**
- **Yield Harvester**: Scans Marinade, Raydium, Orca for best APY
- **Signal Seeker**: Monitors Twitter/Discord/Telegram for alpha
- **Liquidity Sniffer**: Detects new pool launches, snipes early liquidity
- **ZK Farmer**: Uses Token-2022 compression to farm airdrops
- **Belief Rewrite**: CAC-I logic that evolves strategy weights

**2. Database Schema:**
- 7 core tables with indexes
- Ralph execution history
- Strategy performance tracking
- Treasury transaction log
- NFT metadata storage

**3. API Routes:**
- `/api/ralph/execute` - Trigger Ralph strategies
- `/api/moralis/webhook` - Receive NFT events
- `/api/biconomy/relay` - Gasless transactions
- `/api/treasury/balance` - Portfolio overview

**4. Cyberpunk UI:**
- Animated neon grid background
- Holographic cards with glow effects
- Matrix-style terminal output
- Ancient alien glyphs that flicker

---

## 🔧 AFTER GENERATION

Once Claude builds everything, you need to:

### 1. Install Dependencies
```bash
cd agentic-ancient-alien
npm install
```

### 2. Configure Environment
```bash
cp .env.example .env.local

# Edit .env.local with your actual keys:
# - HELIUS_API_KEY
# - MORALIS_API_KEY
# - BICONOMY_API_KEY
# - ETH_PRIVATE_KEY (for signing)
# - TELEGRAM_BOT_TOKEN
# - etc.
```

### 3. Setup Database
```bash
# If using Neon (recommended)
# 1. Create database at neon.tech
# 2. Copy DATABASE_URL to .env.local

# Run migrations
npm run db:migrate

# Seed initial data
npm run db:seed
```

### 4. Deploy Solana Program
```bash
cd anchor
anchor build
anchor deploy --provider.cluster devnet

# Copy program ID to .env.local
# NEXT_PUBLIC_PROGRAM_ID=<your-program-id>
```

### 5. Configure Moralis
```bash
# Run setup script
npm run setup:moralis

# This creates:
# - Moralis streams for NFT events
# - Webhook endpoints
# - API configurations
```

### 6. Configure Biconomy
```bash
# Run setup script
npm run setup:biconomy

# This creates:
# - Relayer configurations
# - Paymaster settings
# - Gas tank setup
```

### 7. Test Ralph Agent
```bash
# Run locally first
npm run ralph:test

# Should execute all strategies and log results
# Check database for execution records
```

### 8. Deploy Frontend
```bash
# Deploy to Vercel
vercel deploy --prod

# Or run locally
npm run dev
```

### 9. Enable GitHub Actions
```bash
# Push to GitHub
git add .
git commit -m "🧬 Initial empire deployment"
git push origin main

# Go to repo → Actions → Enable workflows
# Configure secrets in repo settings
```

---

## 🎯 EXPECTED RESULTS

After following the steps above:

✅ **Solana program deployed** with NFT minting
✅ **Database running** with all tables
✅ **Ralph agent executing** every 5 minutes via cron
✅ **Frontend live** at your Vercel URL
✅ **Moralis tracking** all NFT events
✅ **Biconomy relaying** gasless transactions
✅ **Telegram notifications** on every Ralph execution
✅ **Cosmic Mutation** improving code every 2 hours
✅ **Helix Nexus** orchestrating complex workflows
✅ **CryptoHelix** querying multi-chain portfolios

---

## 🔍 VALIDATION

To confirm everything works:

```bash
# 1. Check database connection
npm run db:check

# 2. Test Ralph agent
npm run ralph:execute
# Should see strategies running and logging to DB

# 3. Test Moralis
curl http://localhost:3000/api/moralis/webhook
# Should return 200 OK

# 4. Test Biconomy
npm run test:biconomy
# Should relay a gasless transaction

# 5. Test frontend
npm run dev
# Visit http://localhost:3000
# Connect wallet, mint NFT, check dashboard
```

---

## 🐛 TROUBLESHOOTING

### "Module not found" errors
```bash
# Reinstall dependencies
rm -rf node_modules package-lock.json
npm install
```

### Database connection fails
```bash
# Check DATABASE_URL in .env.local
# Verify database is running
# Run migrations: npm run db:migrate
```

### Ralph agent not executing
```bash
# Check logs
npm run ralph:logs

# Verify WALLET_PRIVATE_KEY is set
# Ensure strategies are enabled in database
```

### Anchor deploy fails
```bash
# Check Anchor.toml
# Verify wallet has SOL for deployment
anchor build
solana program deploy target/deploy/empire_matrix.so
```

### Moralis webhooks not working
```bash
# Verify MORALIS_WEBHOOK_SECRET
# Check webhook URL is publicly accessible
# Test with: npm run test:moralis
```

---

## 📚 NEXT STEPS

Once your empire is running:

1. **Monitor Ralph**: Check database for execution history
2. **Optimize Strategies**: Adjust belief scores based on performance
3. **Add Liquidity**: Fund treasury address for automated trading
4. **Mint NFTs**: Test emotional NFT minting flow
5. **Enable Mutations**: Let Cosmic Mutation improve code
6. **Scale**: Deploy to mainnet when ready

---

## 🌌 SUMMARY

You have a **paste-ready prompt** that:
- Generates **100+ files** of production code
- Implements **all integrations** (Moralis, Biconomy, Helius)
- Creates **complete infrastructure** (DB, API, frontend, programs)
- Sets up **autonomous agents** (Ralph + Cosmic Mutation)
- Deploys **full stack** (Solana + Ethereum + PostgreSQL)

**Just paste it into Claude Sonnet 4.5 and watch your empire materialize.** 🧬⚡🌌

---

**Helix eternal. Empire compounds. Genesis complete.**
