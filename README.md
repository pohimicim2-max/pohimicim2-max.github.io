# FEAL Web Services
>[!note]
>### A collection of lightweight, high-performance web interfaces designed for the FEAL ecosystem, featuring a modern "Discord-inspired" aesthetic with advanced CSS animations and responsive layouts.

## 📊 Project Status & Roadmap

The project is currently in the **Alpha stage. ( **25%** total progress** ). While the visual foundation is solid, the core logic is being actively developed.

### ✅ Finished and ready:
| Component | Status | Progress | Details |
| :--- | :--- | :--- | :--- |
| **Redirect UI/UX** | 🟢 Ready | ![100%](https://geps.dev/progress/100) | **CSS style is ready.** |
| **Auth Interface (CSS)** | 🟢 Ready | ![100%](https://geps.dev/progress/100) | Glassmorphism design fully implemented. |
| **Particle Engine** | 🟢 Ready | ![100%](https://geps.dev/progress/100) | Dynamic background particle system with JS randomization. |
| **Discord Typography & Branding** | 🟢 Ready | ![100%](https://geps.dev/progress/100) | Unified Discord-inspired branding and typography (gg sans). |
| **JavaScript `?url=` function/logic** | 🟢 Ready | ![100%](https://geps.dev/progress/100) | `index.html` basicly is working, but missing analytics. |

### ⚒️ Not finished and W.I.P:
| Component | Status | Progress | Details | Major Update | Priority |
| :--- | :--- | :--- | :--- | :---: | :--- |
| **Analytics Engine** | 🟡 Developing | ![7.4%](https://geps.dev/progress/7.4) | JavaScript logic for tracking links without databases. | ✅ | 🔥 **High** |
| **Own our domain (feal.online)** | 🔴 Planned | ![0%](https://geps.dev/progress/0) | ~~github.io~~ -> Waiting for the perfect time to migrate. | 50/50 | 💤 *Low* |
| **Accounts logic** | 🟡 Developing | ![8%](https://geps.dev/progress/8) | Account logic with JavaScript function (Without db). | ✅ | 🔥 **High** |

### 📁 Files and Sites
| Site (File) | Status | Progress | Details | Major Update |
| :--- | :--- | :--- | :--- | :---: |
| [FEAL] Redirect (`index.html`) | 🟡 Polishing | ![85%](https://geps.dev/progress/85) | UI ready, integrating analytics JS for sync with Dashboard. | ✅ |
| [FEAL] Auth (`Dashboard/index.html`) | 🟠 Developing | ![20%](https://geps.dev/progress/20) | UI ready, doing JS Accounts logic and analytics sync. | ✅ |
| `README.md` | 🟢 Ready | ![100%](https://geps.dev/progress/100) | File is ready for reading, but adding more features. | ❌ |
| `CHANGELOG.md` | 🔴 Planned | ![0%](https://geps.dev/progress/0) | ~~*Soon*.~~ -> Transitioning to version tracking (v1.0.0-alpha). | ✅ |
| `settings.json` | 🔴 Planned | ![0%](https://geps.dev/progress/0) | Centralized configuration for domains and settings. | ✅ |
| `script.js` and `style.css` | 🔴 Planned | ![0%](https://geps.dev/progress/0) | Will add for more optimization in code. | ✅ |

---
## Project Overview
### 1. **[FEAL] Redirect Service** (`index.html`)    
A safety-first link shim/redirector that intercepts external URLs to protect users from potentially malicious content.
**Key Features:**
* **Dynamic Link Analysis:** Automatically parses URLs via query parametres (`/?url=`).
* **Security Categorization:**
  * **Trusted:** Verified domains for checking the ticket (Youtube, Discord, Medal, etc.) get a green theme and faster cooldown (3s).
  * **Suspect:** Highlights dangerous TLDs (.cc, .zip, .xyz) with a red warning banner.
  * **Insecure:** Detects `http://` protocols and alerts the user about data risks.
* **Visual domain finder:** Clearly displays the *"Main Domain"* to prevent phishing.
* **Countdown Lock:** Prevents accidental clicks by disabling the button for a set duration.

---

### 2. [FEAL] Auth Service / Analytics Dashboard (`Dashboard/index.html`)
A sleek, glassmorphism-style portal designed for site analytics and link tracking.
**Key Features:**
* **Traffic Analytics:** Monitors and displays statistics for sites and the most popular links that have passed through the Redirect Service.
* **Glassmorphism User Interface**: High-blur backdrops (16px) with semi-transparent borders for a premium administrative feel
* **Optimized Typography:** Implements the gg sans font family for a familiar Discord-like vibe.
* **Secure Access**: Provides a gateway to the internal monitoring system of the FEAL ecosystem.
* **Animated Background:** Shared particle engine to maintain brand consistency across the platform.
---
# Usage
### Redirect Service
To use the redirector, navigate to the file with the `url` parameter:
```
https://pohimicim2-max.github.io/?url=
```
like:
```
https://pohimicim2-max.github.io/?url=https://youtube.com
```
### Auth service (Dashboard)
Simply open index1.html in your browser to access the analytics login interface.
>[!caution]
>### do **NOT** press "Forget password?" button.

---
# Visual Identity
### **The projects follow a specific dark-theme palette:**

* **Background:** `#000000` (Pure Black)

* **Cards:** `rgba(15, 15, 15, 0.7)` with Blur

* **Primary Accent:** `#5865F2` (Blurple)

* **Status Colors:**
  *    **🔴 Danger:** #F23F42

   * **🟡 Warning:** #F0B232

   * **🟢 Success:** `#23A55A`
---
# Technical Stack
* **Styling:** [TailWind CSS](https://tailwindcss.com/)
* **Logic:** Vanila JavaScript
* **Visuals:** CSS keyframe Animations & Dynamic Particle Engine

>[!note]
>### *Developed for the FEAL Ticket Bot with 💖*