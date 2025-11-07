# 🧠 SkillSwap — Peer-to-Peer Skill Exchange for Smarter Campus Learning

**SkillSwap** is an Android app that helps students **teach and learn from each other**.  
It connects peers across the campus using a fair **matching system**, built on data structures and algorithms, and works **fully offline** with a realistic, demo-ready experience.

Built in **24 hours** for the *Hack the Campus* hackathon.

---

## 🚀 Overview

Most colleges are full of talented students — coders, designers, musicians, editors — but those skills stay locked in their friend circles.  
**SkillSwap** changes that.

It’s a decentralized skill-sharing platform where:
- Students list what they **can teach** and what they **want to learn**.
- The app **matches** learners and mentors intelligently.
- Users can **chat**, **schedule meetups**, **rate each other**, and **climb the leaderboard**.

No backend, no network dependency — everything is **deterministic and offline** for reliability.

---

## 🔹 Key Features

- 🎯 **Smart Matchmaking Algorithm**  
  Pairs users based on complementary skills using a **PriorityQueue** scoring model:


- 💬 **Chat-Lite System**  
Simple offline chat with auto-replies (`FakeRepository` logic).

- 📅 **Session Scheduling**  
Adds events directly to Android Calendar via intent.

- ⭐ **Ratings & Leaderboard**  
Mentor points increase after ratings, updating ranks in real time.

- 🏠 **Home Dashboard**  
Personalized overview — quick actions, recommendations, top mentors.

- 👤 **Profile Screen**  
Shows user info, badges, skill chips, and shortcuts to manage skills.

- ⚙️ **Demo Mode**  
Includes **Run Live Demo**, **Reset Demo**, **Export Demo Log**, and **offline latency simulation** for a smooth hackathon showcase.

---

## 🧩 Architecture


**Design principles:**
- MVVM pattern with reactive LiveData
- No backend required
- Easily replaceable repository for future real backend (Firebase / Supabase)
- Material 3 + ViewBinding + minimal dark UI

---

## 🛠️ Tech Stack

| Category | Technology |
|-----------|-------------|
| Language | Java |
| Framework | Android SDK |
| UI | Material 3 (Dark) + ViewBinding |
| Architecture | MVVM + Repository Pattern |
| Data | Deterministic FakeRepository (in-memory) |
| Tools | Android Studio, LiveData, PriorityQueue |

---

## 🧪 Demo Mode Features

- 🧭 **1-Tap “Run Live Demo”**  
  Autonomously walks through:
  1. Matches → Profile → Chat  
  2. Suggest Intro  
  3. Schedule via Calendar Intent  
  4. Rate user  
  5. Leaderboard updates  
  6. Back to Home with refreshed data

- ⚡ **Fake Latency**  
  Adds a 350–600ms delay layer to mimic real-world loading.

- 🧾 **Demo Log**  
  Writes each action to `/data/data/.../demo_log.txt` for proof during judging.

- 🔁 **Reset Demo**  
  Resets chats, sessions, and leaderboard back to the seed state.

- 💡 **Coachmarks**  
  Small, timed tooltips guiding the flow during the automated run.

---

## 📦 Installation

### Download APK
Get the latest build from **Releases**:  
[📦 Download SkillSwap demo APK](https://github.com/akshat-1312/SKILL_SWAP_2/SkillSwap.apk)

