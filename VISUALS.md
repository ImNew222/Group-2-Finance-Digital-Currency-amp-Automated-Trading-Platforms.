# 📊 VISUAL AIDS — Neo-Cebu 2026: Finance Sector Defense
### Diagrams & Flowcharts for Presentation

> Copy these mermaid diagrams into any mermaid renderer (e.g., [mermaid.live](https://mermaid.live)) to get images for your slides.

---

## 1. 🏗️ HerculesVault Architecture — The 3 Pillars

```mermaid
graph TB
    subgraph HERCULESVAULT["🛡️ PROJECT HERCULESVAULT"]
        direction TB
        
        subgraph P1["PILLAR 1: Post-Quantum Cryptography"]
            PQC1["CRYSTALS-Kyber<br/>Quantum-Proof Encryption"]
            PQC2["CRYSTALS-Dilithium<br/>Quantum-Proof Signatures"]
            PQC3["AES-256<br/>Data at Rest"]
        end
        
        subgraph P2["PILLAR 2: Zero Trust Architecture"]
            ZT1["Verify Explicitly<br/>Multi-Factor Auth"]
            ZT2["Least Privilege<br/>Role-Based Access"]
            ZT3["Micro-Segmentation<br/>Isolated Network Zones"]
        end
        
        subgraph P3["PILLAR 3: Sentinel AI"]
            AI1["Real-Time<br/>Transaction Monitor"]
            AI2["Deepfake<br/>Detection"]
            AI3["Behavioral<br/>Biometrics"]
            AI4["Predictive Threat<br/>Intelligence"]
        end
    end

    PROTECTED["✅ NEO-CEBU FINANCE<br/>CebuCoin | AutoTrade | Wallets | Smart Contracts"]
    
    P1 --> PROTECTED
    P2 --> PROTECTED
    P3 --> PROTECTED

    style HERCULESVAULT fill:#1a1a2e,stroke:#e94560,stroke-width:3px,color:#fff
    style P1 fill:#0f3460,stroke:#53d8fb,stroke-width:2px,color:#fff
    style P2 fill:#0f3460,stroke:#53d8fb,stroke-width:2px,color:#fff
    style P3 fill:#0f3460,stroke:#53d8fb,stroke-width:2px,color:#fff
    style PROTECTED fill:#16c79a,stroke:#11999e,stroke-width:3px,color:#000
```

---

## 2. 🐉 Hydra-Pulse Threat Map

```mermaid
graph LR
    HYDRA["🐉 HYDRA-PULSE<br/>Threat Framework"]
    
    HYDRA --> H1["🤖 HEAD 1<br/>AI-Powered Attacks"]
    HYDRA --> H2["👤 HEAD 2<br/>Deepfake Fraud"]
    HYDRA --> H3["⚛️ HEAD 3<br/>Quantum Threats"]
    HYDRA --> H4["🎣 HEAD 4<br/>Social Engineering"]
    
    H1 --> H1A["AI Market<br/>Manipulation"]
    H1 --> H1B["Automated<br/>Vulnerability Scanning"]
    
    H2 --> H2A["Fake CEO<br/>Video Calls"]
    H2 --> H2B["Forged<br/>Documents"]
    
    H3 --> H3A["Break RSA/ECC<br/>Encryption"]
    H3 --> H3B["Harvest Now<br/>Decrypt Later"]
    
    H4 --> H4A["AI-Crafted<br/>Phishing"]
    H4 --> H4B["Hyper-Personalized<br/>Scam Messages"]

    style HYDRA fill:#e94560,stroke:#c70039,stroke-width:3px,color:#fff
    style H1 fill:#ff6b6b,stroke:#c70039,color:#fff
    style H2 fill:#ff6b6b,stroke:#c70039,color:#fff
    style H3 fill:#ff6b6b,stroke:#c70039,color:#fff
    style H4 fill:#ff6b6b,stroke:#c70039,color:#fff
```

---

## 3. 🎯 Attack Surface Map — 3 Layers

```mermaid
graph TB
    subgraph ATTACK["🎯 ATTACK SURFACE"]
        direction TB
        
        subgraph HW["🔩 LAYER 1: HARDWARE"]
            HW1["ATM/POS Terminal<br/>Tampering"]
            HW2["Trading Server<br/>Backdoors"]
            HW3["IoT Payment<br/>Sensor Exploits"]
            HW4["Network Router<br/>Hijacking"]
        end
        
        subgraph SW["💻 LAYER 2: SOFTWARE"]
            SW1["Smart Contract<br/>Bugs"]
            SW2["Insecure<br/>APIs"]
            SW3["AI Model<br/>Poisoning"]
            SW4["Outdated<br/>Encryption"]
            SW5["Mobile App<br/>Reverse Engineering"]
        end
        
        subgraph HU["🧠 LAYER 3: HUMAN"]
            HU1["AI-Enhanced<br/>Phishing"]
            HU2["Insider<br/>Threats"]
            HU3["Deepfake<br/>Authorization"]
            HU4["Weak<br/>Passwords"]
            HU5["Security<br/>Fatigue"]
        end
    end
    
    DANGER["⚠️ 82% of breaches<br/>involve the HUMAN layer"]
    HU --> DANGER

    style ATTACK fill:#1a1a2e,stroke:#e94560,stroke-width:2px,color:#fff
    style HW fill:#2d3436,stroke:#fdcb6e,stroke-width:2px,color:#fff
    style SW fill:#2d3436,stroke:#6c5ce7,stroke-width:2px,color:#fff
    style HU fill:#2d3436,stroke:#e17055,stroke-width:2px,color:#fff
    style DANGER fill:#d63031,stroke:#c70039,stroke-width:3px,color:#fff
```

---

## 4. 🚀 12-Month Deployment Timeline

```mermaid
gantt
    title HerculesVault Deployment Roadmap (12 Months)
    dateFormat YYYY-MM
    axisFormat %b

    section Phase 1 - Preparation
    Security Audit              :a1, 2026-07, 1M
    Build PQC Test Lab          :a2, 2026-07, 2M
    Staff Training              :a3, 2026-08, 2M
    Sentinel AI Baseline        :a4, 2026-07, 3M

    section Phase 2 - Deployment
    PQC Encryption Upgrade      :b1, 2026-10, 2M
    Zero Trust Rollout          :b2, 2026-12, 2M
    Sentinel AI Activation      :b3, 2027-02, 1M

    section Phase 3 - Testing
    Legacy Decommission         :c1, 2027-03, 1M
    Red Team Exercise           :c2, 2027-04, 1M
    Disaster Recovery Drill     :c3, 2027-05, 1M
    Public Report               :c4, 2027-06, 1M
```

---

## 5. 🔺 CIA Triad — Defense Flowchart

```mermaid
graph TB
    CIA["🔺 CIA TRIAD"]
    
    CIA --> C["🔒 CONFIDENTIALITY<br/>Only authorized people see data"]
    CIA --> I["🔏 INTEGRITY<br/>Data cannot be changed"]
    CIA --> A["🟢 AVAILABILITY<br/>Systems always running"]
    
    C --> C1["PQC Encryption<br/>Quantum-proof locks"]
    C --> C2["Zero Trust<br/>ID checks everywhere"]
    C --> C3["Sentinel AI<br/>Anomaly detection"]
    
    I --> I1["Dilithium Signatures<br/>Tamper-proof"]
    I --> I2["Blockchain<br/>Immutable records"]
    I --> I3["Sentinel AI<br/>Model integrity check"]
    
    A --> A1["Micro-Segmentation<br/>Isolate failures"]
    A --> A2["Geo-Redundancy<br/>Backup data centers"]
    A --> A3["DDoS Protection<br/>Traffic filtering"]

    C1 -.->|"Stress Test"| CT["Credential Theft<br/>→ Device blocked<br/>→ Behavior flagged<br/>✅ PROTECTED"]
    I1 -.->|"Stress Test"| IT["Contract Tampered<br/>→ Signature fails<br/>→ Blockchain rejects<br/>✅ PROTECTED"]
    A1 -.->|"Stress Test"| AT["DDoS Attack<br/>→ Traffic filtered<br/>→ Backup takes over<br/>✅ PROTECTED"]

    style CIA fill:#e94560,stroke:#c70039,stroke-width:3px,color:#fff
    style C fill:#0984e3,stroke:#74b9ff,stroke-width:2px,color:#fff
    style I fill:#6c5ce7,stroke:#a29bfe,stroke-width:2px,color:#fff
    style A fill:#00b894,stroke:#55efc4,stroke-width:2px,color:#fff
    style CT fill:#2d3436,stroke:#00cec9,color:#fff
    style IT fill:#2d3436,stroke:#00cec9,color:#fff
    style AT fill:#2d3436,stroke:#00cec9,color:#fff
```

---

## 6. 🔄 Zero Trust vs Old Security Model

```mermaid
graph LR
    subgraph OLD["❌ OLD MODEL: Castle & Moat"]
        direction LR
        LOGIN1["Employee<br/>Logs In"] --> TRUST["✅ Trusted!<br/>Access Everything"]
        TRUST --> HACK["😱 If hacked:<br/>Hacker gets ALL"]
    end
    
    subgraph NEW["✅ NEW MODEL: Zero Trust"]
        direction LR
        LOGIN2["Employee<br/>Logs In"] --> CHECK1["🔍 Verify<br/>Identity"]
        CHECK1 --> CHECK2["🔍 Verify<br/>Device"]
        CHECK2 --> CHECK3["🔍 Verify<br/>Location"]
        CHECK3 --> CHECK4["🔍 Verify<br/>Access Level"]
        CHECK4 --> LIMITED["📁 Access ONLY<br/>what you need"]
    end

    style OLD fill:#d63031,stroke:#c70039,stroke-width:2px,color:#fff
    style NEW fill:#00b894,stroke:#00cec9,stroke-width:2px,color:#fff
```

---

## 7. 🔐 How PQC Protects CebuCoin Transactions

```mermaid
sequenceDiagram
    participant U as 👤 User (Sender)
    participant W as 📱 CebuCoin Wallet
    participant S as 🛡️ HerculesVault
    participant B as ⛓️ Blockchain
    participant R as 👤 Receiver

    U->>W: Send 500 CebuCoin
    W->>S: Encrypt with CRYSTALS-Kyber
    S->>S: Sign with CRYSTALS-Dilithium
    S->>B: Submit encrypted + signed transaction
    B->>B: Verify Dilithium signature ✅
    B->>B: Record on immutable ledger ✅
    B->>R: CebuCoin received!
    
    Note over S: Even quantum computers<br/>cannot break this encryption
```

---

## 📌 HOW TO USE THESE DIAGRAMS

### Option A: Online Renderer (Easiest)
1. Go to **[mermaid.live](https://mermaid.live)**
2. Copy-paste any diagram code above
3. Screenshot or download the result
4. Paste into your PowerPoint/Google Slides

### Option B: VS Code Extension
1. Install the **"Markdown Preview Mermaid Support"** extension
2. Open this file in VS Code
3. Press `Ctrl+Shift+V` to preview
4. Screenshot the diagrams

### Option C: Export as Images
```bash
# Install mermaid CLI
npm install -g @mermaid-js/mermaid-cli

# Convert this file's diagrams to PNG
mmdc -i VISUALS.md -o diagram.png
```

---

## 🎤 WHICH DIAGRAM FOR WHICH PRESENTER

| Presenter | Diagram to Show | When |
|-----------|----------------|------|
| **Mary Grace** | #2 Hydra-Pulse Threat Map | While explaining the 4 threats |
| **Jerimy** | #3 Attack Surface Map (3 Layers) | While mapping vulnerabilities |
| **Ashlee** | #1 HerculesVault Architecture + #6 Zero Trust + #7 PQC Transaction | While explaining the solution |
| **Mike** | #4 Deployment Timeline | While explaining the 12-month plan |
| **Everyone** | #5 CIA Triad Flowchart | During the final Act V |
