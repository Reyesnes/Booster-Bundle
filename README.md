# Booster Bundle — Ops Base

Base de operaciones de Booster Bundle: hub legal público, copia de trabajo del sitio en Go High Level (GHL), y espacio de contenido/ads/estrategia. Ver `CLAUDE.md` para el mapa completo del repositorio y las reglas de trabajo con Claude Code.

## 📋 Legal Hub (`docs/`)

Accesible en **legal.boosterbundle.digital**, bilingüe (EN por defecto en `/`, ES en `/es/`, EN explícito en `/en/`):

- **Términos y Condiciones** (`/terms`) — Condiciones de uso generales
- **Política de Privacidad** (`/privacy`) — Recopilación y uso de datos
- **Protección de Datos** (`/data-protection`) — Cumplimiento RGPD y LOPD-GDD
- **Política de Cookies** (`/cookies`) — Cookies y tecnologías de seguimiento
- **Eliminación de Datos** (`/data-deletion`) — Requisito de Meta/Facebook Developers

## 🗂️ Otras áreas del repositorio

- **`ghl/`** — Copia de trabajo del sitio principal, construido en Go High Level. Toda edición de código GHL usa el skill `ghl-code-builder` (ver `.claude/rules/ghl.md`).
- **`content/`** — Calendarios de contenido, copy de anuncios, contenido social, voz de marca.
- **`strategy/`** — Roadmap, OKRs y estrategia de escalado.
- **`.claude/`** — Memoria del proyecto: reglas por carpeta (`.claude/rules/`) y subagentes especializados (`.claude/agents/`).

## 🎨 Design System

Dark editorial brutalist — basado en el design system de Booster Bundle.

**Paleta:**
- `--black: #121212` — fondo principal
- `--cream: #1B1B1B` — surfaces elevadas
- `--volt: #5FD53A` — acento único
- `--white: #FFFFFF` — texto principal
- `--gray-mid: #9A9A9A` — texto secundario

**Tipografía:**
- Display: Archivo Black (uppercase)
- Labels: Space Mono (monospace)
- Body: Inter (sans-serif)

**Estructura:**
- Sharp corners (0px) — estructura
- Pill radius (999px) — interacción

## 🚀 Configuración

### GitHub Pages
1. Ir a Settings → Pages
2. Source: `Deploy from a branch` → `main` → `/docs`
3. Custom domain: `legal.boosterbundle.digital`

### DNS (GoDaddy)
```
Tipo: CNAME
Nombre: legal
Valor: reyesnes.github.io
TTL: 1 hora
```

HTTPS se activa automáticamente en 10-15 min.

## 📝 Responsable Legal

**Nestor Reyes**  
NIE: Z2377517N  
Dirección: Calle Bravo Murillo, 91, 28003 Madrid, España  
Email: legal@boosterbundle.digital

## 📦 Estructura del Repositorio

```
boosterbundle/
├── CLAUDE.md                ← memoria/reglas del proyecto para Claude Code
├── docs/                    ← Legal Hub, GitHub Pages sirve desde aquí
│   ├── CNAME
│   ├── index.html           (EN, por defecto) / es/index.html / en/index.html
│   ├── terms/ · privacy/ · data-protection/ · cookies/ · data-deletion/
│   └── es/                  (mismas rutas en español)
├── ghl/                     ← copia de trabajo del sitio en Go High Level
│   └── pages/<slug>/{source.html, notes.md}
├── content/                 ← contenido, ads, calendario, voz de marca
├── strategy/                ← roadmap, OKRs
├── .claude/
│   ├── rules/               (reglas por carpeta)
│   └── agents/              (subagentes: legal-hub-editor, ghl-maintainer, content-strategist)
├── design-system.md         (referencia)
├── design-system.html       (visual)
└── README.md                (este archivo)
```

## 🔒 Conformidad

- ✅ RGPD (EU 2016/679)
- ✅ LOPD-GDD (España)
- ✅ Ley de Cookies (LSSI-CE)
- ✅ Requisitos Meta/Facebook Developers

## 🔧 Mantenimiento

- Última actualización: Junio 2026
- Próxima revisión: Junio 2027 (o ante cambios legales)

---

*Hub legal construido con Claude Code | Design System v1.0*
