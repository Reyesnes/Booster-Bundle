# Booster Bundle — Legal Hub

Hub de documentos legales para Booster Bundle, accesible en **legal.boosterbundle.digital**.

## 📋 Contenido

- **Términos y Condiciones** (`/terms`) — Condiciones de uso generales
- **Política de Privacidad** (`/privacy`) — Recopilación y uso de datos
- **Protección de Datos** (`/data-protection`) — Cumplimiento RGPD y LOPD-GDD
- **Política de Cookies** (`/cookies`) — Cookies y tecnologías de seguimiento

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
├── docs/                    ← GitHub Pages sirve desde aquí
│   ├── CNAME
│   ├── index.html           (hub principal)
│   ├── terms/
│   │   └── index.html
│   ├── privacy/
│   │   └── index.html
│   ├── data-protection/
│   │   └── index.html
│   ├── cookies/
│   │   └── index.html
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
