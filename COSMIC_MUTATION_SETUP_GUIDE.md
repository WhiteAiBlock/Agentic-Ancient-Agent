# 🌌 COSMIC MUTATION ENGINE: COMPLETE SETUP GUIDE

## ♾️ Autonomous Evolution with Free Ollama + Claude Code

---

## 🎯 WHAT YOU'RE GETTING

**A fully autonomous agent** that:
- ✅ Runs **every 2 hours** on GitHub Actions
- ✅ Uses **Ollama (FREE)** instead of paid Claude API
- ✅ Applies **genetic algorithm mutations** to your code
- ✅ Sends **Telegram consent buttons** for approval
- ✅ Integrates with your **existing infrastructure** (Helius, Solana, Wormhole)
- ✅ **Never stops improving** your Empire codebase

---

## 📦 INSTALLATION

### Step 1: Add the Skill
1. Download `cosmic-mutation-engine.skill`
2. Import into your Claude environment
3. Extract contents if needed

### Step 2: Add GitHub Workflow
1. Copy `cosmic-mutation.yml` to `.github/workflows/` in your repo
2. Commit and push

```bash
mkdir -p .github/workflows
cp cosmic-mutation.yml .github/workflows/
git add .github/workflows/cosmic-mutation.yml
git commit -m "🧬 Add autonomous mutation engine"
git push
```

### Step 3: Configure GitHub Secrets
Go to your repo → Settings → Secrets and variables → Actions

**Your existing secrets** (already configured):
- ✅ `HELIUS_API_KEY`
- ✅ `TELEGRAM_BOT_TOKEN`
- ✅ `TELEGRAM_CHAT_ID`
- ✅ `SOLANA_RPC`
- ✅ `WORMHOLE_ENV`
- ✅ `PRIMARY_WALLET`
- ✅ (all others from your current workflow)

**No new secrets needed!** The workflow uses Ollama (free, no API keys).

### Step 4: Enable GitHub Actions
1. Go to your repo → Actions tab
2. Click "I understand my workflows, go ahead and enable them"
3. Find "Cosmic Mutation Engine" workflow
4. Click "Run workflow" to test manually

---

## 🦙 HOW OLLAMA MAKES IT FREE

### Traditional Claude Code (Paid)
```bash
# Costs $100-200/month
export ANTHROPIC_API_KEY="sk-ant-..."
claude --model claude-opus-4-5 "write code"
```

### With Ollama (FREE)
```bash
# Zero cost, runs locally or on free cloud tier
export ANTHROPIC_AUTH_TOKEN="ollama"
export ANTHROPIC_BASE_URL="http://localhost:11434"
claude --model qwen3-coder:480b-cloud "write code"
```

