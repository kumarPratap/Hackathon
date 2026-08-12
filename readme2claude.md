# 🎓 College EventHub

**Discover. Register. Participate. Experience campus better.**

College EventHub is a modern, responsive web platform that brings every college event into one clean, student-friendly place — so students stop hunting through WhatsApp groups, Instagram posts, and notice boards to find out what's happening on campus.

> Built for **AVISHKAR 2026 — Frontend Web Development Hackathon**

---

## 📌 Table of Contents

- [The Problem](#-the-problem)
- [Our Solution](#-our-solution)
- [Live Demo Flow](#-live-demo-flow)
- [Core Features](#-core-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [How to Use the Site](#-how-to-use-the-site)
- [Judging Criteria Alignment](#-judging-criteria-alignment)
- [Roadmap](#-roadmap)
- [Anticipated Questions](#-anticipated-questions)
- [One-Minute Pitch](#-one-minute-pitch)
- [Team](#-team)

---

## 🎯 The Problem

Event information on a typical campus is scattered across WhatsApp/Telegram groups, Instagram pages, department notices, posters, emails, and word of mouth.

> **Students don't lack opportunities. They lack visibility.**

A student might miss a hackathon they'd love to join, forget the date of a seminar they registered for, or never hear about a cultural event at all — simply because the information never reached them in a usable form.

## 💡 Our Solution

College EventHub is **one platform** where students can discover, understand, register for, and track college events. It doesn't stop at "here's an event" — it carries the student all the way to "you're registered and ready to participate."

```
DISCOVER → EXPLORE → UNDERSTAND → REGISTER → TRACK → PARTICIPATE
```

## 🧭 Live Demo Flow

```
HOME PAGE
   │
   ├── 🔍 Search        📂 Categories        🔥 Featured
   │                         │
   └─────────────────────────┴─────────────────► EVENTS LIST
                                                       │
                                                       ▼
                                                EVENT DETAILS
                                            (date, venue, prize, etc.)
                                                       │
                                                       ▼
                                                 REGISTER NOW
                                                       │
                                                       ▼
                                          REGISTRATION FORM + JS VALIDATION
                                                       │
                                                       ▼
                                             REGISTRATION SUCCESS
                                            (unique ID e.g. CEH-2026-4821)
                                                       │
                                                       ▼
                                                   MY EVENTS
                                                       │
                                                       ▼
                                             🎟️ DIGITAL EVENT PASS
```

## ✨ Core Features

| # | Feature | Description |
|---|---------|-------------|
| 1 | 🔍 **Event Discovery** | Featured events, upcoming events, search, and category browsing |
| 2 | 📂 **Categories** | Technology, Competitions, Seminars, Workshops, Cultural, Sports, Entertainment, Social & Community |
| 3 | 🔎 **Search & Filtering** | Keyword search (e.g. "AI") plus category-based filtering |
| 4 | 📄 **Event Details** | Name, category, description, date, time, venue, organizer, eligibility, deadline, prize, seats left |
| 5 | 📝 **Simple Registration** | Name, email, branch, year, phone — validated client-side with JavaScript |
| 6 | 🆔 **Unique Registration ID** | Auto-generated ID on successful registration, e.g. `CEH-2026-4821` |
| 7 | ⏱️ **Event Countdown** | Live countdown timer (days/hours/min/sec) to each registered event |
| 8 | 🎟️ **Digital Event Pass** | Shareable pass with student name, branch/year, reg ID, date, venue |
| 9 | 📋 **My Events Dashboard** | Personal view of all registered events, IDs, countdowns, and passes |

## 🏗️ Tech Stack

- **HTML5** — structure and semantic markup
- **CSS3** — layout, responsiveness, animations (no frameworks)
- **Vanilla JavaScript** — interactivity, validation, ID generation, countdowns (no frameworks or external APIs)
- **localStorage** — client-side persistence for registrations and "My Events" (no backend required for the prototype)

This stack was chosen deliberately to satisfy the competition's technical restrictions while proving that a polished, functional product doesn't require a framework.

## 🧩 Project Structure

```
College-EventHub/
│
├── index.html      → Structure and content of the application
├── style.css       → Layout, colors, typography, responsiveness, animations, cards, navigation
├── script.js       → Search, filtering, validation, ID generation, countdowns, My Events, localStorage, UI interactions
└── README.md       → This file
```

## 🚀 Getting Started

No build tools, installs, or servers required.

1. **Clone or download** this repository.
2. Open `index.html` directly in any modern browser (Chrome, Edge, Firefox, Safari) — double-click it, or use a lightweight local server for the best experience:
   ```bash
   # Optional — avoids any file:// quirks with localStorage
   npx serve .
   # or
   python3 -m http.server 8000
   ```
3. Navigate to `http://localhost:8000` (if using a server) or the opened file.
4. Start exploring events from the home page.

No API keys, `.env` files, or backend setup are needed — everything runs client-side.

## 🕹️ How to Use the Site

1. **Browse or search** for an event from the home page (by keyword or category).
2. **Open an event** to view full details — date, venue, eligibility, prize, seats.
3. Click **Register Now** and fill in the short form (name, email, branch, year, phone).
4. JavaScript **validates** the form; on success you receive a **unique registration ID**.
5. Head to **My Events** to see all your registrations, live countdowns, and your **digital event pass**.

## 🏆 Judging Criteria Alignment

| Criterion | How This Project Addresses It |
|---|---|
| Attractive UI | Card-based layouts, clear hierarchy, category icons, subtle hover/animation feedback |
| Minimum lines of code | Single-purpose, reusable JS functions and CSS utility patterns; no redundant markup |
| Counter questions | See [Anticipated Questions](#-anticipated-questions) below — the team is prepped to justify every design choice |
| Justify the project | Clear problem → solution narrative (see [The Problem](#-the-problem) and [One-Minute Pitch](#-one-minute-pitch)) |
| UI/UX & functionality (tie-break) | Full user journey implemented: discover → register → track, not just a static listing |
| Code quality & organization (tie-break) | Clean 3-file architecture, consistent naming, commented logic in `script.js` |

## 🗺️ Roadmap

### ✅ Phase 1 — Prototype (Competition Scope, this build)
- [x] Responsive home page with search, categories, and featured/upcoming sections
- [x] Event listing and detailed event view
- [x] Registration form with client-side JavaScript validation
- [x] Unique registration ID generation on successful signup
- [x] localStorage persistence for registrations
- [x] "My Events" dashboard with live countdown timers
- [x] Digital event pass view per registered event
- [x] Fully responsive layout (mobile, tablet, laptop, desktop)

### 🔜 Phase 2 — Polish & Depth (immediate next steps post-hackathon)
- [ ] Empty/error states (no search results, no registered events yet)
- [ ] Basic accessibility pass (keyboard navigation, ARIA labels, contrast check)
- [ ] Dark mode toggle
- [ ] Export/share digital pass as an image or PDF
- [ ] Loading/skeleton states for perceived performance

### 🚀 Phase 3 — Two-Sided Ecosystem (long-term vision)
- [ ] Organizer/club dashboards to publish and manage events
- [ ] Real backend + database (replacing localStorage)
- [ ] User accounts and authentication
- [ ] Email/push notifications and reminders
- [ ] Attendance tracking and check-in via QR code (ties into the digital pass)
- [ ] Club/organizer profile pages
- [ ] Personalized event recommendations
- [ ] Event analytics for organizers (views, registrations, drop-off)

## ❓ Anticipated Questions

**Why did you build this?**
Because students routinely miss events due to scattered, unsearchable information.

**Who is your target user?**
Primarily college students who want to discover and participate in campus events; secondarily, clubs/departments in future phases.

**What problem does it solve?**
Event information fragmentation and difficult event discovery — not a lack of opportunities, but a lack of visibility into them.

**Why not just use WhatsApp/Instagram?**
Those channels are great for communication but poor for structured, searchable, trackable event information — details get buried in conversation threads.

**Why no backend?**
This is a frontend prototype demonstrating the interaction flow and UX. `localStorage` is sufficient to prove the concept without server infrastructure — a backend is the clear next step (see Roadmap Phase 3).

**Why vanilla JavaScript with no frameworks?**
It's a competition requirement, and it keeps the codebase lightweight, dependency-free, and easy for judges to inspect line by line.

**What happens after registration?**
The form is validated → a unique registration ID is generated → the registration is saved to `localStorage` → the event appears under **My Events** with a live countdown and digital pass.

**How is the site responsive?**
CSS3 layout techniques (flexbox/grid) with breakpoints adapt the card grid, navigation, and forms across mobile, tablet, laptop, and desktop viewports.

**What would you add with more time?**
Organizer dashboards, real-time notifications, attendance tracking, and a backend database — all outlined in the Roadmap above.

## 🎤 One-Minute Pitch

> College EventHub is a centralized event discovery and registration platform for college students. Event information today is scattered across WhatsApp groups, social media, and department notices, so students miss opportunities they'd otherwise want to join. EventHub brings events into one platform where students can discover, search, and filter events, view complete details, register in a few clicks, receive a unique registration ID, and track everything through a personal "My Events" dashboard with live countdowns and a digital event pass — all in a clean, responsive, framework-free frontend.

## 👨‍💻 Development Philosophy

> Simple code. Clear purpose. Great experience.

Every feature has a reason to exist. Every interaction should make the student's path from *discovering* an event to *participating* in it a little shorter.

## 📌 Project Status

- **Stage:** Frontend Prototype
- **Focus:** UI/UX + Event Discovery + Registration Flow
- **Stack:** HTML5 + CSS3 + Vanilla JavaScript
- **Platform:** Responsive Web
- **Competition:** AVISHKAR 2026 — Frontend Web Development

## 👥 Team

_Add team member names and roles here before submission._

---

**College EventHub — Your campus. Your events. One place.**
Discover → Register → Participate
