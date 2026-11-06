<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1060 620" width="1060" height="620" role="img" aria-labelledby="t d">
  <title id="t">Kennith Baluyot - 3D Animated Three-Screen Studio Desk</title>
  <desc id="d">3D perspective studio desk featuring an inward-angled left monitor, center workstation monitor, and inward-angled 3D laptop on the right.</desc>
  <style>
    text { font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", monospace; }
    .sans { font-family: system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, sans-serif; }

    @keyframes ambientBreathe {
      0%, 100% { opacity: 0.75; transform: scale(1); }
      50% { opacity: 0.98; transform: scale(1.04); }
    }
    .ambient-glow {
      transform-origin: 530px 200px;
      animation: ambientBreathe 8s ease-in-out infinite;
    }

    @keyframes floatParticle {
      0% { transform: translateY(0) translateX(0); opacity: 0; }
      20% { opacity: 0.55; }
      80% { opacity: 0.55; }
      100% { transform: translateY(-90px) translateX(20px); opacity: 0; }
    }
    .dust { animation: floatParticle 13s linear infinite; }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(5px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .fi { animation: fadeUp 0.8s cubic-bezier(0.16, 1, 0.3, 1) both; }

    @keyframes draw { from { stroke-dashoffset: 650; } to { stroke-dashoffset: 0; } }
    .draw { stroke-dasharray: 650; animation: draw 2s ease-out both; }

    @keyframes typeText { from { clip-path: inset(0 100% 0 0); } to { clip-path: inset(0 0 0 0); } }
    @keyframes curBlink { 0%, 49% { opacity: 1; } 50%, 100% { opacity: 0; } }
    .blink { animation: curBlink 0.9s steps(1) infinite; }

    @keyframes monitorScan {
      0% { transform: translateY(-20px); opacity: 0; }
      20% { opacity: 0.65; }
      80% { opacity: 0.65; }
      100% { transform: translateY(240px); opacity: 0; }
    }
    .scanline { animation: monitorScan 5.5s ease-in-out infinite; }

    @keyframes skillCycle {
      0%, 18% { opacity: 1; visibility: visible; }
      20%, 100% { opacity: 0; visibility: hidden; }
    }
    .cycle-item { animation: skillCycle 20s ease-in-out infinite both; }

    @keyframes aoiLaserSweep {
      0% { transform: translateY(0); opacity: 0.35; }
      50% { transform: translateY(68px); opacity: 1; }
      100% { transform: translateY(0); opacity: 0.35; }
    }
    .laser-beam { animation: aoiLaserSweep 3.4s ease-in-out infinite; }

    @keyframes steamDrift {
      0% { transform: translateY(0) scaleX(1); opacity: 0; }
      35% { opacity: 0.5; }
      100% { transform: translateY(-22px) scaleX(1.5); opacity: 0; }
    }
    .steam { animation: steamDrift 3.2s cubic-bezier(0.4, 0, 0.2, 1) infinite; }

    @keyframes ledPulse {
      0%, 100% { opacity: 0.45; }
      50% { opacity: 1; filter: drop-shadow(0 0 3px currentColor); }
    }
    .led { animation: ledPulse 2.2s ease-in-out infinite; }

    @keyframes keyGlow {
      0%, 84%, 100% { opacity: 0; }
      90% { opacity: 0.95; }
      95% { opacity: 0.25; }
    }
    .keyhit { animation: keyGlow 4s ease-in-out infinite; }

    @keyframes catBreathe {
      0%, 100% { transform: scaleY(1) scaleX(1); }
      50% { transform: scaleY(1.04) scaleX(1.015); }
    }
    .cat-body {
      transform-box: fill-box;
      transform-origin: center bottom;
      animation: catBreathe 4.2s ease-in-out infinite;
    }

    @keyframes tailSway {
      0%, 100% { transform: rotate(0deg); }
      50% { transform: rotate(6deg); }
    }
    .cat-tail {
      transform-origin: 185px 495px;
      animation: tailSway 3.6s ease-in-out infinite;
    }

    @keyframes zzzFloat {
      0% { transform: translate(0, 0) scale(0.7); opacity: 0; }
      30% { opacity: 0.85; }
      100% { transform: translate(12px, -22px) scale(1.15); opacity: 0; }
    }
    .zzz { animation: zzzFloat 3.6s ease-out infinite; }

    @keyframes noteFlutter {
      0%, 100% { transform: rotate(0deg); }
      50% { transform: rotate(1.6deg); }
    }
    .sticky {
      transform-box: fill-box;
      transform-origin: top center;
      animation: noteFlutter 5s ease-in-out infinite;
    }

    @keyframes screenFloat {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-1.5px); }
    }
    .chibi-bob {
      transform-box: fill-box;
      transform-origin: bottom center;
      animation: screenFloat 3.5s ease-in-out infinite;
    }

    @media (prefers-reduced-motion: reduce) { * { animation: none !important; } }
  </style>

  <defs>
    <linearGradient id="bgWall" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#070b14"/>
      <stop offset="55%" stop-color="#0d1526"/>
      <stop offset="100%" stop-color="#131e36"/>
    </linearGradient>

    <pattern id="wallGrid" width="36" height="36" patternUnits="userSpaceOnUse">
      <path d="M36 0H0V36" fill="none" stroke="#1e293b" stroke-width="0.7" opacity="0.38"/>
    </pattern>

    <radialGradient id="ambientBacklight" cx="50%" cy="38%" r="52%">
      <stop offset="0%" stop-color="#38bdf8" stop-opacity="0.30"/>
      <stop offset="50%" stop-color="#a855f7" stop-opacity="0.12"/>
      <stop offset="100%" stop-color="#000000" stop-opacity="0"/>
    </radialGradient>

    <linearGradient id="deskSurface3D" x1="0" y1="0" x2="0.15" y2="1">
      <stop offset="0%" stop-color="#1e293b"/>
      <stop offset="18%" stop-color="#172133"/>
      <stop offset="70%" stop-color="#0f172a"/>
      <stop offset="100%" stop-color="#090e1a"/>
    </linearGradient>

    <linearGradient id="deskFrontLip" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#0f172a"/>
      <stop offset="50%" stop-color="#26354d"/>
      <stop offset="100%" stop-color="#0f172a"/>
    </linearGradient>

    <linearGradient id="bezelDark" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#243044"/>
      <stop offset="100%" stop-color="#0c121e"/>
    </linearGradient>

    <linearGradient id="bezel3DSide" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#3b4d6b"/>
      <stop offset="100%" stop-color="#151e2e"/>
    </linearGradient>

    <linearGradient id="silverStand" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#475569"/>
      <stop offset="45%" stop-color="#94a3b8"/>
      <stop offset="75%" stop-color="#64748b"/>
      <stop offset="100%" stop-color="#334155"/>
    </linearGradient>

    <linearGradient id="laptopBodyGrad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#64748b"/>
      <stop offset="45%" stop-color="#475569"/>
      <stop offset="100%" stop-color="#1e293b"/>
    </linearGradient>

    <linearGradient id="laptopEdgeGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#334155"/>
      <stop offset="50%" stop-color="#94a3b8"/>
      <stop offset="100%" stop-color="#1e293b"/>
    </linearGradient>

    <linearGradient id="glassReflect" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0.07"/>
      <stop offset="35%" stop-color="#ffffff" stop-opacity="0.02"/>
      <stop offset="60%" stop-color="#ffffff" stop-opacity="0"/>
    </linearGradient>

    <linearGradient id="laserGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#00f0ff" stop-opacity="0"/>
      <stop offset="20%" stop-color="#00f0ff" stop-opacity="0.75"/>
      <stop offset="50%" stop-color="#ffffff" stop-opacity="1"/>
      <stop offset="80%" stop-color="#00f0ff" stop-opacity="0.75"/>
      <stop offset="100%" stop-color="#00f0ff" stop-opacity="0"/>
    </linearGradient>

    <filter id="softGlow" x="-25%" y="-25%" width="150%" height="150%">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feComposite in="SourceGraphic" in2="blur" operator="over"/>
    </filter>

    <filter id="shadow3D" x="-20%" y="-20%" width="140%" height="140%">
      <feDropShadow dx="0" dy="8" stdDeviation="7" flood-color="#020409" flood-opacity="0.65"/>
    </filter>

    <filter id="softShadow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="5"/>
    </filter>

    <clipPath id="leftScreenClip"><rect x="0" y="0" width="246" height="196" rx="6"/></clipPath>
    <clipPath id="centerScreenClip"><rect x="322" y="42" width="376" height="248" rx="5"/></clipPath>
    <clipPath id="laptopScreenClip"><rect x="0" y="0" width="236" height="172" rx="6"/></clipPath>
  </defs>

  <rect width="1060" height="620" fill="url(#bgWall)"/>
  <rect width="1060" height="360" fill="url(#wallGrid)"/>
  <ellipse class="ambient-glow" cx="520" cy="180" rx="480" ry="170" fill="url(#ambientBacklight)"/>
  <rect x="430" y="16" width="160" height="5" rx="2.5" fill="#1e293b" stroke="#334155" stroke-width="0.8"/>
  <rect x="435" y="18.5" width="150" height="2" rx="1" fill="#f8fafc" opacity="0.92" filter="url(#softGlow)"/>

  <circle class="dust" cx="140" cy="210" r="1.2" fill="#93c5fd" style="animation-delay:-1.2s;animation-duration:13s"/>
  <circle class="dust" cx="310" cy="160" r="1.0" fill="#93c5fd" style="animation-delay:-5.4s;animation-duration:15s"/>
  <circle class="dust" cx="530" cy="240" r="1.4" fill="#c4b5fd" style="animation-delay:-8.1s;animation-duration:12s"/>
  <circle class="dust" cx="760" cy="175" r="1.1" fill="#93c5fd" style="animation-delay:-3.7s;animation-duration:14s"/>
  <circle class="dust" cx="890" cy="220" r="1.3" fill="#c4b5fd" style="animation-delay:-10.2s;animation-duration:16s"/>

  <polygon points="18,325 1042,325 1060,605 0,605" fill="#02040a" opacity="0.8"/>
  <path d="M 48,308 Q 62,296 84,296 L 976,296 Q 998,296 1012,308 L 1056,574 Q 1060,588 1042,588 L 18,588 Q 0,588 4,574 Z" fill="url(#deskSurface3D)" stroke="#2e3f5c" stroke-width="1.2"/>
  <line x1="84" y1="296" x2="18" y2="588" stroke="#26354f" stroke-width="0.8" opacity="0.3"/>
  <line x1="230" y1="296" x2="190" y2="588" stroke="#26354f" stroke-width="0.8" opacity="0.3"/>
  <line x1="380" y1="296" x2="360" y2="588" stroke="#26354f" stroke-width="0.8" opacity="0.3"/>
  <line x1="530" y1="296" x2="530" y2="588" stroke="#26354f" stroke-width="0.8" opacity="0.3"/>
  <line x1="680" y1="296" x2="700" y2="588" stroke="#26354f" stroke-width="0.8" opacity="0.3"/>
  <line x1="830" y1="296" x2="870" y2="588" stroke="#26354f" stroke-width="0.8" opacity="0.3"/>
  <line x1="976" y1="296" x2="1042" y2="588" stroke="#26354f" stroke-width="0.8" opacity="0.3"/>
  <path d="M 8,582 L 1052,582 Q 1058,582 1056,598 L 4,598 Q 2,582 8,582 Z" fill="url(#deskFrontLip)" stroke="#3b4f73" stroke-width="0.9"/>

  <ellipse cx="510" cy="355" rx="220" ry="34" fill="#38bdf8" opacity="0.12" filter="url(#softShadow)"/>
  <ellipse cx="185" cy="390" rx="135" ry="38" fill="#38bdf8" opacity="0.10" filter="url(#softShadow)"/>
  <ellipse cx="820" cy="395" rx="145" ry="42" fill="#a855f7" opacity="0.11" filter="url(#softShadow)"/>

  <g transform="translate(88, 250)">
    <ellipse cx="20" cy="68" rx="16" ry="5" fill="#04070e" opacity="0.65"/>
    <ellipse cx="20" cy="66" rx="13" ry="3.5" fill="#1e293b" stroke="#475569" stroke-width="0.8"/>
    <g class="chibi-bob">
      <path d="M12,42 L28,42 L31,62 L9,62 Z" fill="#10b981" stroke="#047857" stroke-width="1"/>
      <rect x="12" y="50" width="16" height="4" fill="#064e3b"/>
      <line x1="6" y1="46" x2="14" y2="56" stroke="#e2e8f0" stroke-width="2" stroke-linecap="round"/>
      <rect x="7" y="16" width="26" height="24" rx="8" fill="#fed7aa" stroke="#f97316" stroke-width="0.6"/>
      <path d="M5,22 L2,12 L10,15 L14,7 L20,13 L26,7 L30,15 L38,12 L35,22 Q20,16 5,22 Z" fill="#34d399" stroke="#059669" stroke-width="0.8"/>
      <circle cx="14" cy="29" r="2.2" fill="#0f172a"/>
      <circle cx="13.3" cy="28.3" r="0.7" fill="#ffffff"/>
      <line x1="23" y1="26" x2="27" y2="31" stroke="#7c2d12" stroke-width="1.3" stroke-linecap="round"/>
      <line x1="25" y1="24" x2="25" y2="33" stroke="#ef4444" stroke-width="0.9"/>
    </g>
  </g>

  <!-- CENTER MONITOR -->
  <g id="center-monitor">
    <ellipse cx="510" cy="340" rx="68" ry="11" fill="#03060c" opacity="0.75" filter="url(#softShadow)"/>
    <ellipse cx="510" cy="336" rx="58" ry="8.5" fill="url(#silverStand)" stroke="#cbd5e1" stroke-width="0.8"/>
    <ellipse cx="510" cy="334" rx="50" ry="6" fill="#1e293b"/>
    <rect x="498" y="294" width="24" height="42" rx="3" fill="url(#silverStand)"/>
    <rect x="311" y="30" width="398" height="272" rx="12" fill="url(#bezel3DSide)" filter="url(#shadow3D)"/>
    <rect x="314" y="33" width="392" height="266" rx="10" fill="url(#bezelDark)" stroke="#3b4d6b" stroke-width="1.2"/>
    <circle cx="510" cy="38" r="2.2" fill="#090d16" stroke="#334155" stroke-width="0.8"/>
    <circle class="led" cx="510" cy="38" r="0.9" fill="#22c55e"/>
    <circle class="led" cx="690" cy="294" r="1.5" fill="#38bdf8"/>

    <rect x="322" y="42" width="376" height="248" rx="5" fill="#070b13"/>
    <g clip-path="url(#centerScreenClip)">
      <rect x="322" y="42" width="376" height="248" fill="url(#wallGrid)" opacity="0.5"/>
      <rect x="322" y="42" width="376" height="19" fill="#0f172a"/>
      <circle cx="334" cy="51.5" r="3" fill="#ef4444"/>
      <circle cx="345" cy="51.5" r="3" fill="#f59e0b"/>
      <circle cx="356" cy="51.5" r="3" fill="#10b981"/>
      <text x="370" y="55" font-size="7.8" fill="#64748b">kenshin@workstation :: profile.aoi.ai</text>

      <text x="338" y="83" font-size="16" fill="#f8fafc" font-weight="800" class="fi" style="animation-delay:0.2s" letter-spacing="1.5">KENSHIN BLIRTZ</text>
      <text x="338" y="99" font-size="9.2" fill="#38bdf8" font-weight="600" style="animation:typeText 2.2s steps(30,end) 0.8s both;">Software / Automation Engineer</text>
      <rect class="blink" x="530" y="90" width="5" height="10.5" fill="#38bdf8" style="animation-delay:3s;"/>
      <line x1="338" y1="109" x2="682" y2="109" stroke="#1e2d42" stroke-width="1"/>
      <text x="338" y="121" font-size="7.2" fill="#94a3b8" class="fi" style="animation-delay:0.7s" letter-spacing="1.8">// CORE FOCUS AREAS</text>

      <rect class="fi" x="334" y="128" width="170" height="154" rx="5" fill="#0b1322" opacity="0.92" style="animation-delay:1.0s"/>
      <rect class="draw" x="334" y="128" width="170" height="154" rx="5" fill="none" stroke="#38bdf8" stroke-opacity="0.85" style="animation-delay:1.0s"/>
      <text x="344" y="145" font-size="10.2" fill="#f1f5f9" font-weight="700" class="fi" style="animation-delay:1.4s">Computer Vision</text>
      <rect x="344" y="150" width="28" height="1.8" fill="#38bdf8"/>
      <text x="344" y="162" font-size="7.0" fill="#8da2bd" class="sans fi" style="animation-delay:1.6s">Defect detection, inspection &amp;</text>
      <text x="344" y="171" font-size="7.0" fill="#8da2bd" class="sans fi" style="animation-delay:1.7s">real-time optical systems.</text>

      <g class="fi" style="animation-delay:1.80s">
        <rect x="344" y="183.5" width="3" height="3" fill="#38bdf8"/>
        <text x="352" y="188" font-size="7.5" fill="#e2e8f0" class="sans">Object Detection</text>
        <text x="352" y="196" font-size="6.2" fill="#64748b" class="sans">YOLO, Detectron, DINO</text>
      </g>
      <g class="fi" style="animation-delay:1.95s">
        <rect x="344" y="201.5" width="3" height="3" fill="#38bdf8"/>
        <text x="352" y="206" font-size="7.5" fill="#e2e8f0" class="sans">Face Recognition</text>
        <text x="352" y="214" font-size="6.2" fill="#64748b" class="sans">Biometric</text>
      </g>
      <g class="fi" style="animation-delay:2.10s">
        <rect x="344" y="219.5" width="3" height="3" fill="#38bdf8"/>
        <text x="352" y="224" font-size="7.5" fill="#e2e8f0" class="sans">CNN Architecture</text>
        <text x="352" y="232" font-size="6.2" fill="#64748b" class="sans">Feature Extraction</text>
      </g>
      <g class="fi" style="animation-delay:2.25s">
        <rect x="344" y="237.5" width="3" height="3" fill="#38bdf8"/>
        <text x="352" y="242" font-size="7.5" fill="#e2e8f0" class="sans">Annotation Pipelines</text>
        <text x="352" y="250" font-size="6.2" fill="#64748b" class="sans">CVAT, Roboflow</text>
      </g>
      <g class="fi" style="animation-delay:2.40s">
        <rect x="344" y="255.5" width="3" height="3" fill="#38bdf8"/>
        <text x="352" y="260" font-size="7.5" fill="#e2e8f0" class="sans">Optical Inspection</text>
        <text x="352" y="268" font-size="6.2" fill="#64748b" class="sans">AOI Production</text>
      </g>

      <rect class="fi" x="516" y="128" width="170" height="154" rx="5" fill="#0b1322" opacity="0.92" style="animation-delay:1.2s"/>
      <rect class="draw" x="516" y="128" width="170" height="154" rx="5" fill="none" stroke="#a855f7" stroke-opacity="0.85" style="animation-delay:1.2s"/>
      <text x="526" y="145" font-size="10.2" fill="#f1f5f9" font-weight="700" class="fi" style="animation-delay:1.5s">Applied AI</text>
      <rect x="526" y="150" width="28" height="1.8" fill="#a855f7"/>
      <text x="526" y="162" font-size="7.0" fill="#8da2bd" class="sans fi" style="animation-delay:1.7s">Connecting reasoning models to</text>
      <text x="526" y="171" font-size="7.0" fill="#8da2bd" class="sans fi" style="animation-delay:1.8s">production orchestration.</text>

      <g class="fi" style="animation-delay:2.00s">
        <rect x="526" y="183.5" width="3" height="3" fill="#a855f7"/>
        <text x="534" y="188" font-size="7.5" fill="#e2e8f0" class="sans">LLM Systems</text>
        <text x="534" y="196" font-size="6.2" fill="#64748b" class="sans">Reasoning Engines</text>
      </g>
      <g class="fi" style="animation-delay:2.15s">
        <rect x="526" y="201.5" width="3" height="3" fill="#a855f7"/>
        <text x="534" y="206" font-size="7.5" fill="#e2e8f0" class="sans">Retrieval-Augmented</text>
        <text x="534" y="214" font-size="6.2" fill="#64748b" class="sans">RAG Pipelines</text>
      </g>
      <g class="fi" style="animation-delay:2.30s">
        <rect x="526" y="219.5" width="3" height="3" fill="#a855f7"/>
        <text x="534" y="224" font-size="7.5" fill="#e2e8f0" class="sans">Agentic Workflows</text>
        <text x="534" y="232" font-size="6.2" fill="#64748b" class="sans">Autonomous Actions</text>
      </g>
      <g class="fi" style="animation-delay:2.45s">
        <rect x="526" y="237.5" width="3" height="3" fill="#a855f7"/>
        <text x="534" y="242" font-size="7.5" fill="#e2e8f0" class="sans">Orchestration</text>
        <text x="534" y="250" font-size="6.2" fill="#64748b" class="sans">n8n Automation</text>
      </g>
      <g class="fi" style="animation-delay:2.60s">
        <rect x="526" y="255.5" width="3" height="3" fill="#a855f7"/>
        <text x="534" y="260" font-size="7.5" fill="#e2e8f0" class="sans">Edge Deployment</text>
        <text x="534" y="268" font-size="6.2" fill="#64748b" class="sans">Embedded AI</text>
      </g>

      <rect class="scanline" x="322" y="42" width="376" height="22" fill="url(#laserGrad)" opacity="0.12"/>
      <polygon points="322,42 540,42 425,290 322,290" fill="url(#glassReflect)"/>
    </g>

    <g class="sticky" transform="translate(295, 62) rotate(-4)">
      <rect width="34" height="34" rx="1.5" fill="#fde047" filter="url(#shadow3D)"/>
      <line x1="5" y1="8" x2="26" y2="8" stroke="#854d0e" stroke-width="1.2" opacity="0.6"/>
      <line x1="5" y1="14" x2="28" y2="14" stroke="#854d0e" stroke-width="1" opacity="0.45"/>
      <line x1="5" y1="19" x2="22" y2="19" stroke="#854d0e" stroke-width="1" opacity="0.45"/>
    </g>
    <g class="sticky" transform="translate(293, 102) rotate(3)" style="animation-delay: -2.2s">
      <rect width="34" height="34" rx="1.5" fill="#f9a8d4" filter="url(#shadow3D)"/>
      <line x1="5" y1="9" x2="24" y2="9" stroke="#831843" stroke-width="1.2" opacity="0.6"/>
      <path d="M8,22 Q16,14 26,24" fill="none" stroke="#831843" stroke-width="1" opacity="0.5"/>
    </g>
  </g>

  <!-- 1. LEFT MONITOR -->
  <g id="left-monitor">
    <ellipse cx="176" cy="368" rx="54" ry="12" fill="#03060c" opacity="0.75" filter="url(#softShadow)" transform="rotate(-10 176 368)"/>
    <ellipse cx="176" cy="363" rx="46" ry="9.5" fill="url(#silverStand)" stroke="#cbd5e1" stroke-width="0.9" transform="rotate(-10 176 363)"/>
    <path d="M162,318 L184,312 L188,360 L166,365 Z" fill="url(#silverStand)"/>

    <g transform="matrix(0.95, -0.17, 0.045, 0.98, 34, 132)">
      <rect x="-12" y="-7" width="264" height="214" rx="12" fill="url(#bezel3DSide)" filter="url(#shadow3D)"/>
      <rect x="-7" y="-5" width="260" height="208" rx="10" fill="url(#bezelDark)" stroke="#475569" stroke-width="1.2"/>
      <rect x="0" y="0" width="246" height="196" rx="6" fill="#070b13"/>
      <g clip-path="url(#leftScreenClip)">
        <rect x="0" y="0" width="246" height="196" fill="url(#wallGrid)" opacity="0.55"/>
        <rect x="0" y="0" width="246" height="24" fill="#0f172a" opacity="0.96"/>
        <text x="14" y="15.5" font-size="8.5" fill="#38bdf8" font-weight="700" letter-spacing="1.2">TECH ARSENAL</text>
        <circle class="led" cx="230" cy="12" r="2.5" fill="#38bdf8"/>

        <rect x="12" y="31" width="41" height="15" rx="3" fill="#141e30" stroke="#223046" stroke-width="0.8"/>
        <text x="32.5" y="41.5" font-size="6.5" fill="#94a3b8" font-weight="600" text-anchor="middle">LANG</text>
        <rect x="57" y="31" width="41" height="15" rx="3" fill="#141e30" stroke="#223046" stroke-width="0.8"/>
        <text x="77.5" y="41.5" font-size="6.5" fill="#94a3b8" font-weight="600" text-anchor="middle">WEB</text>
        <rect x="102" y="31" width="41" height="15" rx="3" fill="#141e30" stroke="#223046" stroke-width="0.8"/>
        <text x="122.5" y="41.5" font-size="6.5" fill="#94a3b8" font-weight="600" text-anchor="middle">DATA</text>
        <rect x="147" y="31" width="41" height="15" rx="3" fill="#141e30" stroke="#223046" stroke-width="0.8"/>
        <text x="167.5" y="41.5" font-size="6.5" fill="#94a3b8" font-weight="600" text-anchor="middle">AI/CV</text>
        <rect x="192" y="31" width="41" height="15" rx="3" fill="#141e30" stroke="#223046" stroke-width="0.8"/>
        <text x="212.5" y="41.5" font-size="6.5" fill="#94a3b8" font-weight="600" text-anchor="middle">TOOLS</text>

        <g class="cycle-item" style="animation-delay:0s">
          <text x="14" y="64" font-size="8.5" fill="#e2e8f0" font-weight="700" letter-spacing="0.5">// PROGRAMMING</text>
          <rect x="14" y="74" width="36" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="32" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">C++</text>
          <rect x="56" y="74" width="52" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="82" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Python</text>
          <rect x="114" y="74" width="30" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="129" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">C#</text>
          <rect x="150" y="74" width="42" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="171" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Java</text>
          <rect x="14" y="98" width="42" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="35" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Dart</text>
          <rect x="62" y="98" width="42" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="83" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Rust</text>
          <rect x="110" y="98" width="58" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="139" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Arduino</text>
          <line x1="14" y1="165" x2="232" y2="165" stroke="#1e293b" stroke-width="1"/>
          <text x="14" y="180" font-size="6.8" fill="#34d399" letter-spacing="1">ACTIVE SYNC: MOD_01 [OK]</text>
        </g>

        <g class="cycle-item" style="animation-delay:4s">
          <text x="14" y="64" font-size="8.5" fill="#e2e8f0" font-weight="700" letter-spacing="0.5">// WEB DEVELOPMENT</text>
          <rect x="14" y="74" width="46" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="37" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">HTML5</text>
          <rect x="66" y="74" width="42" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="87" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">CSS3</text>
          <rect x="114" y="74" width="76" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="152" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">JavaScript</text>
          <rect x="14" y="98" width="36" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="32" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">PHP</text>
          <rect x="56" y="98" width="46" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="79" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">React</text>
          <rect x="108" y="98" width="58" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="137" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Node.js</text>
          <line x1="14" y1="165" x2="232" y2="165" stroke="#1e293b" stroke-width="1"/>
          <text x="14" y="180" font-size="6.8" fill="#34d399" letter-spacing="1">ACTIVE SYNC: MOD_02 [OK]</text>
        </g>

        <g class="cycle-item" style="animation-delay:8s">
          <text x="14" y="64" font-size="8.5" fill="#e2e8f0" font-weight="700" letter-spacing="0.5">// DATABASES</text>
          <rect x="14" y="74" width="76" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="52" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">PostgreSQL</text>
          <rect x="96" y="74" width="58" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="125" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">MongoDB</text>
          <rect x="14" y="98" width="46" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="37" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">MySQL</text>
          <rect x="66" y="98" width="52" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="92" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Oracle</text>
          <line x1="14" y1="165" x2="232" y2="165" stroke="#1e293b" stroke-width="1"/>
          <text x="14" y="180" font-size="6.8" fill="#34d399" letter-spacing="1">ACTIVE SYNC: MOD_03 [OK]</text>
        </g>

        <g class="cycle-item" style="animation-delay:12s">
          <text x="14" y="64" font-size="8.5" fill="#e2e8f0" font-weight="700" letter-spacing="0.5">// AI &amp; COMPUTER VISION</text>
          <rect x="14" y="74" width="52" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="40" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">OpenCV</text>
          <rect x="72" y="74" width="58" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="101" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">PyTorch</text>
          <rect x="136" y="74" width="58" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="165" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Jupyter</text>
          <rect x="14" y="98" width="52" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="40" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Kaggle</text>
          <rect x="72" y="98" width="64" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="104" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Roboflow</text>
          <line x1="14" y1="165" x2="232" y2="165" stroke="#1e293b" stroke-width="1"/>
          <text x="14" y="180" font-size="6.8" fill="#34d399" letter-spacing="1">ACTIVE SYNC: MOD_04 [OK]</text>
        </g>

        <g class="cycle-item" style="animation-delay:16s">
          <text x="14" y="64" font-size="8.5" fill="#e2e8f0" font-weight="700" letter-spacing="0.5">// TOOLS &amp; AUTOMATION</text>
          <rect x="14" y="74" width="34" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="31" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Git</text>
          <rect x="54" y="74" width="52" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="80" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">GitHub</text>
          <rect x="112" y="74" width="52" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="138" y="86" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Docker</text>
          <rect x="14" y="98" width="46" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="37" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">Figma</text>
          <rect x="66" y="98" width="124" height="18" rx="9" fill="#0e1a2d" stroke="#1d3557" stroke-width="1"/>
          <text x="128" y="110" font-size="7.2" fill="#7dd3fc" class="sans" text-anchor="middle">n8n Orchestration</text>
          <line x1="14" y1="165" x2="232" y2="165" stroke="#1e293b" stroke-width="1"/>
          <text x="14" y="180" font-size="6.8" fill="#34d399" letter-spacing="1">ACTIVE SYNC: MOD_05 [OK]</text>
        </g>

        <rect class="scanline" x="0" y="0" width="246" height="18" fill="url(#laserGrad)" opacity="0.15"/>
        <polygon points="0,0 140,0 75,196 0,196" fill="url(#glassReflect)"/>
      </g>
    </g>
  </g>

  <!-- 3. RIGHT LAPTOP -->
  <g id="right-laptop">
    <g transform="matrix(0.95, 0.17, -0.045, 0.97, 756, 92)">
      <rect x="-4" y="-7" width="256" height="188" rx="11" fill="url(#bezel3DSide)" filter="url(#shadow3D)"/>
      <rect x="-6" y="-5" width="248" height="184" rx="9" fill="url(#bezelDark)" stroke="#475569" stroke-width="1.2"/>
      <rect x="98" y="-5" width="40" height="6" rx="2" fill="#090d16"/>
      <circle class="led" cx="118" cy="-2" r="1" fill="#22c55e"/>

      <rect x="0" y="0" width="236" height="172" rx="6" fill="#070b13"/>
      <g clip-path="url(#laptopScreenClip)">
        <rect x="0" y="0" width="236" height="172" fill="url(#wallGrid)" opacity="0.55"/>
        <rect x="0" y="0" width="236" height="22" fill="#0f172a" opacity="0.96"/>
        <text x="12" y="14.5" font-size="8.2" fill="#a855f7" font-weight="700" letter-spacing="1.1">AOI :: TELEMETRY_FEED</text>
        <circle class="led" cx="222" cy="11" r="2.3" fill="#a855f7"/>

        <text class="fi" x="12" y="35" font-size="7.4" fill="#cbd5e1" style="animation-delay:0.8s"><tspan fill="#38bdf8">&gt;</tspan> <tspan fill="#f1f5f9">target --inspect</tspan></text>
        <text class="fi" x="12" y="47" font-size="7.4" fill="#cbd5e1" style="animation-delay:1.2s"><tspan fill="#64748b">STATUS:</tspan> <tspan fill="#34d399">ONLINE (100%)</tspan></text>
        <text class="fi" x="12" y="59" font-size="7.4" fill="#cbd5e1" style="animation-delay:1.6s"><tspan fill="#64748b">LINKEDIN:</tspan> <tspan fill="#e2e8f0">kennith-baluyot</tspan></text>
        <text class="fi" x="12" y="71" font-size="7.4" fill="#cbd5e1" style="animation-delay:2.0s"><tspan fill="#64748b">EMAIL:</tspan> <tspan fill="#e2e8f0">baluyotkennith@gmail.com</tspan></text>
        <text class="fi" x="12" y="83" font-size="7.4" fill="#cbd5e1" style="animation-delay:2.4s"><tspan fill="#64748b">PHONE:</tspan> <tspan fill="#e2e8f0">(+63) 915-719-6541</tspan></text>

        <rect x="10" y="92" width="216" height="72" rx="4" fill="#09101d" stroke="#1e2c42" stroke-width="1"/>
        <text x="18" y="103" font-size="6.5" fill="#64748b" font-weight="600" letter-spacing="0.8">OPTICAL INSPECTION :: LIVE</text>
        <text x="218" y="103" font-size="6.5" fill="#34d399" text-anchor="end">FPS: 60.0</text>

        <circle cx="32" cy="118" r="3" fill="#334155"/><circle cx="56" cy="118" r="3" fill="#334155"/><circle cx="80" cy="118" r="3" fill="#334155"/><circle cx="104" cy="118" r="3" fill="#334155"/><circle cx="128" cy="118" r="3" fill="#334155"/><circle cx="152" cy="118" r="3" fill="#334155"/><circle cx="176" cy="118" r="3" fill="#334155"/><circle cx="200" cy="118" r="3" fill="#334155"/>
        <circle cx="32" cy="133" r="3" fill="#334155"/><circle cx="56" cy="133" r="3" fill="#334155"/><circle cx="80" cy="133" r="3" fill="#334155"/><circle cx="104" cy="133" r="3" fill="#334155"/><circle cx="128" cy="133" r="3" fill="#ef4444"/><circle cx="152" cy="133" r="3" fill="#334155"/><circle cx="176" cy="133" r="3" fill="#334155"/><circle cx="200" cy="133" r="3" fill="#334155"/>
        <circle cx="32" cy="148" r="3" fill="#334155"/><circle cx="56" cy="148" r="3" fill="#334155"/><circle cx="80" cy="148" r="3" fill="#334155"/><circle cx="104" cy="148" r="3" fill="#334155"/><circle cx="128" cy="148" r="3" fill="#334155"/><circle cx="152" cy="148" r="3" fill="#334155"/><circle cx="176" cy="148" r="3" fill="#334155"/><circle cx="200" cy="148" r="3" fill="#334155"/>

        <rect class="blink" x="119" y="124" width="18" height="18" fill="none" stroke="#ef4444" stroke-width="1.2"/>
        <text x="141" y="136" font-size="6.4" fill="#ef4444" font-weight="700">DEFECT [99.4%]</text>

        <g transform="translate(10, 92)">
          <line class="laser-beam" x1="0" y1="0" x2="216" y2="0" stroke="#00f0ff" stroke-width="1.8" filter="url(#softGlow)"/>
        </g>
        <polygon points="0,0 135,0 80,172 0,172" fill="url(#glassReflect)"/>
      </g>

      <g class="sticky" transform="translate(234, 24) rotate(6)" style="animation-delay:-1.4s">
        <rect width="34" height="32" rx="1.5" fill="#93c5fd" filter="url(#shadow3D)"/>
        <line x1="5" y1="8" x2="25" y2="8" stroke="#1e3a8a" stroke-width="1.1" opacity="0.6"/>
        <line x1="5" y1="14" x2="20" y2="14" stroke="#1e3a8a" stroke-width="1" opacity="0.45"/>
      </g>
      <g class="sticky" transform="translate(232, 62) rotate(-3)" style="animation-delay:-3.1s">
        <rect width="34" height="32" rx="1.5" fill="#86efac" filter="url(#shadow3D)"/>
        <line x1="5" y1="8" x2="26" y2="8" stroke="#14532d" stroke-width="1.1" opacity="0.6"/>
        <line x1="5" y1="14" x2="22" y2="14" stroke="#14532d" stroke-width="1" opacity="0.45"/>
      </g>
    </g>

    <polygon points="738,266 984,308 920,432 666,386" fill="#02050b" opacity="0.8" filter="url(#softShadow)"/>
    <path d="M 666,378 L 912,422 L 982,306 L 982,315 L 914,431 Q 908,434 900,432 L 668,389 Q 663,387 666,378 Z" fill="url(#laptopEdgeGrad)" stroke="#475569" stroke-width="0.8"/>
    <g transform="matrix(0.95, 0.17, -0.54, 0.88, 744, 260)">
      <rect x="0" y="0" width="248" height="136" rx="10" fill="url(#laptopBodyGrad)" stroke="#94a3b8" stroke-width="0.9"/>
      <rect x="28" y="-3" width="192" height="6" rx="2" fill="#0f172a" stroke="#334155" stroke-width="0.6"/>
      <rect x="14" y="12" width="220" height="74" rx="4" fill="#0f172a" stroke="#334155" stroke-width="0.8"/>
      <line x1="18" y1="20" x2="230" y2="20" stroke="#1e293b" stroke-width="8" stroke-dasharray="11 2.2"/>
      <line x1="18" y1="32" x2="230" y2="32" stroke="#1e293b" stroke-width="9.5" stroke-dasharray="11 2.2"/>
      <line x1="18" y1="45" x2="230" y2="45" stroke="#1e293b" stroke-width="9.5" stroke-dasharray="11 2.2"/>
      <line x1="18" y1="58" x2="230" y2="58" stroke="#1e293b" stroke-width="9.5" stroke-dasharray="11 2.2"/>
      <line x1="18" y1="71" x2="230" y2="71" stroke="#1e293b" stroke-width="9.5" stroke-dasharray="11 2.2"/>
      <rect x="76" y="66.5" width="92" height="9" rx="1.5" fill="#1e293b"/>
      <rect class="keyhit" x="58" y="27.5" width="10" height="9" rx="1" fill="#a855f7" style="animation-delay:0.7s"/>
      <rect class="keyhit" x="111" y="40.5" width="10" height="9" rx="1" fill="#38bdf8" style="animation-delay:1.8s"/>
      <rect class="keyhit" x="150" y="27.5" width="10" height="9" rx="1" fill="#a855f7" style="animation-delay:2.6s"/>
      <rect class="keyhit" x="84" y="53.5" width="10" height="9" rx="1" fill="#38bdf8" style="animation-delay:3.3s"/>
      <rect x="76" y="92" width="96" height="38" rx="4" fill="#3b495e" stroke="#64748b" stroke-width="0.7"/>
      <path d="M108,135 L140,135 L137,132 L111,132 Z" fill="#1e293b"/>
    </g>
  </g>

  <!-- FOREGROUND ACCESSORIES -->
  <g transform="translate(0, 10)">
    <polygon points="295,380 685,380 702,485 278,485" fill="#090e1a" stroke="#1e293b" stroke-width="1.2"/>
    <polygon points="297,382 683,382 699,483 281,483" fill="none" stroke="#38bdf8" stroke-opacity="0.16" stroke-width="1"/>
    <polygon points="348,396 566,396 574,464 340,464" fill="#1e293b" stroke="#3b4d6b" stroke-width="1" filter="url(#shadow3D)"/>
    <polygon points="352,400 562,400 569,458 345,458" fill="#0d1422"/>
    <line x1="354" y1="408" x2="560" y2="408" stroke="#24334a" stroke-width="7" stroke-dasharray="10.5 2.2"/>
    <line x1="353" y1="419" x2="561" y2="419" stroke="#24334a" stroke-width="7" stroke-dasharray="10.5 2.2"/>
    <line x1="352" y1="430" x2="562" y2="430" stroke="#24334a" stroke-width="7" stroke-dasharray="10.5 2.2"/>
    <line x1="351" y1="441" x2="563" y2="441" stroke="#24334a" stroke-width="7" stroke-dasharray="10.5 2.2"/>
    <line x1="350" y1="451" x2="564" y2="451" stroke="#24334a" stroke-width="7" stroke-dasharray="10.5 2.2"/>
    <rect x="412" y="448" width="90" height="6.5" rx="2" fill="#334155"/>
    <rect class="keyhit" x="403" y="415.5" width="10" height="7" rx="1" fill="#38bdf8" style="animation-delay:0.4s;"/>
    <rect class="keyhit" x="454" y="426.5" width="10" height="7" rx="1" fill="#38bdf8" style="animation-delay:1.2s;"/>
    <rect class="keyhit" x="428" y="404.5" width="10" height="7" rx="1" fill="#38bdf8" style="animation-delay:2.0s;"/>
    <rect class="keyhit" x="492" y="437.5" width="10" height="7" rx="1" fill="#38bdf8" style="animation-delay:2.8s;"/>
    <line x1="344" y1="464" x2="570" y2="464" stroke="#38bdf8" stroke-width="1.5" opacity="0.85" filter="url(#softGlow)"/>
    <ellipse cx="632" cy="442" rx="16" ry="7" fill="#03060c" opacity="0.65"/>
    <rect x="618" y="408" width="28" height="44" rx="14" fill="#1e293b" stroke="#475569" stroke-width="1"/>
    <line x1="632" y1="408" x2="632" y2="424" stroke="#334155"/>
    <rect class="led" x="630" y="414" width="4" height="7" rx="2" fill="#38bdf8"/>
  </g>

  <g id="sleeping-cat">
    <ellipse cx="222" cy="518" rx="58" ry="18" fill="#04070e" opacity="0.65" filter="url(#softShadow)"/>
    <path class="cat-tail" d="M180,494 C152,492 135,512 138,542 C140,554 148,554 149,540 C150,518 164,506 184,504 Z" fill="#fb923c" stroke="#c2410c" stroke-width="1"/>
    <g class="cat-body">
      <path d="M174,492 C172,464 218,458 248,476 C268,488 272,512 252,520 C224,526 176,516 174,492 Z" fill="#fb923c" stroke="#ea580c" stroke-width="1"/>
      <path d="M196,467 Q200,484 194,496" fill="none" stroke="#c2410c" stroke-width="3" stroke-linecap="round" opacity="0.65"/>
      <path d="M214,466 Q220,484 213,498" fill="none" stroke="#c2410c" stroke-width="3" stroke-linecap="round" opacity="0.65"/>
      <path d="M232,470 Q238,486 231,500" fill="none" stroke="#c2410c" stroke-width="3" stroke-linecap="round" opacity="0.65"/>
      <circle cx="258" cy="504" r="18" fill="#fb923c" stroke="#ea580c" stroke-width="1"/>
      <polygon points="246,490 250,477 259,487" fill="#ea580c"/>
      <polygon points="264,487 274,478 274,493" fill="#ea580c"/>
      <path d="M252,506 Q256,510 260,506" fill="none" stroke="#7c2d12" stroke-width="1.4" stroke-linecap="round"/>
      <path d="M264,508 Q268,512 272,508" fill="none" stroke="#7c2d12" stroke-width="1.4" stroke-linecap="round"/>
      <circle cx="261" cy="513" r="1.6" fill="#fda4af"/>
      <ellipse cx="246" cy="518" rx="6" ry="3.5" fill="#ffedd5"/>
      <ellipse cx="266" cy="520" rx="5.5" ry="3.2" fill="#ffedd5"/>
    </g>
    <text class="zzz" x="278" y="486" font-size="9" fill="#94a3b8" font-weight="700" style="animation-delay:0s">z</text>
    <text class="zzz" x="286" y="476" font-size="11" fill="#cbd5e1" font-weight="700" style="animation-delay:1.2s">Z</text>
    <text class="zzz" x="294" y="464" font-size="13" fill="#f8fafc" font-weight="700" style="animation-delay:2.4s">Z</text>
  </g>

  <g transform="translate(56, 445) rotate(8)">
    <circle cx="14" cy="14" r="11" fill="none" stroke="#0f172a" stroke-width="3.2"/>
    <circle cx="14" cy="14" r="11" fill="#38bdf8" opacity="0.08"/>
    <circle cx="42" cy="14" r="11" fill="none" stroke="#0f172a" stroke-width="3.2"/>
    <circle cx="42" cy="14" r="11" fill="#38bdf8" opacity="0.08"/>
    <path d="M25,13 Q28,10 31,13" fill="none" stroke="#0f172a" stroke-width="2.5"/>
    <line x1="3" y1="11" x2="-8" y2="4" stroke="#0f172a" stroke-width="2.5" stroke-linecap="round"/>
  </g>

  <g transform="translate(242, 392)">
    <ellipse cx="18" cy="36" rx="16" ry="5" fill="#04070e" opacity="0.65"/>
    <path d="M30,14 Q40,20 30,28" fill="none" stroke="#475569" stroke-width="2.8"/>
    <rect x="4" y="8" width="26" height="26" rx="4" fill="#1e293b" stroke="#475569" stroke-width="1"/>
    <ellipse cx="17" cy="8" rx="13" ry="4" fill="#3b2314" stroke="#64748b" stroke-width="0.9"/>
    <path class="steam" d="M13,5 Q10,-4 13,-13" fill="none" stroke="#cbd5e1" stroke-width="1.3" stroke-linecap="round" style="animation-delay:0.0s;"/>
    <path class="steam" d="M17,5 Q14,-4 17,-13" fill="none" stroke="#cbd5e1" stroke-width="1.3" stroke-linecap="round" style="animation-delay:0.9s;"/>
    <path class="steam" d="M21,5 Q18,-4 21,-13" fill="none" stroke="#cbd5e1" stroke-width="1.3" stroke-linecap="round" style="animation-delay:1.8s;"/>
  </g>

  <g transform="translate(918, 422)">
    <ellipse cx="34" cy="96" rx="30" ry="9" fill="#03060c" opacity="0.7"/>
    <polygon points="8,88 58,98 68,78 20,68" fill="url(#silverStand)" stroke="#cbd5e1" stroke-width="0.8"/>
    <g transform="matrix(0.94, 0.19, -0.18, 0.96, 18, 0)">
      <rect x="0" y="0" width="46" height="86" rx="8" fill="#090d16" stroke="#475569" stroke-width="1.5" filter="url(#shadow3D)"/>
      <rect x="3" y="3" width="40" height="80" rx="6" fill="#0f172a"/>
      <rect x="15" y="6" width="16" height="3.5" rx="1.7" fill="#020617"/>
      <text x="23" y="24" font-size="9" fill="#f8fafc" font-weight="700" text-anchor="middle">12:00</text>
      <rect x="7" y="31" width="32" height="14" rx="3" fill="#1e293b"/>
      <text x="23" y="40" font-size="5.5" fill="#34d399" font-weight="600" text-anchor="middle">AI SYNC</text>
      <rect x="7" y="49" width="32" height="22" rx="3" fill="#141e30" stroke="#38bdf8" stroke-width="0.6"/>
      <circle class="led" cx="23" cy="60" r="3" fill="#38bdf8"/>
      <rect x="15" y="78" width="16" height="1.8" rx="0.9" fill="#64748b"/>
    </g>
  </g>

  <g transform="translate(612, 495) rotate(-5)">
    <rect x="0" y="0" width="96" height="72" rx="5" fill="#0b0f17" stroke="#334155" stroke-width="1" filter="url(#shadow3D)"/>
    <line x1="74" y1="10" x2="58" y2="66" stroke="#94a3b8" stroke-width="3" stroke-linecap="round"/>
    <line x1="74" y1="10" x2="72" y2="16" stroke="#38bdf8" stroke-width="3" stroke-linecap="round"/>
  </g>
</svg>
