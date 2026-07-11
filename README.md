<svg width="1000" height="300" viewBox="0 0 1000 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Muhammad Daud Razzaq Khan — Mobile and Frontend Engineer">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#050810"/>
      <stop offset="55%" stop-color="#0a0f1e"/>
      <stop offset="100%" stop-color="#0d1630"/>
    </linearGradient>

    <!-- Animated shimmer gradient for the name -->
    <linearGradient id="shine" gradientUnits="userSpaceOnUse" x1="0" y1="0" x2="500" y2="0" spreadMethod="reflect">
      <stop offset="0%" stop-color="#ffffff"/>
      <stop offset="45%" stop-color="#00d4ff"/>
      <stop offset="55%" stop-color="#7b61ff"/>
      <stop offset="100%" stop-color="#ffffff"/>
      <animateTransform attributeName="gradientTransform" type="translate" from="0 0" to="1000 0" dur="6s" repeatCount="indefinite"/>
    </linearGradient>

    <!-- Glow filter -->
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="6" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Soft radial light behind content -->
    <radialGradient id="halo" cx="50%" cy="40%" r="60%">
      <stop offset="0%" stop-color="#00d4ff" stop-opacity="0.10"/>
      <stop offset="60%" stop-color="#7b61ff" stop-opacity="0.04"/>
      <stop offset="100%" stop-color="#000000" stop-opacity="0"/>
    </radialGradient>
  </defs>

  <!-- Base -->
  <rect width="1000" height="300" rx="16" fill="url(#bg)"/>
  <rect width="1000" height="300" rx="16" fill="url(#halo)"/>

  <!-- Subtle grid lines -->
  <g stroke="#1c2a4a" stroke-width="1" opacity="0.35">
    <line x1="0" y1="75"  x2="1000" y2="75"/>
    <line x1="0" y1="150" x2="1000" y2="150"/>
    <line x1="0" y1="225" x2="1000" y2="225"/>
    <line x1="200" y1="0" x2="200" y2="300"/>
    <line x1="400" y1="0" x2="400" y2="300"/>
    <line x1="600" y1="0" x2="600" y2="300"/>
    <line x1="800" y1="0" x2="800" y2="300"/>
  </g>

  <!-- Floating particles -->
  <g>
    <circle cx="120" cy="70" r="3" fill="#00d4ff" opacity="0.6">
      <animate attributeName="cy" values="70;45;70" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.6;0.15;0.6" dur="7s" repeatCount="indefinite"/>
    </circle>
    <circle cx="880" cy="90" r="4" fill="#7b61ff" opacity="0.5">
      <animate attributeName="cy" values="90;120;90" dur="9s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.5;0.1;0.5" dur="9s" repeatCount="indefinite"/>
    </circle>
    <circle cx="180" cy="230" r="2.5" fill="#00d4ff" opacity="0.5">
      <animate attributeName="cy" values="230;205;230" dur="6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="820" cy="220" r="2.5" fill="#00d4ff" opacity="0.45">
      <animate attributeName="cy" values="220;248;220" dur="8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="60" cy="160" r="2" fill="#7b61ff" opacity="0.4">
      <animate attributeName="cy" values="160;135;160" dur="10s" repeatCount="indefinite"/>
    </circle>
    <circle cx="945" cy="160" r="2" fill="#7b61ff" opacity="0.4">
      <animate attributeName="cy" values="160;188;160" dur="11s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Corner brackets -->
  <g stroke="#00d4ff" stroke-width="2.5" fill="none" opacity="0.8">
    <path d="M 28 52 L 28 30 L 50 30"/>
    <path d="M 950 30 L 972 30 L 972 52"/>
    <path d="M 972 248 L 972 270 L 950 270"/>
    <path d="M 50 270 L 28 270 L 28 248"/>
  </g>

  <!-- Name with shimmer -->
  <text x="500" y="118" text-anchor="middle"
        font-family="Segoe UI, Helvetica, Arial, sans-serif"
        font-size="44" font-weight="800" letter-spacing="3"
        fill="url(#shine)" filter="url(#glow)">MUHAMMAD DAUD RAZZAQ KHAN</text>

  <!-- Subtitle -->
  <text x="500" y="156" text-anchor="middle"
        font-family="Segoe UI, Helvetica, Arial, sans-serif"
        font-size="19" font-weight="600" letter-spacing="4"
        fill="#a0aec0">MOBILE &amp; FRONTEND ENGINEER</text>

  <!-- Pulsing accent line -->
  <rect x="400" y="172" width="200" height="3" rx="1.5" fill="#00d4ff">
    <animate attributeName="opacity" values="0.35;1;0.35" dur="2.6s" repeatCount="indefinite"/>
    <animate attributeName="x" values="400;390;400" dur="2.6s" repeatCount="indefinite"/>
    <animate attributeName="width" values="200;220;200" dur="2.6s" repeatCount="indefinite"/>
  </rect>

  <!-- Rotating specialties with blinking cursor -->
  <g font-family="Consolas, Menlo, monospace" font-size="22" font-weight="600" text-anchor="middle">
    <text x="500" y="216" fill="#00d4ff" opacity="0">
      &lt;React Native /&gt;
      <animate attributeName="opacity" values="0;1;1;0;0" keyTimes="0;0.04;0.29;0.33;1" dur="12s" repeatCount="indefinite"/>
    </text>
    <text x="500" y="216" fill="#7b61ff" opacity="0">
      &lt;Next.js /&gt;
      <animate attributeName="opacity" values="0;1;1;0;0" keyTimes="0;0.04;0.29;0.33;1" dur="12s" begin="4s" repeatCount="indefinite"/>
    </text>
    <text x="500" y="216" fill="#00d4ff" opacity="0">
      &lt;AI Integration /&gt;
      <animate attributeName="opacity" values="0;1;1;0;0" keyTimes="0;0.04;0.29;0.33;1" dur="12s" begin="8s" repeatCount="indefinite"/>
    </text>
  </g>
  <rect x="618" y="200" width="3" height="20" fill="#00d4ff">
    <animate attributeName="opacity" values="1;0;1" dur="1.1s" repeatCount="indefinite"/>
  </rect>

  <!-- Footer stats line -->
  <text x="500" y="256" text-anchor="middle"
        font-family="Segoe UI, Helvetica, Arial, sans-serif"
        font-size="15" font-weight="500" letter-spacing="1"
        fill="#5a6a8a">20+ PRODUCTS SHIPPED&#160;&#160;&#8226;&#160;&#160;5 COUNTRIES&#160;&#160;&#8226;&#160;&#160;OPEN TO SAUDI ARABIA &#127480;&#127462;</text>
