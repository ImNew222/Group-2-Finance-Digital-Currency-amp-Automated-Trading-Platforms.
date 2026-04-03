# 📖 GROUP 2 — STUDY & TASK GUIDE
### Finance Sector: Digital Currency & Automated Trading Platforms

> This guide helps each member understand their part, what to study, and how to prepare for the defense.

---

## 👥 TASK ASSIGNMENTS

| Member | Chapter | Role During Defense | What You'll Present |
|--------|---------|--------------------|--------------------|
| **Mary Grace** | Chapter I: Introduction & Problem Landscape | Agent Grace — Lead Investigator | What Neo-Cebu's finance sector looks like and what threats are coming |
| **Jerimy** | Chapter II: Attack Surface Mapping | Agent Jerimy — Threat Analyst | Where hackers can break into our systems (hardware, software, people) |
| **Ashlee** | Chapter III: Proposed Solution (TitanVault) | Agent Ashlee — Solution Architect | How our 3-pillar defense system works |
| **Mike** | Chapter IV: Implementation Roadmap | Director Mike — Operations Chief | How we deploy TitanVault without shutting anything down |

> **Chapter V (CIA Triad)** = done **together** — each person explains one part.

---

## 📋 WHAT EACH PERSON NEEDS TO STUDY

---

### 🟣 MARY GRACE — Chapter I (The Problem)

**Your job:** Explain *what we're protecting* and *what's attacking us.*

**Key things to memorize:**
1. **Neo-Cebu's 4 financial systems:**
   - CebuCoin (digital currency — like GCash but on blockchain)
   - AutoTrade (AI that buys/sells stocks automatically)
   - Digital Wallets (where people keep their CebuCoin)
   - Smart Contracts (automatic agreements — no paperwork needed)

2. **The 4 Hydra-Pulse threats:**
   - **AI Attacks** — Robot hackers that learn from mistakes and never sleep
   - **Deepfakes** — Fake video/voice calls that look 100% real (remember the Hong Kong $25M example!)
   - **Quantum Threats** — Future super-computers that can break all current passwords/encryption
   - **Social Engineering** — AI-powered scam messages personalized using your social media

**Simple way to remember:**
> *"We have 4 systems to protect, and 4 monster heads trying to destroy them."*

**Practice question the professor might ask:**
> *"Why are 2026 threats different from 2025 threats?"*
> **Your answer:** "Because attackers now use AI that learns and adapts, deepfakes are too realistic for humans to detect, and quantum computers threaten all current encryption."

---

### 🟢 JERIMY — Chapter II (The Weak Spots)

**Your job:** Explain *where* hackers can break in — the doors, windows, and cracks.

**Key things to memorize:**

1. **Hardware vulnerabilities** (physical machines):
   - ATMs can be tampered with (skimming devices)
   - Trading servers can have physical backdoors
   - IoT payment sensors rarely get updated
   - Routers can be hijacked (Man-in-the-Middle)

2. **Software vulnerabilities** (apps and code):
   - Smart contracts can have coding bugs (remember the DAO Hack — $60M lost!)
   - APIs (connections between systems) can be poorly secured
   - AI can be tricked with fake training data (model poisoning)
   - Current encryption (RSA) will break when quantum computers arrive
   - Mobile apps can be reverse-engineered to steal security keys

3. **Human vulnerabilities** (people):
   - AI-powered phishing (super realistic fake emails)
   - Insider threats (angry employees selling access)
   - Deepfake authorization (fake CEO video calls)
   - Weak passwords ("password123")
   - Security fatigue (people ignoring warnings)

**Simple way to remember:**
> *"Three layers of weak spots: the MACHINES, the CODE, and the PEOPLE."*

**Practice question the professor might ask:**
> *"Which layer is the most dangerous?"*
> **Your answer:** "The human layer — 82% of data breaches involve human error. Even the best technology can't help if someone gives away their password."

---

### 🔵 ASHLEE — Chapter III (The Solution)

**Your job:** Explain *how we defend everything* — this is the most technical part, but use the analogies!

**Key things to memorize:**

#### Pillar 1: Post-Quantum Cryptography (PQC)
- **What it is:** New type of encryption that quantum computers CAN'T break
- **Algorithms:** CRYSTALS-Kyber (encrypts data) and CRYSTALS-Dilithium (digital signatures)
- **Analogy:** *"Replacing all our regular locks with locks that even quantum supercomputers can't pick."*

#### Pillar 2: Zero Trust Architecture (ZTA)
- **What it is:** Never trust anyone automatically — verify EVERY TIME
- **4 rules:** Verify explicitly, least privilege, assume breach, micro-segmentation
- **Analogy:** *"A hotel where you show your passport at the elevator, the hallway, AND your door — stealing a key isn't enough."*

