# 🎓 College EventHub

> **Discover. Register. Participate. Experience campus better.**

College EventHub is a responsive frontend prototype that helps students discover, understand, and register for campus events from one organized place.

Instead of searching WhatsApp groups, Instagram posts, notice boards, department messages, and posters, students can explore events, check important details, register in seconds, and receive a digital event pass.

Built for **AVISHKAR 2026 — Frontend Web Development Hackathon**.

---

## 📌 Contents

- [The Problem](#-the-problem)
- [The Solution](#-the-solution)
- [User Journey](#-user-journey)
- [Features](#-features)
- [Technology](#-technology)
- [Project Structure](#-project-structure)
- [Run Locally](#-run-locally)
- [Roadmap](#-roadmap)
- [Hackathon Strategy](#-hackathon-strategy)
- [Judge Q&A](#-judge-qa)
- [One-Minute Pitch](#-one-minute-pitch)

---

## 🎯 The Problem

Campus event information is usually scattered across WhatsApp and Telegram groups, social-media posts, notices, emails, clubs, and word of mouth.

> **Students do not lack opportunities. They lack visibility.**

A student may never hear about a hackathon they would enjoy, may forget the time and venue of a seminar, or may miss a cultural event because its announcement was buried among unrelated messages.

---

## 💡 The Solution

College EventHub creates one structured experience for the whole student journey:

```text
DISCOVER → EXPLORE → UNDERSTAND → REGISTER → TRACK → PARTICIPATE
```

The platform does not stop at *“Here is an event.”* It helps students reach *“I am registered and ready to participate.”*

### Target users

- **Primary:** College students who want to find and join campus events.
- **Future secondary:** Clubs and departments that need a place to publish and manage events.

> **Organizers create opportunities → Students discover opportunities.**

---

## 🧭 User Journey

```text
HOME PAGE
   │
   ├── Search ──┐
   ├── Category ├──► EVENTS LIST ──► EVENT DETAILS
   └── Featured ┘                         │
                                         REGISTER
                                            │
                              VALIDATED REGISTRATION FORM
                                            │
                              SUCCESS + UNIQUE REGISTRATION ID
                                            │
                                    DIGITAL EVENT PASS
```

---

## ✨ Features

### Available in the current prototype

| Feature | What it does |
|---|---|
| 🔍 Event discovery | Presents a curated list of upcoming campus events. |
| 📂 Search and filters | Searches event names/descriptions and filters events by category. |
| 📄 Event details | Shows date, time, venue, prize, seats, eligibility, and organizer. |
| 📝 Registration validation | Requires valid name, email, branch, year, and 10-digit phone number. |
| 🆔 Registration ID | Generates an ID such as `CEH-2026-4821` after registration. |
| 🎟️ Digital event pass | Displays the registered event, student details, venue, date, and ID. |
| 💾 Browser persistence | Saves registrations in `localStorage` and restores the My Events count. |
| 📱 Responsive interface | Uses CSS grid, flexbox, and breakpoints for mobile through desktop screens. |

### Planned next features

- A dedicated **My Events** dashboard showing every registered event
- Live event countdowns
- Registration deadline and seat-status rules
- Event pass download or print support
- Organizer/club event management

---

## 🎨 UI/UX Principles

College EventHub is designed to be:

1. **Simple** — students should understand it immediately.
2. **Visual** — cards, icons, and clear hierarchy make events easy to scan.
3. **Fast** — a student should reach an event and register with minimal steps.
4. **Responsive** — it should feel natural on mobile, tablet, laptop, and desktop.
5. **Engaging** — hover states, modal feedback, and the event pass make the experience feel active without being distracting.

---

## 🏗️ Technology

| Technology | Purpose |
|---|---|
| HTML5 | Semantic page structure and accessible form controls |
| CSS3 | Responsive layout, visual design, transitions, and modals |
| Vanilla JavaScript | Event search, filtering, dialogs, validation, registration IDs, and browser storage |
| `localStorage` | Saves registration details within the browser for this prototype |

No frameworks, external APIs, backend, API keys, or build tools are required.

---

## 🧩 Project Structure

```text
Hackathon/
├── index.html          # Page structure and current JavaScript interactions
├── style.css           # Visual design and responsive styles
├── README.md           # Project documentation
└── readme2claude.md    # Earlier README draft kept for reference
```

> The current JavaScript lives inside `index.html`. Moving it into `script.js` is a planned code-organization improvement.

---

## 🚀 Run Locally

No installation is needed.

1. Download or clone this project.
2. Open `index.html` in a modern browser.
3. Explore an event, open its details, and try the registration flow.

For the most consistent local-browser behavior, run a lightweight local server from the project folder:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

---

## 🕹️ How to Use

1. Browse the event cards or search for a keyword such as `Hackathon`.
2. Select a category, such as Technology, Competition, Workshop, or Cultural.
3. Open **View Details** to review the event information.
4. Choose **Register Now** and complete the form.
5. Receive a unique registration ID and digital event pass.
6. Use **My Events** in the navigation to view your saved registration pass.

---

## 🗺️ Roadmap

### ✅ Phase 1 — Current hackathon prototype

- [x] Responsive homepage and navigation
- [x] Event cards, search, and category filters
- [x] Event details modal
- [x] Client-side registration validation
- [x] Generated registration ID and digital pass
- [x] `localStorage` registration persistence

### 🔜 Phase 2 — Polish and depth

- [ ] Move JavaScript into `script.js`
- [ ] Dedicated My Events dashboard
- [ ] Live countdown timers for registered events
- [ ] Better empty and error states
- [ ] Keyboard-focus and accessibility review
- [ ] Download/print event pass

### 🚀 Phase 3 — Campus ecosystem

- [ ] Organizer dashboards and event publishing
- [ ] Backend database and student accounts
- [ ] Notifications and reminders
- [ ] Attendance check-in and QR passes
- [ ] Club profiles, recommendations, and event analytics

---

## 🏆 Hackathon Strategy

The project is deliberately focused on the judging priorities described in the competition rulebook:

| Priority | How College EventHub responds |
|---|---|
| Attractive UI/UX | A clean dark interface, visual hierarchy, event cards, responsive layouts, and feedback dialogs. |
| Functionality | Search, filtering, registration validation, IDs, local storage, and passes create a complete core flow. |
| Code quality | The prototype uses only HTML5, CSS3, and vanilla JavaScript with no unnecessary dependencies. |
| Responsiveness | Grid, flexbox, and breakpoints adapt the layout across common screen sizes. |
| Project justification | The problem, target user, and solution are straightforward to explain and defend. |

> **Do not build more. Build better.** Every feature should earn its place in the student journey.

---

## ❓ Judge Q&A

### Why did you build this?

Students miss opportunities because event information is scattered and hard to find.

### Who is the target user?

College students are the primary users. Clubs and departments are future organizer-side users.

### Why not use WhatsApp or Instagram?

They are useful for communication but poor for structured, searchable, and trackable event information. Important details can easily disappear in message threads or feeds.

### Why is there no backend?

This is a frontend prototype focused on validating the user experience and core flow. `localStorage` is enough to demonstrate saved registrations without server infrastructure.

### Why use vanilla JavaScript?

It keeps the project lightweight, easy to understand, and aligned with the hackathon’s frontend restrictions.

### What happens after registration?

The form validates the student’s information, generates a registration ID, saves the registration locally, updates the My Events count, and displays a digital event pass.

### What would you add next?

A complete My Events dashboard, countdowns, organizer tools, notifications, attendance tracking, and a real backend database.

---

## 🎤 One-Minute Pitch

> **College EventHub is a centralized event discovery and registration platform for college students. We identified that event information is scattered across WhatsApp groups, social media, notices, and different departments, which causes students to miss opportunities. EventHub brings these events into one platform where students can discover events, search and filter them, view complete details, register, receive a unique registration ID, and access a digital event pass. Our focus is to make campus participation simple, organized, and accessible through a clean, responsive, framework-free frontend.**

---

## 📌 Project Status

- **Stage:** Frontend prototype
- **Focus:** UI/UX, event discovery, and registration flow
- **Technology:** HTML5, CSS3, and Vanilla JavaScript
- **Platform:** Responsive web
- **Competition:** AVISHKAR 2026 — Frontend Web Development Hackathon

---

## 👨‍💻 Development Philosophy

> **Simple code. Clear purpose. Great experience.**

College EventHub is not designed to impress judges with unnecessary complexity. It is designed to show how a real student problem can be solved with good thinking, good design, and useful functionality.

---

### College EventHub — *Your campus. Your events. One place.*

**Discover → Register → Participate**