</svg>
<div align="center">

<!-- ═══════════════ ANIMATED HEADER (self-hosted SVG — loads 100% reliably, no third-party API) ═══════════════ -->

<img src="./header.svg" width="100%" alt="Muhammad Daud Razzaq Khan — Mobile &amp; Frontend Engineer · React Native · Next.js · AI Integration"/>

<br/><br/>

<!-- ═══════════════ CONTACT BADGES ═══════════════ -->

<a href="https://daudrazzaq.me"><img src="https://img.shields.io/badge/Portfolio-daudrazzaq.me-00d4ff?style=for-the-badge&amp;logo=vercel&amp;logoColor=white&amp;labelColor=0a0f1e" alt="Portfolio"/></a>
<a href="https://linkedin.com/in/daud-razzaq-3a3892233"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077b5?style=for-the-badge&amp;logo=linkedin&amp;logoColor=white&amp;labelColor=0a0f1e" alt="LinkedIn"/></a>
<a href="mailto:daudrazzaq7890@gmail.com"><img src="https://img.shields.io/badge/Email-Hire_Me-ea4335?style=for-the-badge&amp;logo=gmail&amp;logoColor=white&amp;labelColor=0a0f1e" alt="Email"/></a>

</div>

<br/>

<!-- ═══════════════ ABOUT ═══════════════ -->

## 🚀 About Me

