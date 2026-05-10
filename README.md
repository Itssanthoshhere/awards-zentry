<div align="center">
  <br />
    <a href="/" target="_blank">
      <img src="https://github.com/user-attachments/assets/ab600f24-f4d9-4cef-8f1e-3fd9194afb30" alt="Project Banner">
    </a>
  <br />

# 🎮 Awards-Zentry

### A High-Fidelity GSAP-Powered Animated Landing Page Inspired by Awwwards-Level Design

[![React](https://img.shields.io/badge/React-19.2.5-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-8.0-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vite.dev)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-v4.2-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![GSAP](https://img.shields.io/badge/GSAP-3.15-88CE02?style=for-the-badge&logo=greensock&logoColor=black)](https://gsap.com)

> ✨ _Inspired by [Zentry](https://zentry.com) — Built to study and recreate award-winning frontend animation techniques._

<div align="center">
  <a href="https://awards-zentry-black.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/🚀%20Live%20Demo-brightgreen?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Demo" />
  </a>&nbsp;
  <a href="https://santhosh-vs-portfolio.vercel.app" target="_blank">
    <img src="https://img.shields.io/badge/🌐%20Portfolio-black?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>&nbsp;
  <a href="https://github.com/Itssanthoshhere" target="_blank">
    <img src="https://img.shields.io/badge/%20GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</div>

</div>

---

## 📋 Table of Contents

- [About The Project](#-about-the-project)
- [What I Learned](#-what-i-learned)
- [✨ Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [🏗️ Project Structure](#️-project-structure)
- [🚀 Getting Started](#-getting-started)
- [🎯 Key Components](#-key-components)
- [🧠 Animation Techniques](#-animation-techniques)
- [⚡ Performance Notes](#-performance-notes)
- [🔮 Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [📜 License & Attribution](#-license--attribution)

---

## 📖 About The Project

**awards-zentry** is a pixel-perfect, animation-rich recreation of Zentry's award-winning website — one of the most technically impressive landing pages in the gaming/metaverse space. This project was built as a **deep frontend study** to master:

- 🎬 Scroll-driven animations using **GSAP ScrollTrigger**
- 🌀 Complex **clip-path** and 3D CSS transform animations
- 🖱️ Mouse-tracking **perspective tilt** and **parallax** effects
- 🎥 Seamless **video transitions** with scale + clip animations
- 🏗️ Clean, **component-driven React architecture** for large creative UIs

> **Disclaimer:** This is a **study/portfolio project** inspired by [Zentry's](https://zentry.com) design. All original design credit belongs to the Zentry team. This implementation was built purely for educational purposes.

---

## 🧠 What I Learned

- How to structure complex GSAP timelines in React using `useGSAP`
- Managing performance in animation-heavy UIs (quickTo, avoiding re-renders)
- Designing reusable animation components (AnimatedTitle, VideoPreview)
- Balancing creativity and performance in modern frontend development

---

## ✨ Features

### 🎬 Hero Section

- Full-screen video background with **clip-path polygon transitions** on scroll
- Interactive **mini video preview** — click to cycle through 4 hero videos
- GSAP-powered scale animations as videos expand from thumbnail to fullscreen
- Custom loading overlay with a **three-body orbital spinner** (via Uiverse.io)

### 🔍 About Section

- **Scroll-pinned clip-path expansion** — image thumbnail grows from 30vw to 100vw as user scrolls
- 800px scroll distance mapped to full viewport fill via GSAP `scrub`
- `AnimatedTitle` 3D word-by-word fly-in animation

### 🃏 Features / Bento Grid

- **Mouse-tracking 3D perspective tilt** on each bento card
- 5x autoplay video cards with overlay UI
- Radial gradient cursor-following hover effect on "Coming Soon" buttons

### 📖 Story Section

- **3D floating image** with `rotateX/Y` GSAP mouse-tracking
- Custom SVG filter (`feGaussianBlur + feColorMatrix`) for organic rounded clip corners
- Diagonal clip-path image mask

### 🔗 Navbar

- Scroll-aware: **hides on scroll down, reappears on scroll up**
- Floating pill style with `border + bg-black` when scrolled
- Ambient **audio toggle** with animated bar indicators
- Hover underline animation on nav links

### 🖱️ Button Component

- **Dual-layer skew animation** — two stacked text elements slide with `skewY` transform
- Works with left and right icon slots

### 🦶 Footer

- Social links: Discord, Twitter, YouTube, Medium
- Clean responsive layout

---

## 🛠️ Tech Stack

| Category          | Technology                                          | Version | Purpose                                |
| ----------------- | --------------------------------------------------- | ------- | -------------------------------------- |
| **Build Tool**    | [Vite](https://vite.dev)                            | 8.0.10  | Fast HMR, native ESM bundling          |
| **UI Framework**  | [React](https://react.dev)                          | 19.2.5  | Component-driven UI                    |
| **Styling**       | [TailwindCSS v4](https://tailwindcss.com)           | 4.2.4   | Utility-first CSS with `@theme` tokens |
| **Animation**     | [GSAP](https://gsap.com)                            | 3.15.0  | ScrollTrigger, timelines, tweens       |
| **GSAP React**    | [@gsap/react](https://gsap.com/react)               | 2.1.2   | `useGSAP` hook with auto cleanup       |
| **Icons**         | [react-icons](https://react-icons.github.io)        | 5.6.0   | TiLocationArrow, FaDiscord, etc.       |
| **CSS Utilities** | [clsx](https://github.com/lukeed/clsx)              | 2.1.1   | Conditional className merging          |
| **Scroll Hook**   | [react-use](https://github.com/streamich/react-use) | 17.6.0  | `useWindowScroll`                      |

### Fonts Used

| Font                               | Usage                                |
| ---------------------------------- | ------------------------------------ |
| `zentry-regular`                   | Hero headings, special bold elements |
| `general`                          | Body text, nav links, labels         |
| `circular-web`                     | Section descriptions                 |
| `robert-medium` / `robert-regular` | Hero taglines                        |

---

## 🏗️ Project Structure

```
awards-zentry/
│
├── 📁 public/
│   ├── 📁 audio/
│   │   └── loop.mp3              # Ambient background audio
│   ├── 📁 fonts/                 # Custom .woff2 font files
│   │   ├── zentry-regular.woff2
│   │   ├── general.woff2
│   │   ├── circularweb-book.woff2
│   │   ├── robert-medium.woff2
│   │   └── robert-regular.woff2
│   ├── 📁 img/                   # Optimized .webp images
│   │   ├── about.webp
│   │   ├── contact-1.webp
│   │   ├── contact-2.webp
│   │   ├── entrance.webp
│   │   ├── swordman.webp
│   │   ├── swordman-partial.webp
│   │   └── logo.png
│   ├── 📁 videos/                # Hero & feature .mp4 videos
│   │   ├── hero-1.mp4 → hero-4.mp4
│   │   └── feature-1.mp4 → feature-5.mp4
│   └── favicon.svg
│
├── 📁 src/
│   ├── 📁 components/
│   │   ├── Navbar.jsx            # Sticky scroll-aware navigation
│   │   ├── Hero.jsx              # Full-screen video hero
│   │   ├── About.jsx             # Clip-path scroll expand
│   │   ├── AnimatedTitle.jsx     # Reusable 3D word animation
│   │   ├── Features.jsx          # Bento grid with tilt/hover
│   │   ├── Story.jsx             # 3D floating image section
│   │   ├── Contact.jsx           # CTA with clip-path images
│   │   ├── Footer.jsx            # Social links footer
│   │   ├── Button.jsx            # Animated skew button
│   │   └── VideoPreview.jsx      # Parallax 3D video wrapper
│   │
│   ├── App.jsx                   # Root layout composer
│   ├── main.jsx                  # React DOM entry point
│   └── index.css                 # Tailwind v4 + utilities + animations
│
├── index.html                    # HTML shell
├── vite.config.js                # Vite + React + Tailwind config
├── package.json
└── eslint.config.js
```

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

```
Node.js >= 18.0.0
npm >= 9.0.0
```

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/Itssanthoshhere/awards-zentry.git
cd awards-zentry
```

**2. Install dependencies**

```bash
npm install
```

**3. Start the development server**

```bash
npm run dev
```

Visit `http://localhost:5173` in your browser.

### Available Scripts

| Command           | Description                          |
| ----------------- | ------------------------------------ |
| `npm run dev`     | Start development server with HMR    |
| `npm run build`   | Build for production to `dist/`      |
| `npm run preview` | Preview the production build locally |
| `npm run lint`    | Run ESLint across all source files   |

### Production Build

```bash
npm run build
# Output: dist/ folder (ready to deploy)
```

### Deploy to Vercel (Recommended)

```bash
npm install -g vercel
vercel
# Follow prompts — select "Vite" framework preset
```

Or connect your GitHub repo directly at [vercel.com](https://vercel.com) for automatic deployments.

---

## 🎯 Key Components

### `<Hero />`

The most complex component. Manages:

- Video cycling state (4 videos, 1-indexed cycling)
- GSAP clip-path polygon scroll animation
- Mini-preview click → full-screen scale transition
- Loading gate (waits for 3 videos to load before showing UI)

```jsx
// Video cycling logic
const handleMiniVdClick = () => {
  setHasClicked(true);
  setCurrentIndex((prev) => (prev % totalVideos) + 1); // 1 → 2 → 3 → 4 → 1
};
```

### `<AnimatedTitle title="..." containerClass="..." />`

Reusable animated heading. Splits text by `<br />` and word, then animates each word from a 3D rotated position to flat with a stagger.

```jsx
// Usage
<AnimatedTitle
  title="Disc<b>o</b>ver the world's <br /> largest shared <b>a</b>dventure"
  containerClass="mt-5 !text-black text-center"
/>
```

- Supports `<b>` tags for **Zentry font** activation on specific letters
- Animated via GSAP ScrollTrigger — plays on scroll into view, reverses on scroll out

### `<BentoTilt className="...">` + `<BentoCard src title description isComingSoon />`

Two composable components for the features grid:

- `BentoTilt`: Wraps any content with mouse-tracking 3D perspective transform
- `BentoCard`: Renders video background with overlaid title, description, and optional "coming soon" button with radial gradient cursor effect

### `<Button id title leftIcon rightIcon containerClass />`

Fully reusable CTA button with skew slide animation on hover. Supports icon slots on both sides.

### `<VideoPreview>` (children)

Wraps content in a 3D parallax container — parent moves WITH cursor, children move AGAINST cursor, creating perceived depth.

---

## 🧠 Animation Techniques

### 1. Scroll-Pinned Clip-Path Expansion (About Section)

```javascript
gsap
  .timeline({
    scrollTrigger: {
      trigger: "#clip",
      start: "center center",
      end: "+=800 center",
      scrub: 0.5, // Smooth lag behind scroll position
      pin: true, // Pins section during animation
    },
  })
  .to(".mask-clip-path", {
    width: "100vw",
    height: "100vh",
    borderRadius: 0,
  });
```

### 2. 3D Word Stagger (AnimatedTitle)

Each word starts behind and rotated in Z-space:

```css
.animated-word {
  opacity: 0;
  transform: translate3d(10px, 51px, -60px) rotateY(60deg) rotateX(-40deg);
  transform-origin: 50% 50% -150px; /* Origin point behind the element */
}
```

GSAP animates them to `translate3d(0,0,0)` with a 20ms stagger per word.

### 3. Mouse-Tracking Tilt (BentoTilt)

```javascript
const relativeX = (event.clientX - rect.left) / rect.width; // 0–1
const relativeY = (event.clientY - rect.top) / rect.height; // 0–1

const tiltX = (relativeY - 0.5) * 5; // -2.5° to +2.5°
const tiltY = (relativeX - 0.5) * -5; // inverted axis

// Applied as: perspective(700px) rotateX(tiltX) rotateY(tiltY) scale3d(.95,.95,.95)
```

### 4. Video Transition (Hero)

When mini-video is clicked:

1. `#next-video` becomes visible
2. GSAP scales it from `size-64` to `100% x 100%` (1s)
3. `#current-video` scales from `0` to normal (1.5s, appears to shrink out)
4. Video `.play()` fires on animation start

### 5. VideoPreview Parallax

```javascript
// Parent: moves WITH cursor
gsap.to(sectionRef.current, { x: xOffset, y: yOffset, rotationY: xOffset / 2 });
// Child: moves AGAINST cursor (creates depth)
gsap.to(contentRef.current, { x: -xOffset, y: -yOffset });
```

---

## ⚡ Performance Notes

### Current Optimizations

- Videos use `loop muted autoPlay` — no audio decode cost
- GSAP uses `requestAnimationFrame` batching internally
- Vite produces optimized chunks in production build
- `.webp` format for all images (vs PNG/JPG)

### Known Performance Considerations

- **4 videos load simultaneously** in Hero — high bandwidth on first visit
- **5 feature videos autoplay** — continuous GPU decode; consider pausing off-screen videos
- `getBoundingClientRect()` called on every `mousemove` in BentoTilt — consider caching the rect value

### Recommended `vercel.json` for Asset Caching

```json
{
  "headers": [
    {
      "source": "/fonts/(.*)",
      "headers": [
        {
          "key": "Cache-Control",
          "value": "public, max-age=31536000, immutable"
        }
      ]
    },
    {
      "source": "/videos/(.*)",
      "headers": [{ "key": "Cache-Control", "value": "public, max-age=86400" }]
    },
    {
      "source": "/img/(.*)",
      "headers": [{ "key": "Cache-Control", "value": "public, max-age=604800" }]
    }
  ]
}
```

---

## 🔮 Roadmap

- [ ] **TypeScript migration** — add `interface` definitions for all component props
- [ ] **Test suite** — Vitest unit tests + Playwright E2E
- [ ] **Accessibility** — keyboard navigation, ARIA labels, `prefers-reduced-motion` support
- [ ] **SEO** — Open Graph tags, Twitter card meta, sitemap
- [ ] **Mobile** — Touch event support for VideoPreview parallax
- [ ] **WebM videos** — Smaller file sizes than MP4 for web delivery
- [ ] **Lazy loading** — `React.lazy()` for below-fold sections
- [ ] **Error boundaries** — Graceful fallback if video fails to load

---

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/amazing-animation`
3. Commit your changes: `git commit -m 'Add: parallax hero scroll effect'`
4. Push to the branch: `git push origin feature/amazing-animation`
5. Open a Pull Request

---

## 👨‍💻 Author

**V S Santhosh (Sandyy)**

- 🌐 Portfolio: [santhosh-vs-portfolio.vercel.app](https://santhosh-vs-portfolio.vercel.app)
- 💼 LinkedIn: [@thesanthoshvs](https://linkedin.com/in/thesanthoshvs)
- 🐙 GitHub: [@Itssanthoshhere](https://github.com/Itssanthoshhere)
- 🎓 BTech CSE (AI) — Bennett University, Batch 2023–2027

---

## 📜 License & Attribution

This project is for **educational and portfolio purposes only**.

- **Design Inspiration**: [Zentry](https://zentry.com) — All original design concepts belong to the Zentry team
- **Loader Animation**: [Uiverse.io by G4b413l](https://uiverse.io/G4b413l/tidy-walrus-92)
- **Fonts**: Zentry, General Sans, Circular Web, Robert (used under fair use for study)
- **Code**: MIT License — feel free to learn from and build upon this implementation

---

<div align="center">

**⭐ If this project helped you learn GSAP animations or React patterns, please give it a star!**

Made with ❤️ by Itssanthoshhere

</div>