**Models Used:**
- **Primary**: `qwen3-coder:480b-cloud` (Ollama's free cloud tier)
- **Fallback**: `gpt-oss:20b` (local model, completely free)

Both are top-tier coding models, nearly as capable as Claude Opus for most tasks.

---

## 🔔 TELEGRAM CONSENT BUTTONS

### How It Works

**When a mutation is proposed**, you get a Telegram message:

```
🧬 Autonomous Mutation Proposal

ID: a3f2d901
Type: optimization
Risk: low
Fitness Gain: +15.3%

Description:
Cache Helius API responses to reduce rate
limiting. Adds Redis-compatible caching layer.

Files Affected: 3
Lines Changed: +45/-12

⚠️ Auto-apply in 1 hour if not responded

┌─────────────────┬─────────────┐
│  ✅ Approve     │  ❌ Reject  │
├─────────────────┼─────────────┤
│  ℹ️ Details    │  ⏸️ Defer   │
└─────────────────┴─────────────┘
```

**Your options:**
1. **✅ Approve**: Mutation applied immediately
2. **❌ Reject**: Mutation discarded
3. **ℹ️ Details**: Get full diff and analysis
4. **⏸️ Defer**: Skip this run, may appear again
5. **Ignore**: Low-risk mutations auto-apply after 1 hour

### Risk Levels

**Low Risk** (auto-approved after 1 hour):
- Type hints
- Error handling
- Code comments
- Performance optimizations
- Caching

**Medium Risk** (requires approval):
- API integrations
- File structure changes
- New dependencies

**High Risk** (always requires approval):
- Breaking changes
- Security-sensitive code
- Database schema changes

---

## ⚙️ GITHUB ACTIONS WORKFLOW

### What Happens Every 2 Hours

```
1. 🔄 Checkout your repository
2. 🐍 Setup Python 3.11
3. 📦 Install dependencies (from requirements.txt)
4. 🦙 Install Ollama service
5. 📥 Pull AI models (qwen3-coder:480b-cloud, gpt-oss:20b)
6. 🔧 Install Claude Code CLI
7. 🧬 Initialize Helix Nexus (scan skills)
8. 🔍 Run your cosmic scan (existing main.py)
9. 💡 Generate mutation proposals (genetic algorithm)
10. ⚡ Execute Claude Code mutations (Ollama backend)
11. 🧪 Validate changes (syntax, tests)
12. 📊 Generate mutation report
13. 🔔 Send Telegram notification with consent buttons
14. 💾 Upload artifacts (reports, logs)
15. 🌐 Update webapp status (your Replit URLs)
```

**On manual runs**: Changes are committed after approval.
**On scheduled runs**: Artifacts uploaded, manual merge required.

---

## 🧬 GENETIC ALGORITHM DETAILS

### Multi-Objective Fitness Function

Each mutation scored on 5 dimensions:

1. **Efficiency** (25%): Speed, memory, resource usage
2. **Security** (20%): Error handling, input validation
3. **Yield** (25%): Value generation, ROI, blockchain gains
4. **Diversity** (15%): Novel approaches, creativity
5. **Truthfulness** (15%): Correctness, test coverage

### Evolution Process

```
Generation 0: Current codebase
    ↓
Mutation Operators:
  • Point Mutation (random small changes)
  • Crossover (combine best traits)
  • Insertion (add proven patterns)
  • Deletion (remove cruft)
    ↓
Evaluate Fitness → Select Top 50%
    ↓
Breed Next Generation
    ↓
Repeat for 5 generations
    ↓
Best Variant → Propose to User
```

**Population Size**: 10 variants per generation
**Generations**: 5 per run
**Selection**: Top 50% survival rate

---

## 🔐 SAFETY MECHANISMS

### Multiple Safety Layers

1. **Syntax Validation**: All Python files checked before commit
2. **Test Execution**: Existing tests must pass
3. **Backwards Compatibility**: Breaking changes rejected
4. **Manual Approval Gate**: Scheduled runs don't auto-commit
5. **Artifact Preservation**: All mutations saved for 30 days
6. **Git History**: Easy rollback with `git revert`
7. **Risk Classification**: High-risk changes always need approval

### What Gets Mutated

**Allowed:**
- ✅ Performance optimizations
- ✅ Error handling improvements
- ✅ Code documentation
- ✅ Type hints
- ✅ Caching layers
- ✅ API efficiency
- ✅ Test coverage

**Blocked:**
- ❌ Removing features
- ❌ Changing public APIs
- ❌ Modifying secrets
- ❌ Deleting tests
- ❌ Breaking dependencies

---

## 📊 MONITORING & REPORTS

### Telegram Notifications

**Every run** (success or failure):
```
🧬 Cosmic Mutation Complete

⚡ Run: #42
🤖 Model: qwen3-coder:480b-cloud
🔄 Mutations: 7
⏰ Time: 2026-02-05T18:00:00Z

🌌 Helix eternal. Empire compounds.
```

### GitHub Artifacts

**Download after each run:**
- `MUTATION_REPORT.json` - Full metrics and stats
- `MUTATION_LOG.md` - Human-readable changelog
- `claude-mutations.log` - Raw Claude Code output
- `cosmic-state.json` - Blockchain state snapshot
- `mutation-proposals.json` - All GA proposals
- `genetic-mutations.json` - Detailed mutation analysis

### WebApp Status

Real-time updates sent to both your Replit URLs:
```json
{
  "type": "autonomous_mutation",
  "timestamp": "2026-02-05T18:00:00Z",
  "data": {
    "run_number": 42,
    "model": "qwen3-coder:480b-cloud",
    "mutations": 7,
    "status": "complete"
  }
}
```

---

## 🎛️ CONFIGURATION OPTIONS

### Change Run Schedule

Edit `.github/workflows/cosmic-mutation.yml`:

```yaml
on:
  schedule:
    # Every 2 hours (default)
    - cron: '0 */2 * * *'
    
    # Every 4 hours
    # - cron: '0 */4 * * *'
    
    # Every 6 hours
    # - cron: '0 */6 * * *'
    
    # Daily at midnight
    # - cron: '0 0 * * *'
    
    # Hourly (aggressive!)
    # - cron: '0 * * * *'
```

### Use Different Models

```yaml
env:
  # For better code quality (still free)
  MUTATION_MODEL: deepseek-coder:33b
  FALLBACK_MODEL: codellama:13b
  
  # For faster runs (still free)
  MUTATION_MODEL: qwen3-coder:32b
  FALLBACK_MODEL: phi:14b
```

### Adjust Risk Tolerance

Edit `scripts/mutation_consent.py`:

```python
# Auto-approve timeout (default: 1 hour)
AUTO_APPROVE_TIMEOUT = 2  # hours

# Which risks need approval (default: high only)
REQUIRE_APPROVAL_FOR = ['high', 'medium']  # or just ['high']
```

---

## 🔧 LOCAL TESTING

### Test Ollama Setup
```bash
# Install Ollama
curl -fsSL https://ollama.com/install.sh | sh

# Pull models
ollama pull qwen3-coder:480b-cloud
ollama pull gpt-oss:20b

# Verify
ollama list
```

### Test Claude Code Integration
```bash
# Setup environment
python3 scripts/ollama_integration.py setup

# Run a mutation
python3 scripts/ollama_integration.py mutate \
  --prompt "Add error handling to API calls"
```

### Test Telegram Consent
```bash
# Send test proposal
python3 scripts/mutation_consent.py propose \
  --type optimization \
  --description "Test mutation" \
  --risk low

# Check status
python3 scripts/mutation_consent.py check --mutation-id <id>
```

---

## 🚀 FIRST RUN

### Manual Test Run

1. Go to GitHub → Actions
2. Select "Cosmic Mutation Engine"
3. Click "Run workflow"
4. Wait ~10 minutes
5. Check Telegram for consent request
6. Review artifacts in GitHub

### Expected Output

**Telegram message**:
```
🧬 Autonomous Mutation Proposal

ID: abc123
Type: optimization
Risk: low
...
```

**GitHub Artifacts**:
- mutation-reports-1.zip

**WebApp Update**:
- Status POST to your Replit URLs

---

## 🔥 ADVANCED FEATURES

### Custom Mutation Strategies

Create `.mutations/strategy.json`:
```json
{
  "focus_areas": [
    "blockchain_optimization",
    "api_efficiency",
    "error_resilience"
  ],
  "fitness_weights": {
    "efficiency": 0.3,
    "yield": 0.4,
    "security": 0.3
  },
  "allowed_mutations": [
    "caching",
    "batching",
    "retry_logic"
  ]
}
```

### Integration with Existing CI/CD

The workflow integrates seamlessly:
```yaml
# Your existing workflow
- name: Run tests
  run: pytest

# Cosmic mutation workflow runs separately
# but respects the same test suite
```

---

## ❓ TROUBLESHOOTING

### Workflow Not Running

**Check:**
1. GitHub Actions enabled in repo settings
2. Workflow file in `.github/workflows/`
3. No syntax errors in YAML
4. Secrets configured correctly

**Fix:**
```bash
# Validate workflow
cat .github/workflows/cosmic-mutation.yml | yq .
```

### Ollama Installation Fails

**On GitHub Actions:**
- Usually auto-resolved (retry after 30s)
- Check Actions logs for specific error

**Locally:**
```bash
# Linux/Mac
curl -fsSL https://ollama.com/install.sh | sh

# Windows
# Download from ollama.com/download
```

### Claude Code Not Found

**Check PATH:**
```bash
echo $PATH | grep .local/bin
```

**Add to PATH:**
```bash
export PATH="$HOME/.local/bin:$PATH"
```

### Telegram Not Receiving Messages

**Verify:**
```bash
# Test Telegram bot
curl "https://api.telegram.org/bot${TELEGRAM_BOT_TOKEN}/getMe"

# Test send message
curl -X POST "https://api.telegram.org/bot${TELEGRAM_BOT_TOKEN}/sendMessage" \
  -d "chat_id=${TELEGRAM_CHAT_ID}" \
  -d "text=Test"
```

---

## 📚 RESOURCES

### Files Included
- `cosmic-mutation-engine.skill` - Complete skill package
- `cosmic-mutation.yml` - GitHub Actions workflow
- `scripts/ollama_integration.py` - Free Claude Code setup
- `scripts/mutation_consent.py` - Telegram approval system

### External Links
- [Ollama Documentation](https://ollama.com/docs)
- [Claude Code Guide](https://github.com/anthropics/claude-code)
- [GitHub Actions Docs](https://docs.github.com/en/actions)
- [Telegram Bot API](https://core.telegram.org/bots/api)

---

## 🌌 FINAL WORDS

You now have a **truly autonomous agent** that:
- Runs **24/7 without human intervention**
- Uses **free Ollama models** (no API costs)
- **Improves your code** using genetic algorithms
- **Asks permission** via Telegram when needed
- **Integrates seamlessly** with your existing stack

**This is not just automation. This is evolution.**

---

**Helix eternal. Empire compounds. Autonomy infinite.** 🧬🦙⚡

---

*Questions? Check the skill documentation or run mutation engine locally first.*
