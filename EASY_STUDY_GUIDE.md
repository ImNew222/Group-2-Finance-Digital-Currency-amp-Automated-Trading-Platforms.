# 📚 EASY STUDY GUIDE — Group 2: Finance Sector
### Read this to understand EVERYTHING in our project, in plain simple language.

> **No acting needed.** Just read, understand, and you'll be ready to present and answer any question the professor throws at you.

---

## 🧠 THE BIG PICTURE (In One Paragraph)

Our project is about protecting **Neo-Cebu's money systems** (digital currency + automated stock trading) from **4 types of modern cyber attacks**. We designed a defense system called **"Project TitanVault"** that combines 3 technologies: **unbreakable encryption**, **strict access control**, and **an AI security guard**. We also planned how to install it over 12 months without shutting anything down, and proved it works by testing it against attack scenarios.

**That's it.** Everything below is just the details.

---

# CHAPTER I — What's The Problem?

## What is Neo-Cebu?

Neo-Cebu is a **fictional futuristic version of Cebu City in 2026** where everything is digital. People don't use much cash anymore — they use:

| System | What It Is (Simple) |
|--------|-------------------|
| **CebuCoin** | Like GCash, but built on blockchain technology |
| **AutoTrade** | A robot that buys and sells stocks for you — super fast |
| **Digital Wallets** | An app on your phone where you keep your CebuCoin |
| **Smart Contracts** | Agreements that execute automatically (like: "if payday, send salary to employee automatically") |

**Why does this matter?** Because if hackers break these systems, people can't buy food, can't get paid, and the city's economy stops.

---

## The 4 Threats (Hydra-Pulse)

Think of **Hydra-Pulse** as a monster with 4 heads — each head is a different way hackers can attack:

### 🤖 Threat 1: AI Attacks
**What it is:** Hackers now have robots (AI) that hack FOR them. These robot hackers work 24/7, never get tired, and learn from their mistakes.

**Real-world example:** An AI bot studies how AutoTrade works for weeks, then sends thousands of fake buy/sell orders to crash the market.

**Why it's scary:** Old security tools were built to stop humans. They can't keep up with AI that adapts and attacks faster than any human could.

---

### 👤 Threat 2: Deepfakes
**What it is:** Using AI to create fake videos and voice recordings that look and sound 100% real.

**Real-world example:** In 2024, a company in Hong Kong lost **$25 million** because an employee got a video call from someone who looked and sounded exactly like their boss — but it was a deepfake. The "boss" told them to transfer money to a hacker's account.

**Why it's scary:** In 2026, deepfakes are so good that even trained security people can't tell the difference just by looking.

---

### ⚛️ Threat 3: Quantum Computer Attacks
**What it is:** A quantum computer is a new type of super-powerful computer that can break ALL passwords and encryption we use today.

**How encryption works (simple):** Imagine your data is in a safe with a combination lock. Normal computers would need **thousands of years** to guess the combination. A quantum computer could guess it in **minutes**.

**The sneaky part — "Harvest Now, Decrypt Later":** Hackers are ALREADY stealing encrypted data today. They can't read it yet, but they're saving it for when quantum computers become available. Then they'll unlock everything.

---

### 🎣 Threat 4: AI-Powered Scams (Social Engineering)
**What it is:** Instead of sending the same scam email to everyone, AI now creates **personalized** scam messages for EACH person — using info from their Facebook, LinkedIn, etc.

**Example:** The AI reads a bank employee's social media, learns their boss's name and writing style, then sends a fake email that says "Hey, I need you to reset the admin password ASAP." It looks EXACTLY like their real boss wrote it.

**Key stat:** **82% of data breaches happen because a human made a mistake** (clicked a bad link, gave away a password, etc.)

---

# CHAPTER II — Where Can Hackers Break In?

Think of our financial system like a building. We need to check every **door, window, and vent** where someone could sneak in. These entry points are called the **"attack surface."**

## Layer 1: The Machines (Hardware)

These are physical things that can be tampered with:

