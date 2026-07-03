# 🌾 வயல் மருத்துவர் — Vayal Maruthavar
### AI Crop Disease Doctor for Tamil Nadu Farmers

<p align="center">
  <img src="icon.svg" width="120" alt="Vayal Maruthavar Icon"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Language-Tamil%20%7C%20English-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Platform-Progressive%20Web%20App-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/AI-Groq%20%7C%20Qwen%203.6-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Works%20on-2G%20Network-brightgreen?style=for-the-badge"/>
</p>

---

## 🔥 What is Vayal Maruthavar?

**வயல் மருத்துவர்** (Vayal Maruthavar) means **"Field Doctor"** in Tamil.

It is a Tamil-language AI-powered crop disease detection tool built specifically for the **57 lakh farmers of Tamil Nadu**, particularly those in the Cauvery Delta region — Thanjavur, Tiruvarur, and Nagapattinam.

A farmer photographs a sick leaf. AI identifies the disease in seconds. Treatment advice, chemical recommendations, and cost estimates appear instantly — **in Tamil, offline-first, on any basic Android phone.**

> *"AI is not just for cities. The farmer who feeds India deserves it most."*

---

## 😔 The Problem

Tamil Nadu's farmers are in crisis:

| Problem | Scale |
|---|---|
| Farmers dependent on agriculture in TN | 57 lakh |
| Annual crop losses due to disease | ₹5,000+ crore |
| Distance to nearest agri office | 10–15 km |
| Crop loss from Rice Blast if untreated | Up to 80% |
| Farmer deaths in India per year | 10,000+ |
| Existing AI agri tools in Tamil | **Zero** |

When a crop shows disease symptoms, a Tamil Nadu farmer has three bad options:
1. **Walk 10–15 km** to the nearest agricultural office — too slow, disease spreads
2. **Ask the local pesticide shop** — often gives wrong or expensive chemicals
3. **Do nothing** — watch the harvest fail and take a moneylender loan

There is no fast, Tamil-language, offline-capable AI tool that helps them. Until now.

---

## 💡 The Solution

**Vayal Maruthavar** is a Progressive Web App (installable on any Android phone) that:

```
📸 Farmer photographs sick leaf
        ↓
🤖 AI identifies crop type → asks confirmation
        ↓
✅ User confirms (or corrects) the crop
        ↓
🔬 AI analyses disease in seconds
        ↓
📋 Full Tamil diagnosis appears:
   • Disease name (Tamil + English)
   • Severity level
   • How AI identified it
   • Step-by-step treatment
   • Exact chemicals + dosage
   • What NOT to use
   • Estimated cost (₹)
   • Best time to spray
        ↓
🌾 Farmer acts immediately — harvest saved
```

---

## ✨ Key Features

### 🌿 Smart Crop Confirmation
Before diagnosing, the AI asks: *"Is this a Turmeric / மஞ்சள் leaf?"* — the farmer confirms or selects their actual crop from a dropdown. **Eliminates misidentification**, which is the #1 failure of other AI crop tools.

### 🗣️ Tamil-First, Not Translated
All results are delivered in **Tamil** by default. Not poorly translated from English — written in simple, clear Tamil that a farmer from Thanjavur can immediately understand. Toggle to English anytime.

### 📵 Works on 2G
Images are compressed to 70% quality and max 800px before sending. The AI response is concise. **Works reliably on 2G network**, which is the reality in rural Cauvery Delta.

### 🧪 Chemical Guidance
Tells farmers exactly **what to buy** (generic chemical names + dosage per litre) and critically, **what NOT to buy** — directly countering dangerous and expensive misguidance from local pesticide shops.

### 💰 Cost Estimate
Every diagnosis includes an estimated treatment cost in ₹ so farmers can plan their spend before going to the shop.

### 🔄 Language Toggle
Instant switch between **தமிழ் (Tamil)** and **English** on all result cards — useful when a farmer shows the result to an agricultural officer or family member.

### 📲 Installable as App
Built as a **Progressive Web App (PWA)** — opens in Chrome, tap "Add to Home Screen", installs as a full-screen app with icon. No APK. No app store. No permissions. One URL.

---

## 🎯 Who Is This For?

**Primary user:** Small-scale paddy farmers in Tamil Nadu's Cauvery Delta — aged 35–65, Tamil-speaking, owning under 2 acres of farmland. They use basic Android phones with 2G connectivity, have limited English literacy, and are 10–15 km away from the nearest agricultural officer.

**Secondary users:** Village Agricultural Assistants (VAAs), self-help groups (SHGs), agricultural extension workers, and farming cooperatives in Tamil Nadu.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Pure HTML5 + CSS3 + Vanilla JavaScript |
| AI Model | Qwen 3.6-27B Vision (via Groq API) |
| Image Processing | Canvas API (client-side compression) |
| Offline Support | Service Worker + Cache API |
| App Installation | Progressive Web App (PWA) |
| Hosting | GitHub Pages (free, HTTPS) |
| Languages | Tamil (primary) + English (toggle) |
| Network requirement | 2G and above |

