# ImportNow Clone

A faithful, full replica of [ImportNow Concept](https://importnow-concept.vercel.app/#home) — end-to-end imports from China to India.

## 🚀 Features & Architecture

- **3D Interactive Earth (`assets/globe.js`)**:
  - Photorealistic Three.js Earth with custom day/night shader terminator.
  - Animated trade routes (Shanghai, Yiwu, Guangzhou, Shenzhen → Nhava Sheva, Chennai, Hyderabad, Vizag).
  - Dynamic city labels with collision avoidance and pulsing markers.
  - Interactive cursor tracking and tilt perspective.

- **3D Sea Voyage Simulation (`assets/voyage.js`)**:
  - Scroll-driven voyage simulator showing an order traveling from Shanghai to Chennai.
  - Realistic Three.js water surface shader (`Water.js`) and physical atmospheric sky (`Sky.js`).
  - Procedurally modeled container ship with custom hull textures, wake foam, STS port cranes, and loading animations.
  - Day counter and route tracker (`Day 0` through `Day 35`).

- **Landing Page Sections (`index.html`)**:
  - **Hero**: Value proposition, dual CTA buttons, key statistics with animated count-up (`500+` businesses, `83K+` community).
  - **Marquee**: Live trade route ticker (`Yiwu → Adilabad`, `Foshan → Hyderabad`, etc.).
  - **Services**: 6 core services (Product sourcing, Factory inspection, Quality control, Shipping & logistics, Customs clearance, Doorstep delivery) with 3D tilt cards.
  - **Journey**: Interactive 3D container ship voyage.
  - **What We Import**: Major Chinese manufacturing hubs (Foshan, Shenzhen, Guangzhou, Guzhen, Yiwu, Pan-China).
  - **Shanghai Company**: Official registered business licence verification stage with 3D perspective inspection.
  - **China Trips**: Guided Canton Fair & business tour packages.
  - **Proof of Work**: Recently delivered containers and case studies.
  - **Testimonials & Stories**: Real client experiences.
  - **Latest Guides**: Recent blog guides rendered dynamically.
  - **FAQ**: Interactive accordion addressing common importer questions.
  - **Contact & WhatsApp Quote Generator**: Pre-filled quotation inquiry form connected directly to WhatsApp.

- **Blog & Guides System (`blog.html` & `post.html`)**:
  - Category filters (Import guides, Wholesale markets, Product guides, Business ideas, China trips, Shipping, Customs).
  - Live client-side search across articles.
  - Dynamic pagination.
  - Full article view with automated Table of Contents (TOC), related articles, and social share links.
  - Preloaded with 8 comprehensive import guides in `assets/posts.js`.

- **Design System (`assets/site.css`)**:
  - Modern typography using Google Fonts (Sora & Inter).
  - Custom SVG sprite library embedded in `assets/site.js`.
  - Fully responsive across desktop, tablet, and mobile viewports.

## 💻 How to Run Locally

Because the 3D features use modern ES modules and Three.js import maps, serve the files with any local HTTP server:

```bash
# Using Python 3:
python3 -m http.server 8000

# Or using Node:
npx serve .
```

Then open `http://localhost:8000/` in your browser.