```typescript
const daud = {
  role: "Mobile & Frontend Engineer",
  experience: "3.5+ years · 3 product companies + freelance for global clients",
  location: "Lahore, Pakistan → relocating to Riyadh, Saudi Arabia 🇸🇦",

  code: ["TypeScript", "JavaScript", "Python", "SQL"],
  mobile: ["React Native", "Expo", "Native Modules", "Store Releases"],
  web: ["Next.js", "React", "Tailwind", "Framer Motion", "SEO-first builds"],
  ai: ["LLM Chatbots (Gemini)", "Computer Vision (OpenCV, MediaPipe)", "Whisper", "PyTorch"],

  shipped: "20+ products for clients in USA, UK, UAE, Canada & Australia",
  liveOnStores: "WholesaleEZ — App Store & Google Play",
  arabicMarkets: "Bilingual EN/AR apps with full RTL support (MENA)",

  certifications: ["Meta React Native Specialization", "IBM Front-End with React"],
  education: "B.S. Software Engineering — COMSATS University (2021–2025)",
};
```

- 🔭 **Freelance Full-Stack Web &amp; Mobile Developer** — delivering end-to-end for clients across the US, UK, UAE, Canada &amp; Australia
- 📱 **WholesaleEZ** live in production on the **[App Store](https://apps.apple.com/my/app/wholesale-ez/id1592556878)** and **[Google Play](https://play.google.com/store/apps/details?id=wholesaleez.wholesaleezapp.supplierapp)** — real users, not demos
- 🤖 Deep in **AI-integrated products**: LLM chatbots, emotion detection, speech transcription pipelines
- 🌙 Obsessed with **premium UI/UX** — glassmorphism, 60fps Reanimated transitions, dark-mode design systems
- ⚡ Performance focused: **100/100 Lighthouse SEO**, latency reduction, Core Web Vitals
- 🇸🇦 **Open to on-site roles in Riyadh &amp; Jeddah** — available on short notice

<br/>

<!-- ═══════════════ TECH STACK ═══════════════ -->

## 🛠️ Tech Arsenal

<div align="center">

### 📱 Mobile

<img src="https://img.shields.io/badge/React_Native-20232a?style=for-the-badge&amp;logo=react&amp;logoColor=61dafb" alt="React Native"/> <img src="https://img.shields.io/badge/Expo-000020?style=for-the-badge&amp;logo=expo&amp;logoColor=white" alt="Expo"/> <img src="https://img.shields.io/badge/TypeScript-3178c6?style=for-the-badge&amp;logo=typescript&amp;logoColor=white" alt="TypeScript"/> <img src="https://img.shields.io/badge/Redux-764abc?style=for-the-badge&amp;logo=redux&amp;logoColor=white" alt="Redux"/> <img src="https://img.shields.io/badge/React_Query-ff4154?style=for-the-badge&amp;logo=reactquery&amp;logoColor=white" alt="React Query"/>

### 🌐 Web / Frontend

<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&amp;logo=next.js&amp;logoColor=white" alt="Next.js"/> <img src="https://img.shields.io/badge/React-20232a?style=for-the-badge&amp;logo=react&amp;logoColor=61dafb" alt="React"/> <img src="https://img.shields.io/badge/Tailwind_CSS-06b6d4?style=for-the-badge&amp;logo=tailwindcss&amp;logoColor=white" alt="Tailwind CSS"/> <img src="https://img.shields.io/badge/Framer_Motion-0055ff?style=for-the-badge&amp;logo=framer&amp;logoColor=white" alt="Framer Motion"/> <img src="https://img.shields.io/badge/JavaScript-f7df1e?style=for-the-badge&amp;logo=javascript&amp;logoColor=black" alt="JavaScript"/>

### 🤖 AI &amp; Emerging Tech

<img src="https://img.shields.io/badge/Gemini_AI-8e75b2?style=for-the-badge&amp;logo=googlegemini&amp;logoColor=white" alt="Gemini"/> <img src="https://img.shields.io/badge/OpenCV-5c3ee8?style=for-the-badge&amp;logo=opencv&amp;logoColor=white" alt="OpenCV"/> <img src="https://img.shields.io/badge/PyTorch-ee4c2c?style=for-the-badge&amp;logo=pytorch&amp;logoColor=white" alt="PyTorch"/> <img src="https://img.shields.io/badge/MediaPipe-0097a7?style=for-the-badge&amp;logo=google&amp;logoColor=white" alt="MediaPipe"/> <img src="https://img.shields.io/badge/Whisper-412991?style=for-the-badge&amp;logo=openai&amp;logoColor=white" alt="Whisper"/> <img src="https://img.shields.io/badge/Web3_/_Solidity-363636?style=for-the-badge&amp;logo=solidity&amp;logoColor=white" alt="Web3 Solidity"/>

### ⚙️ Backend &amp; Cloud

<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&amp;logo=node.js&amp;logoColor=white" alt="Node.js"/> <img src="https://img.shields.io/badge/Python-3776ab?style=for-the-badge&amp;logo=python&amp;logoColor=white" alt="Python"/> <img src="https://img.shields.io/badge/Firebase-ffca28?style=for-the-badge&amp;logo=firebase&amp;logoColor=black" alt="Firebase"/> <img src="https://img.shields.io/badge/MongoDB-47a248?style=for-the-badge&amp;logo=mongodb&amp;logoColor=white" alt="MongoDB"/> <img src="https://img.shields.io/badge/Django-092e20?style=for-the-badge&amp;logo=django&amp;logoColor=white" alt="Django"/> <img src="https://img.shields.io/badge/Stripe-635bff?style=for-the-badge&amp;logo=stripe&amp;logoColor=white" alt="Stripe"/>

### 🚀 Infrastructure &amp; DevOps

<img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&amp;logo=vercel&amp;logoColor=white" alt="Vercel"/> <img src="https://img.shields.io/badge/Cloudflare_R2-f38020?style=for-the-badge&amp;logo=cloudflare&amp;logoColor=white" alt="Cloudflare R2"/> <img src="https://img.shields.io/badge/Resend-000000?style=for-the-badge&amp;logo=resend&amp;logoColor=white" alt="Resend"/> <img src="https://img.shields.io/badge/Git-f05032?style=for-the-badge&amp;logo=git&amp;logoColor=white" alt="Git"/> <img src="https://img.shields.io/badge/CI/CD-2088ff?style=for-the-badge&amp;logo=githubactions&amp;logoColor=white" alt="CI/CD"/>

</div>

<br/>

<!-- ═══════════════ FEATURED PROJECTS ═══════════════ -->

## 📌 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🏪 WholesaleEZ
**B2B Commerce &amp; Inventory Platform — LIVE IN PRODUCTION**

Enterprise-grade wholesale marketplace: RBAC for suppliers/vendors/warehouses, multi-warehouse real-time inventory, QuickBooks financial sync, secure payments &amp; automated PDF invoicing.

`React Native` `TypeScript` `Django` `Redux/Zustand` `QuickBooks API`

<a href="https://apps.apple.com/my/app/wholesale-ez/id1592556878"><img src="https://img.shields.io/badge/App_Store-LIVE-0d96f6?style=flat-square&amp;logo=appstore&amp;logoColor=white" alt="App Store"/></a> <a href="https://play.google.com/store/apps/details?id=wholesaleez.wholesaleezapp.supplierapp"><img src="https://img.shields.io/badge/Google_Play-LIVE-414141?style=flat-square&amp;logo=googleplay&amp;logoColor=white" alt="Google Play"/></a>

</td>
<td width="50%" valign="top">

### 🌍 ZolMarket
**Bilingual English/Arabic Marketplace (MENA)**

Fully bilingual EN/AR classifieds with right-to-left (RTL) layouts — moderated listings, in-chat price negotiation, seller reputation, and Stripe-powered featured ads.

`React Native` `TypeScript` `Firebase` `Stripe` `Cloudflare R2`

<a href="https://daudrazzaq.me/work/zolmarket"><img src="https://img.shields.io/badge/Case_Study-daudrazzaq.me-00d4ff?style=flat-square&amp;logo=vercel&amp;logoColor=white" alt="Case Study"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔮 Ethereya
**AI Wellness App with Premium Subscriptions**

Subscription-based AI guidance app: LLM-generated personalized reports, conversational AI chatbot with file uploads, glassmorphic UI with fluid Reanimated transitions.

`React Native` `TypeScript` `TanStack Query` `Reanimated` `LLM`

<a href="https://daudrazzaq.me/work/ethereya"><img src="https://img.shields.io/badge/Case_Study-daudrazzaq.me-00d4ff?style=flat-square&amp;logo=vercel&amp;logoColor=white" alt="Case Study"/></a>

</td>
<td width="50%" valign="top">

### 🎯 AI Interview Facilitator
**Computer Vision + LLM Interview Platform**

AI mock-interview system: Gemini-tailored questions from resume parsing, Whisper speech transcription, MediaPipe emotion/non-verbal analysis → objective evaluation reports. ~95% expression-recognition accuracy.

`React Native` `Python` `Gemini` `Whisper` `MediaPipe` `PyTorch`

<a href="https://daudrazzaq.me/work/ai-interview-facilitator"><img src="https://img.shields.io/badge/Case_Study-daudrazzaq.me-00d4ff?style=flat-square&amp;logo=vercel&amp;logoColor=white" alt="Case Study"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏛️ Aureon Studio — *Client Project*
**SEO-First Production Website — LIVE**

Designed and developed the production Next.js website for a London interior-architecture firm: structured data, fluid Framer Motion animations, enquiry + WhatsApp conversion flow. **100/100 Lighthouse SEO.**

`Next.js` `React` `Framer Motion` `Vercel` `Resend`

<a href="https://aureonstudio.co.uk"><img src="https://img.shields.io/badge/Live-aureonstudio.co.uk-00c853?style=flat-square&amp;logo=googlechrome&amp;logoColor=white" alt="Live Site"/></a>

</td>
<td width="50%" valign="top">

### 🍽️ Meal Mate
**AI Food &amp; Nutrition App**

Snap a photo → instant meal identification and nutrition breakdown. AI recipe generation from your pantry, calorie tracking, streaks &amp; grocery lists. Vision backend in FastAPI + PyTorch.

`React Native` `TypeScript` `Python` `FastAPI` `PyTorch`

<a href="https://daudrazzaq.me/work/meal-mate"><img src="https://img.shields.io/badge/Case_Study-daudrazzaq.me-00d4ff?style=flat-square&amp;logo=vercel&amp;logoColor=white" alt="Case Study"/></a>

</td>
</tr>
</table>

<div align="center">

**➕ More projects:** TrendUp (Web3 social) · Cleaners Choice (on-demand services) · Luci (booking marketplace, EN/TH) · Cafena (Next.js e-commerce)

<a href="https://daudrazzaq.me/work"><img src="https://img.shields.io/badge/View_All_Projects-daudrazzaq.me/work-00d4ff?style=for-the-badge&amp;logo=safari&amp;logoColor=white&amp;labelColor=0a0f1e" alt="View All Projects"/></a>

</div>

<br/>

<!-- ═══════════════ EXPERIENCE ═══════════════ -->

## 💼 Experience

| | Role | Company | Period |
|---|---|---|---|
| 🟢 | **Freelance Full-Stack Developer** | Independent — Web &amp; Mobile · Global Clients (US, UK, UAE, CA, AU) | 2021 – Present |
| 🔵 | **React Native Developer** | Webexhaust — Remote | Oct 2025 – Jun 2026 |
| 🔵 | **React Native Developer** | 7 Kings Code — Lahore | Mar 2025 – Sep 2025 |
| 🔵 | **React Native Developer** | Wise360 Solutions — Abbottabad *(cut app load times ~30%)* | Feb 2023 – Mar 2025 |

<br/>

<!-- ═══════════════ CERTIFICATIONS ═══════════════ -->

## 📜 Certifications &amp; Education

<div align="center">

<a href="https://coursera.org/verify/specialization/DS8NWQGQNBAB"><img src="https://img.shields.io/badge/Meta-React_Native_Specialization_(8_courses)-0668e1?style=for-the-badge&amp;logo=meta&amp;logoColor=white&amp;labelColor=0a0f1e" alt="Meta React Native Specialization"/></a>

<a href="https://coursera.org/verify/WTJPNLAKXVDM"><img src="https://img.shields.io/badge/IBM-Front--End_Apps_with_React-054ada?style=for-the-badge&amp;logo=ibm&amp;logoColor=white&amp;labelColor=0a0f1e" alt="IBM Front-End with React"/></a>

<a href="https://coursera.org/verify/MLHJ3WLFKJGP"><img src="https://img.shields.io/badge/Meta-Intro_to_Front--End_Development-0668e1?style=for-the-badge&amp;logo=meta&amp;logoColor=white&amp;labelColor=0a0f1e" alt="Meta Intro to Front-End"/></a>

🎓 **B.S. Software Engineering** — COMSATS University Islamabad · 2021–2025

</div>

<br/>

---

<!-- ═══════════════ FOOTER / CTA ═══════════════ -->

<div align="center">

## 🤝 Let's Build Something World-Class

**🇸🇦 Actively seeking Senior React Native / Next.js roles in Riyadh &amp; Jeddah**

Fluent in **English** &amp; **Urdu** · Arabic-market product experience · Available on short notice

<br/>

<a href="https://daudrazzaq.me/contact"><img src="https://img.shields.io/badge/💬_Start_a_Conversation-daudrazzaq.me/contact-00d4ff?style=for-the-badge&amp;labelColor=0a0f1e" alt="Contact"/></a>
<a href="mailto:daudrazzaq7890@gmail.com"><img src="https://img.shields.io/badge/📧_Email-daudrazzaq7890@gmail.com-ea4335?style=for-the-badge&amp;labelColor=0a0f1e" alt="Email"/></a>

<br/><br/>

⭐ *If my work interests you, check out* **[daudrazzaq.me](https://daudrazzaq.me)** *for live demos*

<!-- ═══════════════ ANIMATED FOOTER (self-hosted SVG) ═══════════════ -->

<img src="./footer.svg" width="100%" alt="footer"/>

</div>

<svg width="1000" height="90" viewBox="0 0 1000 90" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="footer">
  <defs>
    <linearGradient id="fbg" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#050810"/>
      <stop offset="50%" stop-color="#0a0f1e"/>
      <stop offset="100%" stop-color="#050810"/>
    </linearGradient>
  </defs>
  <rect width="1000" height="90" rx="14" fill="url(#fbg)"/>

  <rect x="300" y="18" width="400" height="2" rx="1" fill="#00d4ff">
    <animate attributeName="opacity" values="0.3;1;0.3" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="width" values="400;440;400" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="x" values="300;280;300" dur="3s" repeatCount="indefinite"/>
  </rect>

  <text x="500" y="52" text-anchor="middle"
        font-family="Segoe UI, Helvetica, Arial, sans-serif"
        font-size="16" font-weight="600" letter-spacing="1"
        fill="#a0aec0">Thanks for stopping by &#8212; let&#8217;s build something world-class</text>

  <g>
    <circle cx="150" cy="45" r="2.5" fill="#00d4ff" opacity="0.5">
      <animate attributeName="opacity" values="0.5;0.1;0.5" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="850" cy="45" r="2.5" fill="#7b61ff" opacity="0.5">
      <animate attributeName="opacity" values="0.5;0.1;0.5" dur="5s" repeatCount="indefinite"/>
    </circle>
  </g>

  <text x="500" y="76" text-anchor="middle"
        font-family="Segoe UI, Helvetica, Arial, sans-serif"
        font-size="13" letter-spacing="0.5"
        fill="#5a6a8a">daudrazzaq.me &#160;&#8226;&#160; Open to Riyadh &amp; Jeddah &#127480;&#127462;</text>
</svg>