#### Pillar 3: Sentinel AI
- **What it is:** Our own AI security guard watching everything 24/7
- **4 powers:** Transaction monitoring, deepfake detection, behavioral biometrics, threat prediction
- **Analogy:** *"A guard who memorized everyone's face, voice, and walking style — even a perfect disguise won't fool it."*

**Simple way to remember:**
> *"Three pillars: Unbreakable LOCKS (PQC), ID checks at every DOOR (Zero Trust), and a smart GUARD watching everything (Sentinel AI)."*

**Practice question the professor might ask:**
> *"What happens if one pillar fails?"*
> **Your answer:** "That's why we have three layers. If PQC is somehow bypassed, Zero Trust still blocks unauthorized access. If Zero Trust fails, Sentinel AI detects the abnormal behavior. All three must fail for an attack to succeed."*

---

### 🟠 MIKE — Chapter IV (The Deployment)

**Your job:** Explain *how we install TitanVault without breaking anything.*

**Key things to memorize:**

#### Phase 1: Preparation (Months 1–3)
- Security audit (full scan of current systems)
- Build a test lab (copy of the real system to experiment on)
- Train all employees on new security rules
- Feed Sentinel AI 2 years of data so it learns what's "normal"

#### Phase 2: Deploy One Layer at a Time (Months 4–8)
- Months 4–5: Upgrade encryption to PQC (run OLD + NEW side by side)
- Months 6–7: Deploy Zero Trust (new ID system for everyone)
- Month 8: Activate Sentinel AI (it's been watching for 5 months already)

#### Phase 3: Full Switch + Testing (Months 9–12)
- Turn off old systems — TitanVault is now primary
- Hire ethical hackers to try to break in (Red Team)
- Simulate worst-case scenario (all 3 pillars attacked at once)
- Publish public report for citizens

**Simple way to remember:**
> *"Three phases: PREPARE (don't touch live systems), DEPLOY (run old + new side by side), TEST (try to break it ourselves)."*

**The key principle to always say:**
> *"The old system and new system run side by side. If anything goes wrong, we fall back instantly. No citizen notices anything."*

**Practice question the professor might ask:**
> *"What if something goes wrong during deployment?"*
> **Your answer:** "We use parallel-run. Both old and new systems run together. If the new system has any issue, we instantly switch back to the old one. Zero downtime."

---

### 🔴 EVERYONE — Chapter V (CIA Triad)

**Each person takes one part + its stress test:**

| Member | CIA Part | Stress Test Scenario |
|--------|----------|---------------------|
| **Mary Grace** | **Confidentiality** — "Only authorized people can see the data" | A hacker steals an employee's password → Zero Trust blocks the device + Sentinel detects wrong typing patterns → account locked ✅ |
| **Jerimy** | **Integrity** — "Nobody can change data without permission" | A hacker edits a smart contract → PQC signature breaks → blockchain rejects it → Sentinel alerts team ✅ |
| **Ashlee** | Full **TitanVault summary** — "Three pillars working together" | Wrap-up: explain how all 3 pillars protect all 3 CIA principles |
| **Mike** | **Availability** — "The system is always running" | A DDoS attack floods AutoTrade → Sentinel filters traffic → micro-segmentation isolates it → backup servers take over ✅ |

---

## ⏱️ PRESENTATION TIMING (7 Minutes Total)

| Time | Who | What |
|------|-----|------|
| 0:00–1:30 | Mary Grace | Act I — the threats |
| 1:30–3:00 | Jerimy | Act II — the weak spots |
| 3:00–4:30 | Ashlee | Act III — TitanVault solution |
| 4:30–5:30 | Mike | Act IV — deployment plan |
| 5:30–7:00 | Everyone | Act V — CIA Triad + stress tests |

---

## 🧠 STUDY TIPS

1. **Read your chapter in the script** (`NEO_CEBU_SCRIPT.md`) — it's written like a movie, so it's easier to remember
2. **Memorize the analogies** — when the professor asks something hard, use the simple comparisons
3. **Know your stress test** — the Q&A will probably include "what if this gets attacked?" scenarios
4. **Know your neighbor's chapter** — at least understand the basics of the chapter before and after yours
5. **Practice transitions** — when Mary Grace finishes, she says *"Jerimy, tell us where the weak spots are"* etc.

---

## 🗂️ FILES OVERVIEW

| File | What it's for |
|------|--------------|
| `ACTIVITY.md` | Project tracker with deadlines |
| `NEO_CEBU_SCRIPT.md` | Movie-script version — read this to learn your part |
| `Group2_Finance_FinalProject.docx` | The formal manuscript to submit |
| `GUIDE.md` | This file — task assignments and study guide |
