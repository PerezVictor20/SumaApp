<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 1200" width="100%" height="100%">
  <defs>
    <!-- Gradients -->
    <linearGradient id="bg-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0f172a"/>
      <stop offset="50%" stop-color="#1e1b4b"/>
      <stop offset="100%" stop-color="#311042"/>
    </linearGradient>

    <linearGradient id="accent-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#6366f1"/>
      <stop offset="50%" stop-color="#a855f7"/>
      <stop offset="100%" stop-color="#ec4899"/>
    </linearGradient>

    <linearGradient id="card-grad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0.07"/>
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0.02"/>
    </linearGradient>

    <linearGradient id="green-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#10b981"/>
      <stop offset="100%" stop-color="#059669"/>
    </linearGradient>

    <linearGradient id="orange-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#f59e0b"/>
      <stop offset="100%" stop-color="#d97706"/>
    </linearGradient>

    <!-- Drop Shadows & Glows -->
    <filter id="drop-shadow" x="-10%" y="-10%" width="120%" height="120%">
      <feDropShadow dx="0" dy="8" stdDeviation="6" flood-color="#000000" flood-opacity="0.4"/>
    </filter>

    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feComposite in="SourceGraphic" in2="blur" operator="over"/>
    </filter>

    <!-- Clip Paths -->
    <clipPath id="avatar-clip">
      <circle cx="100" cy="100" r="36"/>
    </clipPath>
  </defs>

  <style>
    .title { font-family: system-ui, -apple-system, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; font-weight: 800; fill: #ffffff; }
    .subtitle { font-family: system-ui, -apple-system, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; font-weight: 400; fill: #94a3b8; }
    .heading { font-family: system-ui, -apple-system, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; font-weight: 700; fill: #f8fafc; }
    .body-text { font-family: system-ui, -apple-system, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; font-weight: 400; fill: #cbd5e1; font-size: 14px; line-height: 1.6; }
    .code-text { font-family: 'Courier New', Courier, monospace; font-weight: 600; fill: #38bdf8; font-size: 13px; }
    .badge-text { font-family: system-ui, -apple-system, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; font-weight: 600; fill: #ffffff; font-size: 12px; }
    .card { fill: url(#card-grad); stroke: rgba(255, 255, 255, 0.1); stroke-width: 1; rx: 16px; }
    .code-block { fill: #090d16; stroke: rgba(255, 255, 255, 0.1); stroke-width: 1; rx: 8px; }
  </style>

  <!-- Background Layer -->
  <rect width="800" height="1200" fill="url(#bg-grad)"/>

  <!-- Decorative Background Grid & Glows -->
  <g opacity="0.05" stroke="#ffffff" stroke-width="1">
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40"/>
    </pattern>
    <rect width="800" height="1200" fill="url(#grid)"/>
  </g>
  <circle cx="100" cy="150" r="250" fill="#6366f1" opacity="0.15" filter="url(#glow)"/>
  <circle cx="700" cy="800" r="300" fill="#a855f7" opacity="0.12" filter="url(#glow)"/>

  <!-- HEADER SECTION -->
  <g transform="translate(50, 60)">
    <!-- App Icon Banner -->
    <rect x="0" y="0" width="72" height="72" rx="18" fill="url(#accent-grad)" filter="url(#drop-shadow)"/>
    <path d="M 24 36 L 48 36 M 36 24 L 36 48" stroke="#ffffff" stroke-width="6" stroke-linecap="round"/>
    
    <!-- Title & Subtitle -->
    <text x="92" y="34" class="title" font-size="36">SumaApp</text>
    <text x="92" y="58" class="subtitle" font-size="16">Aplicación Android de Suma Simple y Elegante</text>

    <!-- Badges -->
    <g transform="translate(0, 90)">
      <!-- Android Badge -->
      <rect x="0" y="0" width="110" height="26" rx="13" fill="#10b981" opacity="0.2"/>
      <rect x="0" y="0" width="110" height="26" rx="13" fill="none" stroke="#10b981" stroke-width="1"/>
      <circle cx="14" cy="13" r="4" fill="#10b981"/>
      <text x="26" y="17" class="badge-text" fill="#34d399">Android App</text>

      <!-- Gradle Badge -->
      <rect x="120" y="0" width="100" height="26" rx="13" fill="#6366f1" opacity="0.2"/>
      <rect x="120" y="0" width="100" height="26" rx="13" fill="none" stroke="#6366f1" stroke-width="1"/>
      <circle cx="134" cy="13" r="4" fill="#818cf8"/>
      <text x="146" y="17" class="badge-text" fill="#a5b4fc">Gradle 8.13</text>

      <!-- Kotlin Badge -->
      <rect x="230" y="0" width="120" height="26" rx="13" fill="#a855f7" opacity="0.2"/>
      <rect x="230" y="0" width="120" height="26" rx="13" fill="none" stroke="#a855f7" stroke-width="1"/>
      <circle cx="244" cy="13" r="4" fill="#c084fc"/>
      <text x="256" y="17" class="badge-text" fill="#e9d5ff">Kotlin DSL (.kts)</text>
    </g>
  </g>

  <!-- Divider Line -->
  <rect x="50" y="195" width="700" height="1" fill="url(#accent-grad)" opacity="0.4"/>

  <!-- SECTION 1: DESCRIPTION -->
  <g transform="translate(50, 220)">
    <rect x="0" y="0" width="700" height="110" class="card" filter="url(#drop-shadow)"/>
    <text x="24" y="34" class="heading" font-size="18">📌 Descripción del Proyecto</text>
    <text x="24" y="62" class="body-text">
      <tspan x="24" dy="0">SumaApp es una aplicación nativa de Android desarrollada en Kotlin. Su objetivo principal es</tspan>
      <tspan x="24" dy="22">proporcionar una interfaz sencilla para realizar cálculos aritméticos básicos (sumas) de forma</tspan>
      <tspan x="24" dy="22">rápida, segura y con una arquitectura limpia basada en las mejores prácticas de Gradle.</tspan>
    </text>
  </g>

  <!-- SECTION 2: FEATURES -->
  <g transform="translate(50, 350)">
    <rect x="0" y="0" width="700" height="165" class="card" filter="url(#drop-shadow)"/>
    <text x="24" y="34" class="heading" font-size="18">🚀 Características Principales</text>

    <!-- Bullet 1 -->
    <circle cx="32" cy="62" r="5" fill="#a855f7"/>
    <text x="48" y="66" class="body-text"><tspan font-weight="700" fill="#ffffff">Interfaz Intuitiva:</tspan> Diseño optimizado para ingresar números y obtener resultados al instante.</text>

    <!-- Bullet 2 -->
    <circle cx="32" cy="92" r="5" fill="#a855f7"/>
    <text x="48" y="96" class="body-text"><tspan font-weight="700" fill="#ffffff">Construcción Moderna:</tspan> Configurado con Kotlin DSL (<tspan class="code-text">build.gradle.kts</tspan>) y Gradle 8.13.</text>

    <!-- Bullet 3 -->
    <circle cx="32" cy="122" r="5" fill="#a855f7"/>
    <text x="48" y="126" class="body-text"><tspan font-weight="700" fill="#ffffff">Generación APK Directa:</tspan> Incluye soporte de compilación listo para generación de APKs Debug.</text>
  </g>

  <!-- SECTION 3: PROJECT STRUCTURE -->
  <g transform="translate(50, 530)">
    <rect x="0" y="0" width="700" height="210" class="card" filter="url(#drop-shadow)"/>
    <text x="24" y="34" class="heading" font-size="18">📁 Estructura del Proyecto</text>

    <!-- Structure Code View -->
    <rect x="24" y="48" width="652" height="142" class="code-block"/>
    <text x="40" y="72" class="code-text" fill="#38bdf8">SumaApp/</text>
    <text x="40" y="92" class="code-text" fill="#94a3b8">├── app/                      <tspan fill="#64748b"># Módulo principal de la aplicación</tspan></text>
    <text x="40" y="112" class="code-text" fill="#94a3b8">│   ├── build.gradle.kts      <tspan fill="#64748b"># Configuración de dependencias y Android</tspan></text>
    <text x="40" y="132" class="code-text" fill="#94a3b8">│   └── build/outputs/apk/    <tspan fill="#64748b"># Archivos binarios ejecutables (app-debug.apk)</tspan></text>
    <text x="40" y="152" class="code-text" fill="#94a3b8">├── .gradle/                  <tspan fill="#64748b"># Caché y configuración del motor Gradle (8.13)</tspan></text>
    <text x="40" y="172" class="code-text" fill="#94a3b8">└── .gitignore                <tspan fill="#64748b"># Exclusiones del control de versiones Git</tspan></text>
  </g>

  <!-- SECTION 4: INSTALLATION & COMPILATION -->
  <g transform="translate(50, 755)">
    <rect x="0" y="0" width="700" height="255" class="card" filter="url(#drop-shadow)"/>
    <text x="24" y="34" class="heading" font-size="18">🛠️ Instalación y Compilación</text>

    <!-- Step 1 -->
    <text x="24" y="65" class="body-text" font-weight="700" fill="#f43f5e">1. Clonar el repositorio:</text>
    <rect x="24" y="75" width="652" height="34" class="code-block"/>
    <text x="36" y="97" class="code-text" fill="#f1f5f9">git clone https://github.com/usuario/SumaApp.git</text>

    <!-- Step 2 -->
    <text x="24" y="132" class="body-text" font-weight="700" fill="#f43f5e">2. Abrir en Android Studio e importar Gradle.</text>

    <!-- Step 3 -->
    <text x="24" y="162" class="body-text" font-weight="700" fill="#f43f5e">3. Compilar el proyecto vía Terminal (Gradle Wrapper):</text>
    <rect x="24" y="172" width="652" height="58" class="code-block"/>
    <text x="36" y="194" class="code-text" fill="#a7f3d0"># En Linux/macOS</text>
    <text x="36" y="214" class="code-text" fill="#f1f5f9">./gradlew assembleDebug</text>
    <text x="220" y="194" class="code-text" fill="#a7f3d0"># En Windows</text>
    <text x="220" y="214" class="code-text" fill="#f1f5f9">gradlew.bat assembleDebug</text>
  </g>

  <!-- FOOTER SECTION -->
  <g transform="translate(50, 1030)">
    <rect x="0" y="0" width="700" height="110" rx="16" fill="rgba(255, 255, 255, 0.03)" stroke="rgba(255, 255, 255, 0.08)" stroke-width="1"/>
    
    <!-- Requirements -->
    <text x="24" y="32" class="heading" font-size="15" fill="#cbd5e1">📋 Requisitos del Sistema</text>
    <text x="24" y="55" class="body-text" font-size="13">
      • JDK 17 o superior  |  • Android Studio Jellyfish / Ladybug o superior  |  • Gradle 8.13+
    </text>

    <!-- License Note -->
    <rect x="24" y="70" width="652" height="1" fill="#ffffff" opacity="0.1"/>
    <text x="24" y="92" class="body-text" font-size="12" fill="#64748b">
      Proyecto generado y estructurado con éxito. Licencia MIT - Libre uso y distribución.
    </text>
  </g>
</svg>
