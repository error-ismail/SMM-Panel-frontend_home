# 🚀 SMM Hero

### Modern SMM Panel Landing Page for Social Media Growth

<p align="center">
  <img src="https://img.shields.io/badge/React-19.1-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/>
  <img src="https://img.shields.io/badge/Vite-7.1-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>
  <img src="https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/CSS3-Responsive-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
</p>

<p align="center">
  <b>A polished, responsive SMM panel landing page built with React and Vite.</b>
</p>

---

## 🌐 Overview

**SMM Hero** is a modern single-page landing website for a social media marketing panel. It presents social media growth services, platform-specific offerings, the ordering process, payment methods, growth strategy, service advantages, FAQs, and a conversion-focused CTA.

The project is built as a component-based React application with reusable data, custom hooks, responsive layouts, and an asset-driven visual system.

> **Note:** This repository contains the frontend landing page only. The buttons, navigation links, and service information are currently presentation/demo flows rather than a complete SMM ordering backend.

---

# ✨ Features

## 🏠 Hero Section

- Brand/navigation header
- Social platform highlights
- Customer rating presentation
- Primary and secondary CTA buttons
- Responsive hero artwork
- Social platform shortcut icons

## 📊 Statistics

- Animated order counter
- Available services counter
- Registered users counter
- Regional ranking highlight
- Scroll-triggered presentation

## 📱 Platform Services

The services section covers multiple social platforms:

- Facebook
- Instagram
- X (Twitter)
- YouTube
- TikTok
- LinkedIn
- Telegram
- Discord
- Spotify
- SoundCloud
- Snapchat
- Website Traffic

Each platform has its own service description and list of available service types.

## ⚙️ Working Process

The landing page explains the SMM workflow in four steps:

```text
┌────────────────┐
│ 01 Create      │
│    Account     │
└───────┬────────┘
        │
        ▼
┌────────────────┐
│ 02 Add Funds   │
└───────┬────────┘
        │
        ▼
┌────────────────┐
│ 03 Select      │
│    Service     │
└───────┬────────┘
        │
        ▼
┌────────────────┐
│ 04 Place       │
│    Order       │
└────────────────┘
```

## 💳 Payment Methods

A dedicated payment section visually presents supported payment methods, including:

- Visa
- Mastercard
- SEPA
- Instant Deposit
- Google Pay
- Apple Pay
- PayPal

The section includes the Bangladesh map/radar visual and animated payment badges.

## 📈 Social Media Growth Strategy

The growth section presents a staged strategy:

```text
Weeks 1–2
   │
   ▼
Initial SMM Momentum
   │
   ▼
Weeks 3–4
   │
   ▼
Consistent Content
   │
   ▼
Months 2–3
   │
   ▼
Content + Light Support
   │
   ▼
Months 3–6
   │
   ▼
Organic Growth Focus
```

## 🛡️ Advantages

The page highlights four major selling points:

- No password requirement
- Real-user focused messaging
- Gradual delivery
- Track-record based credibility

## ❓ FAQ

Interactive FAQ accordion covering common questions about:

- Followers and engagement
- Delivery time
- Drip-feed delivery
- Daily ordering
- Agency usage
- Engagement retention
- Platform selection

## 🎯 CTA & Footer

- Final conversion-focused CTA
- Service shortcut
- Account CTA
- Social links
- Quick links
- Service links
- Contact information

---

# 🧩 Application Architecture

```text
                         React Application
                                │
                                ▼
                            App.jsx
                                │
          ┌─────────────────────┼─────────────────────┐
          │                     │                     │
          ▼                     ▼                     ▼
        Hero                  Stats                Services
          │                     │                     │
          ▼                     ▼                     ▼
       Header              useCountUp             content.js
                                │
                                │
          ┌─────────────────────┼─────────────────────┐
          │                     │                     │
          ▼                     ▼                     ▼
       Process              Payments               Growth
          │                     │                     │
          └─────────────────────┼─────────────────────┘
                                │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
          Advantages           FAQ              CTA
              │                │                │
              └────────────────┼────────────────┘
                               ▼
                            Footer
```

---

# 🏗️ Component Structure

```text
src/
│
├── App.jsx
├── main.jsx
│
├── components/
│   ├── Header.jsx
│   ├── Footer.jsx
│   └── SectionHeading.jsx
│
├── sections/
│   ├── Hero.jsx
│   ├── Stats.jsx
│   ├── Services.jsx
│   ├── Process.jsx
│   ├── Payments.jsx
│   ├── Growth.jsx
│   ├── Advantages.jsx
│   ├── Faq.jsx
│   └── Cta.jsx
│
├── data/
│   └── content.js
│
├── hooks/
│   ├── useCountUp.js
│   └── useInView.js
│
├── assets/
│   └── images/
│
└── styles.css
```

---

# 🔄 Data & UI Flow

The project keeps most of the page content in a centralized data file instead of hard-coding repeated content inside individual sections.

```text
                 content.js
                     │
        ┌────────────┼────────────┐
        │            │            │
        ▼            ▼            ▼
      Hero         Services      Stats
        │            │            │
        └────────────┼────────────┘
                     │
                     ▼
               React Components
                     │
                     ▼
                Rendered UI
```

This structure makes the landing page easier to maintain and update without changing the component logic.

---

# 🎨 Design System