- **ATMs and card terminals** → Hackers install tiny devices (skimmers) that copy your card data while you pay normally
- **Trading servers** → The actual computers running AutoTrade. If someone sneaks a bad chip into the hardware, they control everything
- **Payment sensors** → Those tap-to-pay devices everywhere? They rarely get software updates, making them easy to hack
- **Internet routers** → If a hacker takes over a router, they can secretly read ALL data passing through it (like opening someone's mail before they get it)

## Layer 2: The Software (Apps & Code)

These are bugs and weaknesses in the programs:

- **Smart contract bugs** → If there's a coding mistake in a smart contract, hackers can exploit it to drain money. This already happened: the "DAO Hack" in 2016 lost **$60 million** because of one bug
- **API connections** → APIs are like doors between different systems (bank ↔ wallet ↔ trading). If those doors aren't locked properly, hackers walk right through
- **Tricking the AI (Model Poisoning)** → Feed the AutoTrade AI bad data → it makes terrible trading decisions → hackers profit
- **Old encryption** → Our current "locks" (RSA, ECC) will be useless once quantum computers arrive
- **Phone app hacking** → Hackers can take apart the CebuCoin app's code and find security keys hidden inside

## Layer 3: The People (Human Mistakes)

The most dangerous layer because **technology can't fix human error**:

- **Phishing** → Fake emails/texts that trick you into clicking bad links or giving away passwords
- **Insider threats** → A disgruntled employee could sell database access on the dark web
- **Deepfake calls** → Fake video call from "the boss" approving a big money transfer
- **Bad passwords** → People still use "password123" or reuse the same password everywhere
- **Security fatigue** → When you get 50 security alerts a day, you start ignoring ALL of them — including the real ones

---

# CHAPTER III — Our Solution: Project TitanVault

TitanVault is our defense system. It has **3 layers** (we call them "pillars"). If one layer fails, the other two still protect everything.

## Pillar 1: Post-Quantum Cryptography (PQC)

### What is it?
New types of encryption (digital locks) that **even quantum computers can't break**.

### Why do we need it?
Our current locks (RSA, ECC) are like regular padlocks. Quantum computers are like a master lockpick that can open any regular padlock. So we replace ALL our padlocks with a completely new type of lock that the master lockpick has never seen.

### The specific locks we use:
| Lock Name | What It Does |
|-----------|-------------|
| **CRYSTALS-Kyber** | Encrypts data (scrambles it so nobody can read it) |
| **CRYSTALS-Dilithium** | Digital signature (proves a transaction is real and hasn't been tampered with) |
| **AES-256** | Encrypts stored data with a longer key (like making your padlock combination twice as long) |

### 💡 Simple analogy:
> You hear a master locksmith is coming to town who can open ANY regular lock. So you replace ALL your locks with a completely different type that this locksmith has never seen and has no tools for.

---

## Pillar 2: Zero Trust Architecture (ZTA)

### What is it?
A security rule that says: **"Never trust anyone. Verify EVERY TIME."**

### The old way vs. the new way:
- **OLD (Castle Model):** Once you're inside the building, you can go anywhere. Problem: if a hacker gets in, they get EVERYTHING.
- **NEW (Zero Trust):** Even if you're already inside, you must show your ID at EVERY door, EVERY time. Even the CEO gets checked.

### The 4 rules:
1. **Verify explicitly** — Check identity + device + location + time before allowing access
2. **Least privilege** — Only give people access to what they NEED. A teller shouldn't access trading algorithms.
3. **Assume breach** — Design the system AS IF hackers are already inside
4. **Micro-segmentation** — Divide the network into tiny isolated rooms. Hacking one room doesn't let you into any other room.

### 💡 Simple analogy:
> Imagine a hotel where even if you have a room key, you still need to show your face at the elevator, scan your fingerprint in the hallway, AND use your key at your door. Even if a thief steals your room key, they'd be stopped at 3 other checkpoints.

---

## Pillar 3: Sentinel AI

### What is it?
Our own AI that watches EVERYTHING in real-time — like a super-intelligent security guard.

### What it does:
| Power | How It Works |
|-------|-------------|
| **Transaction Monitor** | Watches every buy/sell/transfer. If something looks weird, it freezes the transaction in 0.3 seconds |
| **Deepfake Detector** | Scans video calls for tiny signs of AI manipulation (pixel glitches, unnatural eye movement) |
| **Behavioral Biometrics** | Learns how each person types and navigates. If someone logs in with stolen credentials but types differently → blocked |
| **Threat Prediction** | Scans dark web forums and global threat feeds. If hackers are planning an attack on Neo-Cebu, we know before it happens |

### 💡 Simple analogy:
> A security guard who has memorized every employee's face, voice, typing style, and daily routine. Even if someone puts on a perfect disguise, the guard notices they walk differently and type weird.

---

### How the 3 pillars work together:

```
ATTACK HAPPENS
     ↓
[Pillar 1 - PQC] → Data is encrypted → Hacker CAN'T read it
     ↓ (what if they bypass encryption?)
[Pillar 2 - Zero Trust] → Access denied → Hacker CAN'T enter
     ↓ (what if they get credentials?)
[Pillar 3 - Sentinel AI] → Behavior doesn't match → Account LOCKED
     ↓
ALL 3 MUST FAIL for an attack to succeed (extremely unlikely)
```

---

# CHAPTER IV — How We Install It (Without Breaking Anything)

The problem: **millions of people use CebuCoin every day.** We can't just shut everything down to upgrade. So we do it in 3 phases over 12 months.

## Phase 1: Prepare (Months 1–3)
**Don't touch the live system yet.** Just get ready.
- Scan everything to confirm all weak spots ✅
- Build a copy of the entire system to test on ✅
- Train all employees on new security rules ✅
- Feed Sentinel AI 2 years of data so it learns what's "normal" ✅

## Phase 2: Deploy One Layer at a Time (Months 4–8)
**Run OLD and NEW systems side by side.** If anything goes wrong, switch back instantly.
- **Months 4–5:** Upgrade encryption to PQC (quantum-proof locks)
- **Months 6–7:** Roll out Zero Trust (ID checks everywhere)
- **Month 8:** Turn on Sentinel AI (it's been observing for 5 months already)

## Phase 3: Finish & Test (Months 9–12)
**Turn off old systems. TitanVault is now the main defense.**
- Hire ethical hackers to try breaking in (Red Team) ✅
- Simulate a worst-case scenario (all 3 pillars attacked at once) ✅
- Publish a public report so citizens trust the system ✅

### 💡 Key principle to remember:
> "The old system and the new system run side by side. If the new system has ANY issue, we instantly fall back to the old one. No citizen notices a thing."

---

# CHAPTER V — Proving It Works (CIA Triad)

**CIA** here does NOT mean the spy agency. It stands for 3 security goals:

| Letter | Means | In Simple Terms |
|--------|-------|----------------|
| **C** | Confidentiality | Can strangers see my data? **NO.** |
| **I** | Integrity | Can someone secretly change my data? **NO.** |
| **A** | Availability | Can I access my money when I need it? **YES.** |

Every security system MUST pass all 3. Here's how TitanVault passes:

---

### 🔒 C — Confidentiality Test

**Scenario:** A hacker steals an employee's password and logs in.

**What happens:**
1. Zero Trust checks the device → **not recognized** → extra verification required
2. Sentinel AI checks typing pattern → **doesn't match** the real employee
3. Account is **locked in 5 seconds**

**Result:** Hacker saw nothing. ✅

---

### 🔏 I — Integrity Test

**Scenario:** A hacker changes a smart contract to redirect loan payments to their wallet.

**What happens:**
1. PQC digital signature on the contract → **signature doesn't match** the modified version
2. Blockchain → **rejects** the altered contract (you can't change blockchain records)
3. Sentinel AI → **flags** the attempt and alerts the security team

**Result:** Nothing was changed. ✅

---

### 🟢 A — Availability Test

**Scenario:** A DDoS attack floods AutoTrade with 10 million fake requests per second.

**What happens:**
1. Sentinel AI detects the attack in 0.2 seconds → **filters out** fake traffic
2. Micro-segmentation → AutoTrade is isolated → **wallets and smart contracts keep working**
3. Backup servers → take over from different location

**Result:** System stayed online. ✅

---

# ❓ QUESTIONS THE PROFESSOR MIGHT ASK (And Your Answers)

### "Why not just use existing security tools?"
> "Existing tools were built for 2024-2025 threats. They use rule-based detection that can't adapt to AI-powered attacks. Our TitanVault uses AI vs AI, quantum-proof encryption, and a Zero Trust model that assumes the attacker is already inside. It's built for 2026 and beyond."

### "What if quantum computers never become a threat?"
> "We're using the 'Harvest Now, Decrypt Later' defense. Attackers are already collecting encrypted data today. Even if quantum computers take 5 more years, our data from today would still be vulnerable. PQC protects it from day one."

### "What's the weakest point in your system?"
> "Honestly, it's still the human element. No technology can fully prevent someone from giving away their password. That's why we combine technology (PQC + Zero Trust) with AI monitoring (Sentinel) — so even when humans make mistakes, the system catches it."

### "What happens if all 3 pillars fail at the same time?"
> "We planned for that in Phase 3 with our disaster recovery drill. We have geographic redundancy (backup servers in a different city) and can restore from a clean backup. But the probability of all 3 failing simultaneously is extremely low because each pillar protects against different types of attacks."

### "How much would this cost?"
> "The phased approach spreads costs over 12 months. Phase 1 is mostly labor (audits and training). PQC algorithms are open-source (free from NIST). The biggest cost is Sentinel AI's infrastructure, but it replaces the need for large 24/7 human security teams, so it pays for itself."

---

# 🎤 QUICK CHEAT SHEET FOR THE DEFENSE

If you forget everything else, remember these **5 sentences:**

1. **"Neo-Cebu's financial systems face 4 threats: AI attacks, deepfakes, quantum threats, and social engineering."**
2. **"Hackers can break in through the machines, the software, or the people."**
3. **"TitanVault has 3 pillars: unbreakable locks (PQC), ID checks everywhere (Zero Trust), and a smart guard (Sentinel AI)."**
4. **"We deploy it in 12 months with zero downtime — old and new systems run side by side."**
5. **"It passes all CIA tests: no one sees what they shouldn't, no one changes what they shouldn't, and the system never goes down."**

**That's your entire project in 5 sentences.** Everything else is just details backing these up.
