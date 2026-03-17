# Limón Digital — Website corporativo

Sitio web oficial de Limón Digital SpA. Stack: **Astro + Tailwind CSS**.

## Estructura

```
src/
├── pages/
│   ├── index.astro       ← Home
│   ├── servicios.astro   ← Servicios
│   ├── demos.astro       ← Galería de demos
│   ├── precios.astro     ← Planes y precios
│   ├── nosotros.astro    ← Sobre Limón Digital
│   └── contacto.astro    ← Formulario de contacto
├── layouts/
│   └── BaseLayout.astro  ← Layout compartido + GA4 placeholder
├── components/
│   ├── Navbar.astro      ← Navegación con active state
│   ├── Footer.astro      ← Footer corporativo
│   └── WhatsApp.astro    ← Botón flotante WhatsApp
└── styles/
    └── global.css        ← Variables de marca + animaciones
```

## Setup

```bash
npm create astro@latest . -- --template minimal --typescript strict --install --no-git
npm install
npx astro add tailwind -y
# Copia src/ y public/ del zip
npm run dev
```

## Configuraciones pendientes

- [ ] `WhatsApp.astro` — reemplaza `56900000000` con el número real
- [ ] `contacto.astro` y `demos.astro` — actualiza email de contacto
- [ ] `BaseLayout.astro` — agrega `GA_ID` cuando esté listo Google Analytics
- [ ] `demos.astro` — actualiza URL de demo-landing-basic cuando esté deployada

## Deploy

```bash
git add .
git commit -m "feat: sitio corporativo Limón Digital"
git push origin main
```

Netlify despliega automáticamente con cada push.