**No frameworks. No dependencies. No build step.** Just one HTML file, a service worker, and a manifest. Runs on any device with a browser.

---

## 📁 Project Structure

```
vayal-maruthavar/
│
├── index.html        # Main app — entire frontend + AI logic
├── manifest.json     # PWA manifest (app name, icon, display mode)
├── sw.js             # Service worker (offline caching)
├── icon.svg          # App icon (wheat motif)
└── README.md         # This file
```

---

## 🚀 How to Run Locally

**No installation required.** Just open `index.html` in any browser.

```bash
# Clone the repo
git clone https://github.com/yourusername/vayal-maruthavar.git

# Navigate into it
cd vayal-maruthavar

# Open in browser (or just double-click index.html)
open index.html
```

**To use the AI features**, you need a free Groq API key:
1. Go to [console.groq.com](https://console.groq.com)
2. Sign up free → API Keys → Create API Key
3. Open `index.html` in any text editor
4. Find the line: `const KEY='your-key-here'`
5. Replace with your key → save → open in browser

---

## 🌍 How to Deploy (GitHub Pages)

1. Fork or upload this repo to GitHub
2. Go to **Settings → Pages**
3. Source: **Deploy from branch → main → / (root)**
4. Click **Save**
5. Your app is live at: `https://yourusername.github.io/vayal-maruthavar`

**To install as an app on Android:**
- Open the live URL in Chrome
- Tap **⋮ → Add to Home Screen → Install**
- App icon appears on home screen — opens full screen

---

## 📊 Projected Impact

| Scenario | Farmers Reached | Harvests Saved | Crop Value Protected |
|---|---|---|---|
| 1% adoption (TN) | 57,000 | 28,500 | ₹142 Cr |
| 5% adoption (TN) | 2.85 lakh | 1.42 lakh | ₹711 Cr |
| 10% adoption (TN) | 5.7 lakh | 2.85 lakh | ₹1,425 Cr |

*Assumes avg farm size 0.85 acres, paddy yield ₹50,000/harvest, 50% early detection success rate*

---

## 🗺️ Roadmap

### Phase 1 — Current (Rice diseases, Cauvery Delta)
- [x] AI crop disease detection with Tamil output
- [x] Smart crop type confirmation
- [x] Chemical + dosage recommendations
- [x] Tamil / English language toggle
- [x] 2G-optimised image compression
- [x] PWA — installable on Android
- [ ] Voice output (Tamil text-to-speech)

### Phase 2 — Next (All TN crops)
- [ ] Expand to sugarcane, banana, cotton, groundnut, turmeric
- [ ] Market price prediction (best time to sell)
- [ ] Cyclone / unseasonal rain early warning
- [ ] TNAU disease database integration

### Phase 3 — Scale (South India)
- [ ] Telugu, Kannada, Marathi language support
- [ ] Government VAA integration for distribution
- [ ] Disease outbreak alert system (crowd-sourced hotspot map)
- [ ] Soil health scanner (camera-based)

### Phase 4 — National
- [ ] All Indian languages
- [ ] Crop loan and insurance advisory
- [ ] Farmer community peer network
- [ ] Pre-installation on Samsung Galaxy phones sold in rural India

---

## 🏆 Competition

This project was built for **Samsung Solve for Tomorrow 2026** under the **"AI for India"** theme.

The core belief driving this project: most AI tools in agriculture are built for English-speaking, internet-connected, city-adjacent users. Vayal Maruthavar is built specifically for the farmer standing in a paddy field in Nagapattinam at 6 AM, who speaks only Tamil and has a basic Android phone with 2G signal.

---

## 👤 About the Developer

Built by a student from Tamil Nadu — with zero prior coding experience — using AI-assisted development, persistence, and a genuine belief that technology should reach those who need it most, not just those who can afford it.

**Core strengths used to build this:** Communication, persistence, and refusing to give up through 10+ API errors in one night.

---

## 📄 License

This project is currently **private** during the Samsung Solve for Tomorrow 2026 competition period.

Post-competition, it will be released under the **MIT License** — free for anyone to use, modify, and build upon, including other students, NGOs, and agricultural organisations working to support Indian farmers.

---

## 🙏 Acknowledgements

- **TNAU (Tamil Nadu Agricultural University)** — for decades of crop disease research that informed the AI prompting
- **Groq** — for providing free, fast AI API access that makes this viable for students
- **Tamil Nadu's farmers** — for feeding millions, and deserving so much better tools than they currently have

---

<p align="center">
  <strong>வயல் மருத்துவர் · Tamil Nadu Crop Doctor · AI for India</strong><br>
  <em>Built with persistence. Built for farmers. Built in Tamil.</em>
</p>
