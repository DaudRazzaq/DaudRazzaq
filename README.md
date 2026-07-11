<div align="center">

<!-- ═══════════════ ANIMATED HEADER ═══════════════ -->

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