The existing design is intentionally preserved and built around:

- Orange gradient accents
- Warm cream backgrounds
- Dark navy typography
- Rounded cards and buttons
- Soft shadows
- Responsive grid layouts
- Custom illustrations and platform artwork
- Scroll and hover interactions
- Reduced-motion support for selected animations

**No design system or visual layout is changed by this repository cleanup.**

---

# 🛠️ Tech Stack

### Frontend

- React 19
- JavaScript ES Modules
- CSS3
- HTML5

### Build Tool

- Vite 7

### Development

- npm
- ESLint-ready project structure
- Component-based architecture
- Custom React hooks

### Assets

- WebP
- PNG
- SVG-style CSS effects and gradients

---

# 📂 Project Structure

```text
smm-hero/
│
├── public/
│   └── hero.webp
│
├── src/
│   ├── assets/
│   │   └── images/
│   ├── components/
│   ├── data/
│   ├── hooks/
│   ├── sections/
│   ├── App.jsx
│   ├── main.jsx
│   └── styles.css
│
├── .gitignore
├── index.html
├── netlify.toml
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

### Why `node_modules` and `dist` are not included

They are generated/local build artifacts and should not be committed to GitHub.

- `node_modules/` → recreated with `npm install`
- `dist/` → recreated with `npm run build`

---

# 🚀 Getting Started

## Prerequisites

Make sure you have installed:

- Node.js 18+
- npm

## 1. Clone the Repository

```bash
git clone https://github.com/ilovectg/smm-hero.git
cd smm-hero
```

## 2. Install Dependencies

```bash
npm install
```

## 3. Start Development Server

```bash
npm run dev
```

Vite will start the development server, normally at:

```text
http://localhost:5173
```

## 4. Create Production Build

```bash
npm run build
```

## 5. Preview Production Build

```bash
npm run preview
```

---

# ☁️ Netlify Deployment

This project is configured for Netlify with:

```text
Build command: npm run build
Publish directory: dist
```

The repository includes a `netlify.toml` file so these settings can be detected automatically.

### Deploy from GitHub

1. Push the project to GitHub.
2. Open Netlify.
3. Select **Add new project → Import an existing project**.
4. Connect the GitHub repository.
5. Confirm the build command:

```text
npm run build
```

6. Confirm the publish directory:

```text
dist
```

7. Deploy the site.

Every new GitHub push can then trigger a new Netlify deployment.

---

# 🧠 Technical Highlights

### Reusable Components

Common UI patterns are separated into reusable components such as `Header`, `Footer`, and `SectionHeading`.

### Data-Driven Sections

Service platforms, FAQs, payment methods, statistics, navigation, and other repeated content are maintained in `src/data/content.js`.

### Custom Hooks

The project includes:

- `useCountUp` for animated statistics
- `useInView` for viewport-based interactions

### Responsive Layout

The layout uses CSS grid, flexbox, responsive breakpoints, scalable typography, and fluid visual sizing to support different screen sizes.

---

# 📌 Current Scope

This repository focuses on the **frontend presentation and landing-page experience**.

It does not currently include:

- User authentication backend
- Real order processing
- Payment gateway integration
- Customer dashboard
- SMM provider API integration
- Database/backend service

These can be added later without requiring the existing visual sections to be redesigned.

---

# 🔮 Future Improvements

- [ ] Connect real authentication
- [ ] Add customer dashboard
- [ ] Integrate SMM provider APIs
- [ ] Add real order management
- [ ] Add payment gateway integration
- [ ] Add service search and filtering
- [ ] Add user order tracking
- [ ] Add backend API
- [ ] Add database integration
- [ ] Add automated testing

---

# 📈 Project Flow

```text
                    🌐 Landing Page
                          │
                          ▼
                    🏠 Hero Section
                          │
                          ▼
                    📊 Statistics
                          │
                          ▼
                   📱 SMM Services
                          │
                          ▼
                   ⚙️ Working Process
                          │
                          ▼
                    💳 Payments
                          │
                          ▼
                    📈 Growth Plan
                          │
                          ▼
                    🛡️ Advantages
                          │
                          ▼
                       ❓ FAQ
                          │
                          ▼
                       🎯 CTA
                          │
                          ▼
                      🧾 Footer
```

---

# 🎯 Project Highlights

```text
┌──────────────────────────────────────────────┐
│                  🚀 SMM HERO                 │
├──────────────────────────────────────────────┤
│                                              │
│  ⚛️ React + Vite Frontend                   │
│  📱 Multi-Platform SMM Services              │
│  📊 Animated Statistics                      │
│  ⚙️ 4-Step Ordering Process                 │
│  💳 Payment Method Showcase                  │
│  📈 Growth Strategy                          │
│  🛡️ Service Advantages                      │
│  ❓ Interactive FAQ                          │
│  🎯 Conversion-Focused CTA                   │
│  📱 Responsive Layout                        │
│                                              │
└──────────────────────────────────────────────┘
```

---

# 👨‍💻 Author

**ilovectg**

Built as a modern React frontend project with a focus on clean component structure, responsive UI, reusable content, and polished visual presentation.

---

<p align="center">
  <b>⚡ Fast UI. 📱 Social Growth. 🚀 Modern React.</b>
</p>
'''
# normalize package name only? keep existing to avoid unintended change
